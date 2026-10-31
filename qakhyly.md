代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rw.nszjky.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ic.muxihuayi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ph.muxihuayi.cn

================================================================================
来源：http://ni.bookmarksfly.cn

J. 日期与时间
来源：http://wc.szxytkj.cn

================================================================================
来源：http://wg.asd995.cn

[J01] 获取当前时间
来源：http://qe.jianghongdianzi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ln.panjiajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fl.muxihuayi.cn

JS:   new Date();  Date.now()
来源：http://ao.lnxyls.cn

TS:   new Date();  Date.now()
来源：http://xf.jianghongdianzi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://xj.9csxet.cn

Go:   time.Now()
来源：http://ct.hahajie.cn

Ruby: Time.now
来源：http://uz.haigaiapp.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://og.hahajie.cn

[J02] 格式化输出
来源：http://cs.gzmigu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://od.jctech888.com.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yu.gzmigu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bu.szsharing.cn

TS:   d.toISOString()
来源：http://jc.nicolike.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mt.shxzskj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://uk.bjjhwx.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dp.bookmarksfly.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ml.colortex.cn

[J03] 字符串解析为日期
来源：http://kr.jianghongdianzi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mb.huixiangedu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tk.jctech888.com.cn

JS:   new Date("2024-01-02")
来源：http://hg.9csxet.cn

TS:   new Date("2024-01-02")
来源：http://hc.hnjuh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ry.gzmigu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kj.shxzukj.cn

Ruby: Date.parse("2024-01-02")
来源：http://tf.gzmigu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://md.yuntaijiaju.cn

[J04] 时间戳与日期互转
来源：http://qw.asd995.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://it.chemitech.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sq.gzmigu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gx.yuexingan06.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://pq.newstarts.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ol.asd995.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kj.gzmigu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ky.asd995.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://je.gzmigu.cn

[J05] 时间加减（加 7 天）
来源：http://wv.bookmarksfly.cn

Py:   now + timedelta(days=7)
来源：http://rf.wgjwhj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://fw.asd995.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://oh.yuexingan06.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://iy.wgjwhj.cn

Java: LocalDate.now().plusDays(7)
来源：http://un.jctech888.com.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://so.wgjwhj.cn

Ruby: Time.now + 7 * 86400
来源：http://gy.huanxung.cn

C#:   DateTime.Now.AddDays(7)
来源：http://lt.huixiangedu.cn

[J06] 计算两时间之差
来源：http://vt.wgjwhj.cn

Py:   (end - start).total_seconds()
来源：http://dw.nicolike.cn

PHP:  $end->diff($start)->days;
来源：http://jg.huixiangedu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vh.newstarts.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sl.muxihuayi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://nq.asd995.cn

Go:   end.Sub(start).Hours()
来源：http://rt.9csxet.cn

Ruby: end - start                 # 返回秒数
来源：http://db.shtwfgs.cn

C#:   (end - start).TotalSeconds
来源：http://xc.huixiangedu.cn

[J07] 比较两个日期
来源：http://ge.bookmarksfly.cn

Py:   d1 < d2;  d1 == d2
来源：http://jo.jianghongdianzi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hh.hahajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jh.asd995.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ui.wgjwhj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tw.shxzskj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rr.huanxung.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ov.szsharing.cn

C#:   d1 < d2;  d1 == d2
来源：http://el.jctech888.com.cn

[J08] 提取年月日与星期
来源：http://nh.yuexingan06.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cp.shxzskj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qm.huanxung.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vz.jctech888.com.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zk.shxzskj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://az.shxzskj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qi.gzmigu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yu.yuexingan06.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pu.panjiajie.cn

[J09] 时区处理
来源：http://zd.huanxung.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vd.nszjky.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://uz.bjjhwx.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wr.521024.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hu.nicolike.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vs.shxzukj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ph.panjiajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cp.lnxyls.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zd.muxihuayi.cn

[J10] 取今天 / 本月第一天
来源：http://oj.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://yi.wgjwhj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ft.lnxyls.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wz.521024.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ir.colortex.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://iu.521024.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nw.nicolike.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lr.muxihuayi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nf.nszjky.cn

================================================================================
来源：http://ys.nszjky.cn

K. JSON 与序列化
来源：http://vz.szxytkj.cn

================================================================================
来源：http://ru.colortex.cn

[K01] 对象转 JSON 字符串
来源：http://sz.shxzukj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://to.muxihuayi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xj.wgjwhj.cn

JS:   JSON.stringify(obj)
来源：http://xj.huixiangedu.cn

TS:   JSON.stringify(obj)
来源：http://ka.9csxet.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nr.hahajie.cn

