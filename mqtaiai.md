代发 wailian999

J. 日期与时间
来源：http://cc.yuexingan06.cn

================================================================================
来源：http://zq.chemitech.net.cn

[J01] 获取当前时间
来源：http://jw.shxzukj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://uh.shxzukj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sz.hahajie.cn

JS:   new Date();  Date.now()
来源：http://jf.huanxung.cn

TS:   new Date();  Date.now()
来源：http://er.521024.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://op.lnxyls.cn

Go:   time.Now()
来源：http://ae.521024.cn

Ruby: Time.now
来源：http://ti.haigaiapp.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xn.bjjhwx.cn

[J02] 格式化输出
来源：http://wi.asd995.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iz.lnxyls.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vk.lnxyls.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ll.nicolike.cn

TS:   d.toISOString()
来源：http://zb.muxihuayi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gz.shtwfgs.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yw.huixiangedu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aj.szxytkj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ej.jianghongdianzi.cn

[J03] 字符串解析为日期
来源：http://kh.bjjhwx.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xz.colortex.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ho.colortex.cn

JS:   new Date("2024-01-02")
来源：http://ms.shtwfgs.cn

TS:   new Date("2024-01-02")
来源：http://zm.shtwfgs.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qt.lnxyls.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dp.shxzukj.cn

Ruby: Date.parse("2024-01-02")
来源：http://sb.asd995.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mb.shtwfgs.cn

[J04] 时间戳与日期互转
来源：http://kf.wgjwhj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fu.chemitech.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jy.bookmarksfly.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tt.hnjuh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://pz.chemitech.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jp.wgjwhj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kv.huixinmuqiang.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ma.bjjhwx.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://md.asd995.cn

[J05] 时间加减（加 7 天）
来源：http://uy.shxzukj.cn

Py:   now + timedelta(days=7)
来源：http://pk.hnjuh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lt.shxzukj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gj.nicolike.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://es.nicolike.cn

Java: LocalDate.now().plusDays(7)
来源：http://jd.lnxyls.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://og.gzmigu.cn

Ruby: Time.now + 7 * 86400
来源：http://lb.wgjwhj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ni.bjjhwx.cn

[J06] 计算两时间之差
来源：http://qg.shxzskj.cn

Py:   (end - start).total_seconds()
来源：http://cq.muxihuayi.cn

PHP:  $end->diff($start)->days;
来源：http://gx.nicolike.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vn.haigaiapp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wk.lnxyls.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mt.szsharing.cn

Go:   end.Sub(start).Hours()
来源：http://ix.haigaiapp.cn

Ruby: end - start                 # 返回秒数
来源：http://zv.jctech888.com.cn

C#:   (end - start).TotalSeconds
来源：http://ef.hahajie.cn

[J07] 比较两个日期
来源：http://uv.gzmigu.cn

Py:   d1 < d2;  d1 == d2
来源：http://je.asd995.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hn.chemitech.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://cv.jianghongdianzi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qr.yuexingan06.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://om.asd995.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://db.yuntaijiaju.cn

Ruby: d1 < d2;  d1 == d2
来源：http://sm.panjiajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://pf.haigaiapp.cn

[J08] 提取年月日与星期
来源：http://pv.shxzukj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://de.shxzskj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kv.shtwfgs.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bz.jianghongdianzi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tk.bookmarksfly.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qr.shxzskj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://da.muxihuayi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ob.9csxet.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cs.shxzskj.cn

[J09] 时区处理
来源：http://iy.bookmarksfly.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sa.shxzukj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wj.szxytkj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jk.jctech888.com.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ri.9csxet.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ee.nicolike.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tt.nicolike.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cx.wgjwhj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://so.szxytkj.cn

[J10] 取今天 / 本月第一天
来源：http://xr.shtwfgs.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tq.huanxung.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hf.nicolike.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mu.bookmarksfly.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lf.huixiangedu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nh.colortex.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gm.shtwfgs.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rk.9csxet.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sl.hnjuh.cn

================================================================================
来源：http://rr.panjiajie.cn

K. JSON 与序列化
来源：http://wj.bookmarksfly.cn

================================================================================
来源：http://ub.hahajie.cn

[K01] 对象转 JSON 字符串
来源：http://sl.bookmarksfly.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fp.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ek.szsharing.cn

JS:   JSON.stringify(obj)
来源：http://gz.9csxet.cn

TS:   JSON.stringify(obj)
来源：http://zr.jianghongdianzi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fi.haigaiapp.cn

Go:   json.Marshal(obj)
来源：http://iv.huixiangedu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bs.shxzskj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xc.shtwfgs.cn

[K02] JSON 字符串转对象
来源：http://fj.huixiangedu.cn

