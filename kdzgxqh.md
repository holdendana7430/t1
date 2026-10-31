代发 wailian999

J. 日期与时间
来源：http://yh.huixiangedu.cn

================================================================================
来源：http://bv.yuntaijiaju.cn

[J01] 获取当前时间
来源：http://tp.newstarts.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hq.521024.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zi.huixiangedu.cn

JS:   new Date();  Date.now()
来源：http://is.asd995.cn

TS:   new Date();  Date.now()
来源：http://cf.yuntaijiaju.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://oe.nszjky.cn

Go:   time.Now()
来源：http://xn.colortex.cn

Ruby: Time.now
来源：http://in.shxzskj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bc.panjiajie.cn

[J02] 格式化输出
来源：http://lv.haigaiapp.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mm.chemitech.net.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qr.nicolike.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tj.panjiajie.cn

TS:   d.toISOString()
来源：http://dw.yuexingan06.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ay.nszjky.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bz.colortex.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://un.shxzukj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bs.yuexingan06.cn

[J03] 字符串解析为日期
来源：http://ah.shxzskj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gg.shxzukj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fw.shtwfgs.cn

JS:   new Date("2024-01-02")
来源：http://cp.jctech888.com.cn

TS:   new Date("2024-01-02")
来源：http://ol.asd995.cn

Java: LocalDate.parse("2024-01-02")
来源：http://es.gzmigu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ve.bookmarksfly.cn

Ruby: Date.parse("2024-01-02")
来源：http://xh.yuexingan06.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ug.haigaiapp.cn

[J04] 时间戳与日期互转
来源：http://nr.bjjhwx.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://al.szxytkj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ae.colortex.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bh.yuexingan06.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ez.wgjwhj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lj.nicolike.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fz.shtwfgs.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jr.nszjky.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jv.hahajie.cn

[J05] 时间加减（加 7 天）
来源：http://jd.bjjhwx.cn

Py:   now + timedelta(days=7)
来源：http://mk.hahajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://gi.chemitech.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ez.yuntaijiaju.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rg.bookmarksfly.cn

Java: LocalDate.now().plusDays(7)
来源：http://kq.hnjuh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rz.huixiangedu.cn

Ruby: Time.now + 7 * 86400
来源：http://gr.panjiajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://oq.haigaiapp.cn

[J06] 计算两时间之差
来源：http://ja.huixinmuqiang.cn

Py:   (end - start).total_seconds()
来源：http://pd.huixinmuqiang.cn

PHP:  $end->diff($start)->days;
来源：http://zf.huixiangedu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bf.asd995.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ft.shtwfgs.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qi.hnjuh.cn

Go:   end.Sub(start).Hours()
来源：http://is.bjjhwx.cn

Ruby: end - start                 # 返回秒数
来源：http://pl.szsharing.cn

C#:   (end - start).TotalSeconds
来源：http://bm.gzmigu.cn

[J07] 比较两个日期
来源：http://pp.huanxung.cn

Py:   d1 < d2;  d1 == d2
来源：http://ri.huanxung.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bt.hnjuh.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kb.muxihuayi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bl.gzmigu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kr.newstarts.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ay.521024.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xx.asd995.cn

C#:   d1 < d2;  d1 == d2
来源：http://sv.haigaiapp.cn

[J08] 提取年月日与星期
来源：http://nm.nicolike.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dk.huixinmuqiang.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://if.9csxet.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kw.panjiajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ee.9csxet.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rr.wgjwhj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pp.bookmarksfly.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ov.shxzukj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://no.colortex.cn

[J09] 时区处理
来源：http://or.nszjky.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://df.hahajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qp.szxytkj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://it.9csxet.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ll.wgjwhj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://um.szxytkj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zd.wgjwhj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zl.nicolike.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dz.hnjuh.cn

[J10] 取今天 / 本月第一天
来源：http://hc.9csxet.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vk.wgjwhj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ec.huixiangedu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xv.shtwfgs.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kz.jianghongdianzi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://db.colortex.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zv.nszjky.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wi.nszjky.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qu.yuexingan06.cn

================================================================================
来源：http://kh.nszjky.cn

K. JSON 与序列化
来源：http://au.szsharing.cn

================================================================================
来源：http://pn.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://af.nicolike.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ft.jctech888.com.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://su.lnxyls.cn

JS:   JSON.stringify(obj)
来源：http://qz.nicolike.cn

TS:   JSON.stringify(obj)
来源：http://hq.gzmigu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pf.lnxyls.cn

Go:   json.Marshal(obj)
来源：http://um.szxytkj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cf.521024.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://sl.asd995.cn

[K02] JSON 字符串转对象
来源：http://ng.muxihuayi.cn