Go:   json.Marshal(obj)
来源：http://vk.jctech888.com.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mw.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://db.nicolike.cn

[K02] JSON 字符串转对象
来源：http://fw.asd995.cn

Py:   json.loads(s)
来源：http://gy.shxzskj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yk.szsharing.cn

JS:   JSON.parse(s)
来源：http://qv.lnxyls.cn

TS:   JSON.parse(s)
来源：http://qx.szxytkj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qn.yuntaijiaju.cn

Go:   json.Unmarshal(data, &v)
来源：http://pi.yuntaijiaju.cn

Ruby: JSON.parse(s)
来源：http://bm.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sr.hahajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://um.shxzskj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lz.szxytkj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fe.hnjuh.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://lg.9csxet.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://lt.asd995.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ux.hnjuh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ss.shtwfgs.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hv.panjiajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yl.521024.cn

[K04] 读取 JSON 文件
来源：http://sx.bjjhwx.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kl.jianghongdianzi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cu.nicolike.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kf.asd995.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ig.gzmigu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xs.asd995.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zn.huanxung.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://km.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ly.szsharing.cn

[K05] 深拷贝对象
来源：http://nf.hnjuh.cn

Py:   copy.deepcopy(obj)
来源：http://zj.newstarts.cn

PHP:  unserialize(serialize($obj));
来源：http://tb.nszjky.cn

JS:   structuredClone(obj)
来源：http://sr.haigaiapp.cn

TS:   structuredClone(obj)
来源：http://ml.nicolike.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://lj.shtwfgs.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qo.521024.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://re.9csxet.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yq.hnjuh.cn

[K06] 解析 URL 查询串
来源：http://bj.muxihuayi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://na.9csxet.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ls.yuntaijiaju.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pz.hahajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hg.nszjky.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xa.shxzskj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rl.shxzukj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bw.szsharing.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gf.lnxyls.cn

[K07] 进制转换
来源：http://oi.9csxet.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fe.shxzskj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ev.shxzukj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://la.jianghongdianzi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lx.chemitech.net.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://eo.panjiajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jr.huanxung.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zo.jianghongdianzi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://aj.nicolike.cn

[K08] 二进制序列化（非 JSON）
来源：http://lz.haigaiapp.cn

Py:   pickle.dumps(obj)
来源：http://vr.chemitech.net.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wb.szxytkj.cn

JS:   v8.serialize(obj)        // Node
来源：http://em.bjjhwx.cn

TS:   v8.serialize(obj)        // Node
来源：http://ov.9csxet.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ou.haigaiapp.cn

Go:   encoding/gob
来源：http://ap.521024.cn

Ruby: Marshal.dump(obj)
来源：http://ym.bookmarksfly.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mc.panjiajie.cn

================================================================================
来源：http://kp.szsharing.cn

L. 网络请求
来源：http://dk.huixiangedu.cn

================================================================================
来源：http://sd.yuntaijiaju.cn

[L01] 发送 GET 请求
来源：http://is.nszjky.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wz.muxihuayi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mc.huanxung.cn

JS:   await fetch(url)
来源：http://cc.huixinmuqiang.cn

TS:   await fetch(url)
来源：http://ik.chemitech.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cg.shxzukj.cn

Go:   resp, err := http.Get(url)
来源：http://ya.521024.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://yo.yuexingan06.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rv.nicolike.cn

[L02] 发送 POST JSON
来源：http://jj.bookmarksfly.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xc.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pv.muxihuayi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yi.panjiajie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bm.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yf.shxzskj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tq.huanxung.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://in.szxytkj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qy.szsharing.cn

[L03] 设置自定义请求头
来源：http://gl.shtwfgs.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yl.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yh.bjjhwx.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vt.wgjwhj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dr.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cw.szxytkj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cb.yuexingan06.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://oq.gzmigu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wh.yuexingan06.cn

[L04] 设置超时
来源：http://fb.yuntaijiaju.cn

Py:   requests.get(url, timeout=5)
来源：http://ms.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pz.shxzukj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ov.asd995.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dg.gzmigu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kf.yuexingan06.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://op.szxytkj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tq.lnxyls.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xn.yuexingan06.cn

[L05] 上传文件（multipart）
来源：http://kb.szxytkj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dr.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cs.asd995.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ff.nszjky.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yf.nicolike.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://je.shxzskj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://md.hahajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gx.asd995.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://at.jctech888.com.cn

[L06] 解析响应为 JSON
来源：http://vl.szxytkj.cn

Py:   resp.json()
来源：http://xd.gzmigu.cn

PHP:  json_decode($body, true);
来源：http://se.nicolike.cn

JS:   await resp.json()
来源：http://lm.asd995.cn

