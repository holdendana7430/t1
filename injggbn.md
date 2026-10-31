代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bq.shxzukj.cn

JS:   new Date();  Date.now()
来源：http://qa.shxzukj.cn

TS:   new Date();  Date.now()
来源：http://kc.lnxyls.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://si.szxytkj.cn

Go:   time.Now()
来源：http://ql.gzmigu.cn

Ruby: Time.now
来源：http://zn.521024.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ca.wgjwhj.cn

[J02] 格式化输出
来源：http://xm.huixiangedu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://se.bjjhwx.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rn.gzmigu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hn.haigaiapp.cn

TS:   d.toISOString()
来源：http://pr.yuntaijiaju.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hn.colortex.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yg.nicolike.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xu.shtwfgs.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://se.huanxung.cn

[J03] 字符串解析为日期
来源：http://dk.jianghongdianzi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lc.szxytkj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://db.521024.cn

JS:   new Date("2024-01-02")
来源：http://qs.yuntaijiaju.cn

TS:   new Date("2024-01-02")
来源：http://vt.haigaiapp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jr.szxytkj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ud.gzmigu.cn

Ruby: Date.parse("2024-01-02")
来源：http://mm.wgjwhj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ab.hnjuh.cn

[J04] 时间戳与日期互转
来源：http://hq.yuexingan06.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mq.nicolike.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zr.bjjhwx.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xm.haigaiapp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ij.shxzukj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fm.asd995.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gm.chemitech.net.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://km.muxihuayi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://oi.yuexingan06.cn

[J05] 时间加减（加 7 天）
来源：http://md.yuexingan06.cn

Py:   now + timedelta(days=7)
来源：http://vb.shxzukj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vz.bookmarksfly.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yd.gzmigu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kv.shtwfgs.cn

Java: LocalDate.now().plusDays(7)
来源：http://tc.colortex.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tb.huanxung.cn

Ruby: Time.now + 7 * 86400
来源：http://nk.yuexingan06.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pr.wgjwhj.cn

[J06] 计算两时间之差
来源：http://hi.newstarts.cn

Py:   (end - start).total_seconds()
来源：http://bl.9csxet.cn

PHP:  $end->diff($start)->days;
来源：http://hh.asd995.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bw.bookmarksfly.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lb.haigaiapp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://cs.bjjhwx.cn

Go:   end.Sub(start).Hours()
来源：http://qc.wgjwhj.cn

Ruby: end - start                 # 返回秒数
来源：http://zy.9csxet.cn

C#:   (end - start).TotalSeconds
来源：http://xz.jctech888.com.cn

[J07] 比较两个日期
来源：http://nt.hahajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://fe.szsharing.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lj.chemitech.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://yx.szxytkj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rl.hnjuh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yz.lnxyls.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mq.jianghongdianzi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://yo.muxihuayi.cn

C#:   d1 < d2;  d1 == d2
来源：http://xx.huixinmuqiang.cn

[J08] 提取年月日与星期
来源：http://qe.yuntaijiaju.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lx.colortex.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qz.nszjky.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cg.shxzukj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ku.nicolike.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lf.szsharing.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sm.gzmigu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tm.521024.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yt.newstarts.cn

[J09] 时区处理
来源：http://if.lnxyls.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uw.nszjky.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xa.szxytkj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ss.9csxet.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kj.yuntaijiaju.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bl.9csxet.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fa.shxzskj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ek.wgjwhj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ah.newstarts.cn

[J10] 取今天 / 本月第一天
来源：http://ml.521024.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ea.lnxyls.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nf.huanxung.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zy.huanxung.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pz.bjjhwx.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mb.nszjky.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yb.jianghongdianzi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ya.gzmigu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sa.szxytkj.cn

================================================================================
来源：http://qu.hahajie.cn

K. JSON 与序列化
来源：http://zn.shtwfgs.cn

================================================================================
来源：http://ij.panjiajie.cn

[K01] 对象转 JSON 字符串
来源：http://ot.9csxet.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dp.lnxyls.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ow.nszjky.cn

JS:   JSON.stringify(obj)
来源：http://qs.shtwfgs.cn

TS:   JSON.stringify(obj)
来源：http://gx.bjjhwx.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kz.haigaiapp.cn

Go:   json.Marshal(obj)
来源：http://bx.newstarts.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ha.9csxet.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://eu.yuexingan06.cn

[K02] JSON 字符串转对象
来源：http://ae.chemitech.net.cn

Py:   json.loads(s)
来源：http://hm.lnxyls.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://va.szxytkj.cn

JS:   JSON.parse(s)
来源：http://pq.wgjwhj.cn

TS:   JSON.parse(s)
来源：http://jd.haigaiapp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hb.521024.cn

Go:   json.Unmarshal(data, &v)
来源：http://os.hahajie.cn