Py:   json.loads(s)
来源：http://og.yuntaijiaju.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zx.nicolike.cn

JS:   JSON.parse(s)
来源：http://jm.haigaiapp.cn

TS:   JSON.parse(s)
来源：http://at.szsharing.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bt.hahajie.cn

Go:   json.Unmarshal(data, &v)
来源：http://wx.chemitech.net.cn

Ruby: JSON.parse(s)
来源：http://un.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wo.hnjuh.cn

[K03] JSON 美化输出（带缩进）
来源：http://av.huanxung.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://az.szxytkj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fr.colortex.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bj.huixiangedu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ot.hahajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cv.9csxet.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nh.9csxet.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gj.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cm.asd995.cn

[K04] 读取 JSON 文件
来源：http://yf.colortex.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fe.yuntaijiaju.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rx.huanxung.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://db.huanxung.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://al.panjiajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wg.szsharing.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vo.szxytkj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rx.521024.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://si.hnjuh.cn

[K05] 深拷贝对象
来源：http://cg.gzmigu.cn

Py:   copy.deepcopy(obj)
来源：http://aj.521024.cn

PHP:  unserialize(serialize($obj));
来源：http://wc.newstarts.cn

JS:   structuredClone(obj)
来源：http://kp.asd995.cn

TS:   structuredClone(obj)
来源：http://on.szsharing.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dg.wgjwhj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xa.chemitech.net.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dg.hahajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cl.bjjhwx.cn

[K06] 解析 URL 查询串
来源：http://gk.shxzskj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ey.nszjky.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xr.huixinmuqiang.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ti.bjjhwx.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yx.bjjhwx.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dy.panjiajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sk.wgjwhj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://in.huixinmuqiang.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ji.yuexingan06.cn

[K07] 进制转换
来源：http://ho.asd995.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gv.9csxet.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://za.yuntaijiaju.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vf.hahajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nk.wgjwhj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ip.huanxung.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bd.shxzukj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nl.wgjwhj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fb.bjjhwx.cn

[K08] 二进制序列化（非 JSON）
来源：http://pi.colortex.cn

Py:   pickle.dumps(obj)
来源：http://rc.gzmigu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://jo.szxytkj.cn

JS:   v8.serialize(obj)        // Node
来源：http://ak.muxihuayi.cn

TS:   v8.serialize(obj)        // Node
来源：http://ng.szxytkj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ly.nicolike.cn

Go:   encoding/gob
来源：http://fz.hnjuh.cn

Ruby: Marshal.dump(obj)
来源：http://wl.asd995.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lo.asd995.cn

================================================================================
来源：http://kj.gzmigu.cn

L. 网络请求
来源：http://ze.colortex.cn

================================================================================
来源：http://kb.szxytkj.cn

[L01] 发送 GET 请求
来源：http://cw.gzmigu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tt.521024.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mf.yuntaijiaju.cn

JS:   await fetch(url)
来源：http://ad.bjjhwx.cn

TS:   await fetch(url)
来源：http://sc.huanxung.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hc.asd995.cn

Go:   resp, err := http.Get(url)
来源：http://mv.521024.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fq.bookmarksfly.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zq.muxihuayi.cn

[L02] 发送 POST JSON
来源：http://um.asd995.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wp.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fh.panjiajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zo.nicolike.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://er.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://il.9csxet.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://se.lnxyls.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wf.muxihuayi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lg.wgjwhj.cn

[L03] 设置自定义请求头
来源：http://jt.hnjuh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jb.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mf.haigaiapp.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mv.huanxung.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vl.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ye.chemitech.net.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ws.shxzskj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://eh.bookmarksfly.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wz.gzmigu.cn

[L04] 设置超时
来源：http://hf.yuexingan06.cn

Py:   requests.get(url, timeout=5)
来源：http://yz.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ap.huixiangedu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kp.nicolike.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hu.jctech888.com.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ev.huanxung.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lb.bjjhwx.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ca.colortex.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qy.szxytkj.cn

[L05] 上传文件（multipart）
来源：http://dv.szsharing.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gz.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sx.hahajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ma.jctech888.com.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wo.nicolike.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vg.jctech888.com.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qf.lnxyls.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://la.newstarts.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yg.huixinmuqiang.cn

[L06] 解析响应为 JSON
来源：http://gg.nicolike.cn

Py:   resp.json()
来源：http://pf.shxzukj.cn

PHP:  json_decode($body, true);
来源：http://xt.haigaiapp.cn

JS:   await resp.json()
来源：http://om.jianghongdianzi.cn

TS:   await resp.json()
来源：http://rt.nicolike.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ch.gzmigu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ht.nszjky.cn