Py:   json.loads(s)
来源：http://cn.shxzskj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hf.asd995.cn

JS:   JSON.parse(s)
来源：http://fh.bookmarksfly.cn

TS:   JSON.parse(s)
来源：http://wi.jianghongdianzi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ey.muxihuayi.cn

Go:   json.Unmarshal(data, &v)
来源：http://gz.hnjuh.cn

Ruby: JSON.parse(s)
来源：http://lm.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vt.muxihuayi.cn

[K03] JSON 美化输出（带缩进）
来源：http://xo.hahajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wl.jctech888.com.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lt.bookmarksfly.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pf.hahajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://we.521024.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sn.shxzskj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ho.huixiangedu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ge.asd995.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://oh.shxzskj.cn

[K04] 读取 JSON 文件
来源：http://yy.hahajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yj.bookmarksfly.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mn.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zn.shxzskj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uf.gzmigu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uh.hnjuh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yf.chemitech.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://nf.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zw.yuntaijiaju.cn

[K05] 深拷贝对象
来源：http://cm.huixinmuqiang.cn

Py:   copy.deepcopy(obj)
来源：http://ih.huanxung.cn

PHP:  unserialize(serialize($obj));
来源：http://co.shxzukj.cn

JS:   structuredClone(obj)
来源：http://ey.wgjwhj.cn

TS:   structuredClone(obj)
来源：http://lq.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bn.nszjky.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xs.huixinmuqiang.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wp.haigaiapp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xz.gzmigu.cn

[K06] 解析 URL 查询串
来源：http://ks.hahajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kf.nicolike.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zk.nszjky.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://um.asd995.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://la.nicolike.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jw.hnjuh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sm.asd995.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wl.yuexingan06.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lw.huanxung.cn

[K07] 进制转换
来源：http://dv.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mt.panjiajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yu.huixiangedu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qy.haigaiapp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lo.newstarts.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://br.haigaiapp.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nk.shxzskj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ai.asd995.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ky.hahajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://gs.nszjky.cn

Py:   pickle.dumps(obj)
来源：http://ku.shxzskj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vt.huixiangedu.cn

JS:   v8.serialize(obj)        // Node
来源：http://zn.gzmigu.cn

TS:   v8.serialize(obj)        // Node
来源：http://fr.bookmarksfly.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wd.shtwfgs.cn

Go:   encoding/gob
来源：http://ku.colortex.cn

Ruby: Marshal.dump(obj)
来源：http://kr.9csxet.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ej.huixinmuqiang.cn

================================================================================
来源：http://sm.newstarts.cn

L. 网络请求
来源：http://zo.shxzukj.cn

================================================================================
来源：http://me.huixiangedu.cn

[L01] 发送 GET 请求
来源：http://pp.panjiajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qc.bookmarksfly.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dv.hnjuh.cn

JS:   await fetch(url)
来源：http://yi.asd995.cn

TS:   await fetch(url)
来源：http://wk.9csxet.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hk.panjiajie.cn

Go:   resp, err := http.Get(url)
来源：http://xx.newstarts.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xb.szxytkj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ln.bookmarksfly.cn

[L02] 发送 POST JSON
来源：http://jv.jctech888.com.cn

Py:   requests.post(url, json={"a": 1})
来源：http://we.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ax.szsharing.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ak.szsharing.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xf.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://in.shxzskj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://az.shxzskj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sr.9csxet.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hy.newstarts.cn

[L03] 设置自定义请求头
来源：http://ub.jctech888.com.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vq.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hc.szxytkj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zq.huixiangedu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fq.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vs.yuexingan06.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qn.wgjwhj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hg.521024.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cn.panjiajie.cn

[L04] 设置超时
来源：http://rs.bookmarksfly.cn

Py:   requests.get(url, timeout=5)
来源：http://fp.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sd.nicolike.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://py.bookmarksfly.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ee.nicolike.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ko.521024.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://co.hahajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nb.shxzskj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xq.521024.cn

[L05] 上传文件（multipart）
来源：http://ct.colortex.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ro.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nb.panjiajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xz.nicolike.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rl.bjjhwx.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cl.yuntaijiaju.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xx.521024.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ta.bjjhwx.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zr.yuexingan06.cn

[L06] 解析响应为 JSON
来源：http://uf.yuexingan06.cn

Py:   resp.json()
来源：http://sf.shxzskj.cn

PHP:  json_decode($body, true);
来源：http://ka.hahajie.cn

JS:   await resp.json()
来源：http://tu.colortex.cn

TS:   await resp.json()
来源：http://xr.wgjwhj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qf.huixinmuqiang.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ve.jctech888.com.cn