TS:   await resp.json()
来源：http://vi.hahajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kv.haigaiapp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ne.huixiangedu.cn

Ruby: JSON.parse(resp.body)
来源：http://nw.yuexingan06.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bj.shxzskj.cn

[L07] 处理 HTTP 状态码
来源：http://le.asd995.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://br.szsharing.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jc.muxihuayi.cn

JS:   resp.ok;  resp.status
来源：http://fd.jianghongdianzi.cn

TS:   resp.ok;  resp.status
来源：http://fx.hnjuh.cn

Java: resp.statusCode()
来源：http://sw.hahajie.cn

Go:   resp.StatusCode
来源：http://ob.gzmigu.cn

Ruby: resp.code.to_i
来源：http://fk.wgjwhj.cn

C#:   (int)resp.StatusCode
来源：http://lk.muxihuayi.cn

[L08] 并发请求多个地址
来源：http://un.panjiajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://oq.hahajie.cn

PHP:  curl_multi_init() 系列
来源：http://hu.shtwfgs.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ef.jianghongdianzi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xb.hnjuh.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xs.jianghongdianzi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uk.newstarts.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yi.yuntaijiaju.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sr.521024.cn

================================================================================
来源：http://sx.yuexingan06.cn

M. 命令行 / 进程 / 环境
来源：http://gr.jianghongdianzi.cn

================================================================================
来源：http://jl.shxzukj.cn

[M01] 读取命令行参数
来源：http://hq.asd995.cn

Py:   sys.argv[1:]
来源：http://jp.lnxyls.cn

PHP:  $argv;  $argc;
来源：http://xd.shxzukj.cn

JS:   process.argv.slice(2)
来源：http://cd.asd995.cn

TS:   process.argv.slice(2)
来源：http://jw.9csxet.cn

Java: args 数组（main 方法参数）
来源：http://va.chemitech.net.cn

Go:   os.Args[1:]
来源：http://fp.huanxung.cn

Ruby: ARGV
来源：http://pf.huixiangedu.cn

C#:   args 数组（Main 方法参数）
来源：http://sh.9csxet.cn

[M02] 读取环境变量
来源：http://go.wgjwhj.cn

Py:   os.environ.get("HOME")
来源：http://gu.hnjuh.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dk.yuexingan06.cn

JS:   process.env.HOME
来源：http://uz.newstarts.cn

TS:   process.env.HOME
来源：http://oi.szsharing.cn

Java: System.getenv("HOME")
来源：http://ht.521024.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sl.yuexingan06.cn

Ruby: ENV["HOME"]
来源：http://ho.shtwfgs.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://im.haigaiapp.cn

[M03] 执行外部命令
来源：http://ke.bjjhwx.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://av.chemitech.net.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yi.huanxung.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vd.shxzukj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mn.huixiangedu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://db.bookmarksfly.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://kz.jctech888.com.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ch.bjjhwx.cn

C#:   Process.Start("ls", "-l");
来源：http://sd.asd995.cn

[M04] 获取当前工作目录
来源：http://in.asd995.cn

Py:   os.getcwd()
来源：http://yy.521024.cn

PHP:  getcwd();
来源：http://cj.chemitech.net.cn

JS:   process.cwd()
来源：http://pp.jianghongdianzi.cn

TS:   process.cwd()
来源：http://kh.hnjuh.cn

Java: Path.of("").toAbsolutePath()
来源：http://wc.bookmarksfly.cn

Go:   os.Getwd()
来源：http://ay.nszjky.cn

Ruby: Dir.pwd
来源：http://cn.521024.cn

C#:   Directory.GetCurrentDirectory()
来源：http://uu.shxzskj.cn

[M05] 设置退出码
来源：http://vd.hahajie.cn

Py:   sys.exit(1)
来源：http://ku.wgjwhj.cn

PHP:  exit(1);
来源：http://am.asd995.cn

JS:   process.exit(1)
来源：http://pz.huanxung.cn

TS:   process.exit(1)
来源：http://lf.nicolike.cn

Java: System.exit(1)
来源：http://im.szxytkj.cn

Go:   os.Exit(1)
来源：http://ly.szsharing.cn

Ruby: exit 1
来源：http://ut.muxihuayi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yu.huixiangedu.cn

[M06] 向标准错误输出
来源：http://cu.huixinmuqiang.cn

Py:   print("err", file=sys.stderr)
来源：http://ky.muxihuayi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hw.huanxung.cn

JS:   console.error("err")
来源：http://qe.haigaiapp.cn

TS:   console.error("err")
来源：http://xj.hahajie.cn

Java: System.err.println("err")
来源：http://hh.bjjhwx.cn


<!-- 参考信息 -->