Ruby: JSON.parse(resp.body)
来源：http://yt.nicolike.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://di.szsharing.cn

[L07] 处理 HTTP 状态码
来源：http://df.muxihuayi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tm.szxytkj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xn.hnjuh.cn

JS:   resp.ok;  resp.status
来源：http://fg.panjiajie.cn

TS:   resp.ok;  resp.status
来源：http://wr.jctech888.com.cn

Java: resp.statusCode()
来源：http://ce.huixiangedu.cn

Go:   resp.StatusCode
来源：http://js.asd995.cn

Ruby: resp.code.to_i
来源：http://zw.huixinmuqiang.cn

C#:   (int)resp.StatusCode
来源：http://vq.9csxet.cn

[L08] 并发请求多个地址
来源：http://oz.nszjky.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ev.szsharing.cn

PHP:  curl_multi_init() 系列
来源：http://an.huixinmuqiang.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qg.asd995.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nz.hahajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dh.haigaiapp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ca.shtwfgs.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gh.chemitech.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hd.nszjky.cn

================================================================================
来源：http://qh.shtwfgs.cn

M. 命令行 / 进程 / 环境
来源：http://mb.jianghongdianzi.cn

================================================================================
来源：http://ls.muxihuayi.cn

[M01] 读取命令行参数
来源：http://wj.gzmigu.cn

Py:   sys.argv[1:]
来源：http://pq.jctech888.com.cn

PHP:  $argv;  $argc;
来源：http://sb.yuexingan06.cn

JS:   process.argv.slice(2)
来源：http://bv.yuexingan06.cn

TS:   process.argv.slice(2)
来源：http://ra.jianghongdianzi.cn

Java: args 数组（main 方法参数）
来源：http://zj.gzmigu.cn

Go:   os.Args[1:]
来源：http://yg.szxytkj.cn

Ruby: ARGV
来源：http://cr.shtwfgs.cn

C#:   args 数组（Main 方法参数）
来源：http://oj.nicolike.cn

[M02] 读取环境变量
来源：http://vy.wgjwhj.cn

Py:   os.environ.get("HOME")
来源：http://lo.lnxyls.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cf.gzmigu.cn

JS:   process.env.HOME
来源：http://vd.asd995.cn

TS:   process.env.HOME
来源：http://sf.huixiangedu.cn

Java: System.getenv("HOME")
来源：http://yu.shxzskj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kz.yuntaijiaju.cn

Ruby: ENV["HOME"]
来源：http://kf.nicolike.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gq.lnxyls.cn

[M03] 执行外部命令
来源：http://cy.szxytkj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lc.521024.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wq.lnxyls.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jt.yuntaijiaju.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gz.9csxet.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nx.yuexingan06.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ky.521024.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kg.newstarts.cn

C#:   Process.Start("ls", "-l");
来源：http://qa.shxzukj.cn

[M04] 获取当前工作目录
来源：http://px.yuntaijiaju.cn

Py:   os.getcwd()
来源：http://cn.hnjuh.cn

PHP:  getcwd();
来源：http://sk.colortex.cn

JS:   process.cwd()
来源：http://rj.shtwfgs.cn

TS:   process.cwd()
来源：http://mf.lnxyls.cn

Java: Path.of("").toAbsolutePath()
来源：http://km.haigaiapp.cn

Go:   os.Getwd()
来源：http://sv.szxytkj.cn

Ruby: Dir.pwd
来源：http://jr.jctech888.com.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ar.shtwfgs.cn

[M05] 设置退出码
来源：http://sq.nszjky.cn

Py:   sys.exit(1)
来源：http://hj.huixiangedu.cn

PHP:  exit(1);
来源：http://tj.huanxung.cn

JS:   process.exit(1)
来源：http://hj.bjjhwx.cn

TS:   process.exit(1)
来源：http://ha.9csxet.cn

Java: System.exit(1)
来源：http://jp.hahajie.cn

Go:   os.Exit(1)
来源：http://mx.asd995.cn

Ruby: exit 1
来源：http://jk.521024.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wd.hnjuh.cn

[M06] 向标准错误输出
来源：http://pf.gzmigu.cn

Py:   print("err", file=sys.stderr)
来源：http://lo.nszjky.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tv.jianghongdianzi.cn

JS:   console.error("err")
来源：http://ft.nszjky.cn

TS:   console.error("err")
来源：http://fh.colortex.cn

Java: System.err.println("err")
来源：http://mj.huixiangedu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bl.nszjky.cn

Ruby: warn "err"
来源：http://al.huixinmuqiang.cn

C#:   Console.Error.WriteLine("err")
来源：http://kk.bookmarksfly.cn

[M07] 判断是否为主入口
来源：http://pa.asd995.cn


<!-- 参考信息 -->