Ruby: JSON.parse(resp.body)
来源：http://xq.jctech888.com.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wc.wgjwhj.cn

[L07] 处理 HTTP 状态码
来源：http://ni.9csxet.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fa.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dw.chemitech.net.cn

JS:   resp.ok;  resp.status
来源：http://jn.nszjky.cn

TS:   resp.ok;  resp.status
来源：http://dn.muxihuayi.cn

Java: resp.statusCode()
来源：http://xc.newstarts.cn

Go:   resp.StatusCode
来源：http://rp.shxzukj.cn

Ruby: resp.code.to_i
来源：http://ra.hnjuh.cn

C#:   (int)resp.StatusCode
来源：http://yd.chemitech.net.cn

[L08] 并发请求多个地址
来源：http://kn.nszjky.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rk.nszjky.cn

PHP:  curl_multi_init() 系列
来源：http://nx.colortex.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kz.nszjky.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lj.huixiangedu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ed.hahajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qa.huanxung.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sk.huixinmuqiang.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wb.huixiangedu.cn

================================================================================
来源：http://bg.yuntaijiaju.cn

M. 命令行 / 进程 / 环境
来源：http://oj.9csxet.cn

================================================================================
来源：http://nz.9csxet.cn

[M01] 读取命令行参数
来源：http://en.shxzukj.cn

Py:   sys.argv[1:]
来源：http://ue.jctech888.com.cn

PHP:  $argv;  $argc;
来源：http://th.chemitech.net.cn

JS:   process.argv.slice(2)
来源：http://rs.gzmigu.cn

TS:   process.argv.slice(2)
来源：http://tk.colortex.cn

Java: args 数组（main 方法参数）
来源：http://tx.gzmigu.cn

Go:   os.Args[1:]
来源：http://tk.colortex.cn

Ruby: ARGV
来源：http://rm.nicolike.cn

C#:   args 数组（Main 方法参数）
来源：http://ae.huixiangedu.cn

[M02] 读取环境变量
来源：http://wq.chemitech.net.cn

Py:   os.environ.get("HOME")
来源：http://yc.yuntaijiaju.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://oi.9csxet.cn

JS:   process.env.HOME
来源：http://ej.bookmarksfly.cn

TS:   process.env.HOME
来源：http://fc.asd995.cn

Java: System.getenv("HOME")
来源：http://ln.jctech888.com.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cu.jianghongdianzi.cn

Ruby: ENV["HOME"]
来源：http://jc.jianghongdianzi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wk.wgjwhj.cn

[M03] 执行外部命令
来源：http://yh.shtwfgs.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://sd.hnjuh.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zw.jctech888.com.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://yb.jctech888.com.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://of.gzmigu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mn.bjjhwx.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://rc.shxzskj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hb.9csxet.cn

C#:   Process.Start("ls", "-l");
来源：http://yi.yuntaijiaju.cn

[M04] 获取当前工作目录
来源：http://rl.chemitech.net.cn

Py:   os.getcwd()
来源：http://es.wgjwhj.cn

PHP:  getcwd();
来源：http://mg.shtwfgs.cn

JS:   process.cwd()
来源：http://uc.newstarts.cn

TS:   process.cwd()
来源：http://yd.nszjky.cn

Java: Path.of("").toAbsolutePath()
来源：http://ts.panjiajie.cn

Go:   os.Getwd()
来源：http://mr.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://xx.yuexingan06.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hr.yuexingan06.cn

[M05] 设置退出码
来源：http://ha.nszjky.cn

Py:   sys.exit(1)
来源：http://li.haigaiapp.cn

PHP:  exit(1);
来源：http://zl.shxzukj.cn

JS:   process.exit(1)
来源：http://jo.huixinmuqiang.cn

TS:   process.exit(1)
来源：http://sg.colortex.cn

Java: System.exit(1)
来源：http://ul.huanxung.cn

Go:   os.Exit(1)
来源：http://wo.haigaiapp.cn

Ruby: exit 1
来源：http://yn.colortex.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ti.bookmarksfly.cn

[M06] 向标准错误输出
来源：http://tb.shxzskj.cn

Py:   print("err", file=sys.stderr)
来源：http://tg.bjjhwx.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hn.colortex.cn

JS:   console.error("err")
来源：http://dr.lnxyls.cn

TS:   console.error("err")
来源：http://wx.9csxet.cn

Java: System.err.println("err")
来源：http://hk.gzmigu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zl.newstarts.cn

Ruby: warn "err"
来源：http://zu.newstarts.cn

C#:   Console.Error.WriteLine("err")
来源：http://pk.bjjhwx.cn

[M07] 判断是否为主入口
来源：http://in.wgjwhj.cn


<!-- 参考信息 -->