Ruby: JSON.parse(s)
来源：http://yw.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pd.bjjhwx.cn

[K03] JSON 美化输出（带缩进）
来源：http://ll.panjiajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ze.szsharing.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ki.huixinmuqiang.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qt.shxzskj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rp.huixiangedu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qf.9csxet.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vi.huixiangedu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ed.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jj.newstarts.cn

[K04] 读取 JSON 文件
来源：http://wn.nszjky.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://is.yuntaijiaju.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kc.jianghongdianzi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dk.huanxung.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ym.szxytkj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gq.szsharing.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gu.521024.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ou.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hy.muxihuayi.cn

[K05] 深拷贝对象
来源：http://qk.haigaiapp.cn

Py:   copy.deepcopy(obj)
来源：http://ce.wgjwhj.cn

PHP:  unserialize(serialize($obj));
来源：http://pc.asd995.cn

JS:   structuredClone(obj)
来源：http://vv.jianghongdianzi.cn

TS:   structuredClone(obj)
来源：http://bz.nszjky.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wt.yuexingan06.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://le.hnjuh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zx.shtwfgs.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ki.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://zx.colortex.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nu.colortex.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cb.nszjky.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qh.shxzukj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bp.shxzukj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pk.shxzskj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://tl.hahajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kn.newstarts.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fq.huixinmuqiang.cn

[K07] 进制转换
来源：http://bl.chemitech.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ri.colortex.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vd.nicolike.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cw.shtwfgs.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lt.huixinmuqiang.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kt.yuexingan06.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ee.bookmarksfly.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kv.szxytkj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zf.jianghongdianzi.cn

[K08] 二进制序列化（非 JSON）
来源：http://pf.hnjuh.cn

Py:   pickle.dumps(obj)
来源：http://mv.lnxyls.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ye.gzmigu.cn

JS:   v8.serialize(obj)        // Node
来源：http://on.wgjwhj.cn

TS:   v8.serialize(obj)        // Node
来源：http://sn.hahajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rl.chemitech.net.cn

Go:   encoding/gob
来源：http://xl.szxytkj.cn

Ruby: Marshal.dump(obj)
来源：http://ty.chemitech.net.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wg.huixinmuqiang.cn

================================================================================
来源：http://um.nszjky.cn

L. 网络请求
来源：http://wz.jianghongdianzi.cn

================================================================================
来源：http://xp.hahajie.cn

[L01] 发送 GET 请求
来源：http://hv.jctech888.com.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dg.yuntaijiaju.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qg.muxihuayi.cn

JS:   await fetch(url)
来源：http://ow.shxzskj.cn

TS:   await fetch(url)
来源：http://eu.bookmarksfly.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zb.jctech888.com.cn

Go:   resp, err := http.Get(url)
来源：http://dm.jctech888.com.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://lg.shxzukj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pv.hahajie.cn

[L02] 发送 POST JSON
来源：http://mp.chemitech.net.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gz.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zp.jctech888.com.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ar.lnxyls.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yg.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nl.asd995.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uj.jctech888.com.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lh.yuexingan06.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zd.newstarts.cn

[L03] 设置自定义请求头
来源：http://qt.colortex.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hv.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://oj.bookmarksfly.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ey.haigaiapp.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nn.asd995.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kc.huanxung.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zz.haigaiapp.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nf.9csxet.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lp.haigaiapp.cn

[L04] 设置超时
来源：http://np.jctech888.com.cn

Py:   requests.get(url, timeout=5)
来源：http://px.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kx.yuntaijiaju.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lb.huixinmuqiang.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oa.hnjuh.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ew.yuntaijiaju.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yt.szxytkj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kd.panjiajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tf.jctech888.com.cn

[L05] 上传文件（multipart）
来源：http://ko.muxihuayi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cc.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fd.szxytkj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://my.yuntaijiaju.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jc.chemitech.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://po.muxihuayi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kf.521024.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uc.jianghongdianzi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jh.szsharing.cn

[L06] 解析响应为 JSON
来源：http://hi.wgjwhj.cn

Py:   resp.json()
来源：http://rg.panjiajie.cn

PHP:  json_decode($body, true);
来源：http://ok.wgjwhj.cn

JS:   await resp.json()
来源：http://us.asd995.cn

TS:   await resp.json()
来源：http://ay.9csxet.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jw.nszjky.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bz.jctech888.com.cn

Ruby: JSON.parse(resp.body)
来源：http://yj.newstarts.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ua.chemitech.net.cn

[L07] 处理 HTTP 状态码
来源：http://rf.szsharing.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://es.jctech888.com.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ug.9csxet.cn

JS:   resp.ok;  resp.status
来源：http://xq.newstarts.cn

TS:   resp.ok;  resp.status
来源：http://hl.shtwfgs.cn

Java: resp.statusCode()
来源：http://fu.asd995.cn

Go:   resp.StatusCode
来源：http://rn.hnjuh.cn

Ruby: resp.code.to_i
来源：http://mc.huixiangedu.cn

C#:   (int)resp.StatusCode
来源：http://it.nszjky.cn

[L08] 并发请求多个地址
来源：http://ed.newstarts.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://og.bjjhwx.cn

PHP:  curl_multi_init() 系列
来源：http://et.9csxet.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lm.szxytkj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zv.yuntaijiaju.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zd.9csxet.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://iq.asd995.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lu.9csxet.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://su.huixiangedu.cn

================================================================================
来源：http://bo.newstarts.cn

M. 命令行 / 进程 / 环境
来源：http://fz.huixinmuqiang.cn

================================================================================
来源：http://cp.hnjuh.cn

[M01] 读取命令行参数
来源：http://bp.huixinmuqiang.cn

Py:   sys.argv[1:]
来源：http://wx.yuexingan06.cn

PHP:  $argv;  $argc;
来源：http://hq.9csxet.cn

JS:   process.argv.slice(2)
来源：http://gc.521024.cn

TS:   process.argv.slice(2)
来源：http://hn.szsharing.cn

Java: args 数组（main 方法参数）
来源：http://em.shtwfgs.cn

Go:   os.Args[1:]
来源：http://gv.bjjhwx.cn

Ruby: ARGV
来源：http://ov.huixiangedu.cn

C#:   args 数组（Main 方法参数）
来源：http://kc.hahajie.cn

[M02] 读取环境变量
来源：http://zj.shtwfgs.cn

Py:   os.environ.get("HOME")
来源：http://td.muxihuayi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zv.jianghongdianzi.cn

JS:   process.env.HOME
来源：http://hz.9csxet.cn

TS:   process.env.HOME
来源：http://af.shxzskj.cn

Java: System.getenv("HOME")
来源：http://qd.hahajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://do.chemitech.net.cn

Ruby: ENV["HOME"]
来源：http://zk.szsharing.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ur.wgjwhj.cn

[M03] 执行外部命令
来源：http://pd.9csxet.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ip.bookmarksfly.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ns.jianghongdianzi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ox.yuexingan06.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qp.hnjuh.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ry.yuexingan06.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://pl.bookmarksfly.cn

Ruby: system("ls -l");  `ls -l`
来源：http://sg.hahajie.cn

C#:   Process.Start("ls", "-l");
来源：http://nw.huixiangedu.cn

[M04] 获取当前工作目录
来源：http://bi.chemitech.net.cn

Py:   os.getcwd()
来源：http://px.huixiangedu.cn

PHP:  getcwd();
来源：http://vm.gzmigu.cn

JS:   process.cwd()
来源：http://kv.muxihuayi.cn

TS:   process.cwd()
来源：http://sl.asd995.cn

Java: Path.of("").toAbsolutePath()
来源：http://hk.bookmarksfly.cn

Go:   os.Getwd()
来源：http://hu.gzmigu.cn

Ruby: Dir.pwd
来源：http://xe.huanxung.cn

C#:   Directory.GetCurrentDirectory()
来源：http://bs.newstarts.cn

[M05] 设置退出码
来源：http://gi.hahajie.cn

Py:   sys.exit(1)
来源：http://bm.colortex.cn

PHP:  exit(1);
来源：http://jx.szsharing.cn

JS:   process.exit(1)
来源：http://pi.huanxung.cn

TS:   process.exit(1)
来源：http://oj.wgjwhj.cn

Java: System.exit(1)
来源：http://mt.gzmigu.cn

Go:   os.Exit(1)
来源：http://kd.huixiangedu.cn

Ruby: exit 1
来源：http://re.bookmarksfly.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lf.wgjwhj.cn

[M06] 向标准错误输出
来源：http://tn.jianghongdianzi.cn

Py:   print("err", file=sys.stderr)
来源：http://oy.chemitech.net.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://sc.yuexingan06.cn

JS:   console.error("err")
来源：http://fb.colortex.cn

TS:   console.error("err")
来源：http://ew.panjiajie.cn

Java: System.err.println("err")
来源：http://gv.jctech888.com.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qf.bjjhwx.cn

Ruby: warn "err"
来源：http://ip.bookmarksfly.cn

C#:   Console.Error.WriteLine("err")
来源：http://ng.yuntaijiaju.cn

[M07] 判断是否为主入口
来源：http://nx.wgjwhj.cn

Py:   if __name__ == "__main__":
来源：http://lb.521024.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mf.haigaiapp.cn

JS:   require.main === module
来源：http://vs.521024.cn

TS:   require.main === module
来源：http://ch.panjiajie.cn


<!-- 参考信息 -->