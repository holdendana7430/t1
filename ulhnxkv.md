代发 wailian999

J. 日期与时间
来源：http://ja.jianghongdianzi.cn

================================================================================
来源：http://yh.huixiangedu.cn

[J01] 获取当前时间
来源：http://bd.9csxet.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rc.gzmigu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://in.hnjuh.cn

JS:   new Date();  Date.now()
来源：http://mi.shtwfgs.cn

TS:   new Date();  Date.now()
来源：http://dx.yuntaijiaju.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vn.hnjuh.cn

Go:   time.Now()
来源：http://fj.yuexingan06.cn

Ruby: Time.now
来源：http://vy.9csxet.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rp.yuntaijiaju.cn

[J02] 格式化输出
来源：http://yi.jctech888.com.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mu.jianghongdianzi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jh.huixinmuqiang.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rv.521024.cn

TS:   d.toISOString()
来源：http://eu.hnjuh.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jr.bjjhwx.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://no.wgjwhj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yn.colortex.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vv.wgjwhj.cn

[J03] 字符串解析为日期
来源：http://yb.huixinmuqiang.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gt.shxzukj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ae.huixinmuqiang.cn

JS:   new Date("2024-01-02")
来源：http://zv.huixiangedu.cn

TS:   new Date("2024-01-02")
来源：http://wy.nszjky.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qd.hahajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sy.chemitech.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://ch.shxzskj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fs.wgjwhj.cn

[J04] 时间戳与日期互转
来源：http://sg.huixiangedu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jq.lnxyls.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://oh.wgjwhj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://md.shxzskj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bn.9csxet.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://oh.bookmarksfly.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cs.szxytkj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cg.hnjuh.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fi.nicolike.cn

[J05] 时间加减（加 7 天）
来源：http://mz.521024.cn

Py:   now + timedelta(days=7)
来源：http://me.shxzukj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://gv.bookmarksfly.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ox.shxzukj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tv.yuntaijiaju.cn

Java: LocalDate.now().plusDays(7)
来源：http://fj.haigaiapp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fn.shxzskj.cn

Ruby: Time.now + 7 * 86400
来源：http://na.521024.cn

C#:   DateTime.Now.AddDays(7)
来源：http://fd.jianghongdianzi.cn

[J06] 计算两时间之差
来源：http://kw.huixinmuqiang.cn

Py:   (end - start).total_seconds()
来源：http://wk.huanxung.cn

PHP:  $end->diff($start)->days;
来源：http://bk.haigaiapp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zk.bookmarksfly.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ts.newstarts.cn

Java: Duration.between(start, end).toSeconds()
来源：http://yg.newstarts.cn

Go:   end.Sub(start).Hours()
来源：http://cu.9csxet.cn

Ruby: end - start                 # 返回秒数
来源：http://fw.szsharing.cn

C#:   (end - start).TotalSeconds
来源：http://gq.huanxung.cn

[J07] 比较两个日期
来源：http://sh.hnjuh.cn

Py:   d1 < d2;  d1 == d2
来源：http://lw.bjjhwx.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://na.szxytkj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://im.bookmarksfly.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ke.shxzskj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mr.hahajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zc.huixiangedu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://au.nicolike.cn

C#:   d1 < d2;  d1 == d2
来源：http://il.szxytkj.cn

[J08] 提取年月日与星期
来源：http://qt.colortex.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://th.bookmarksfly.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jj.bjjhwx.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pq.jctech888.com.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wm.9csxet.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ag.bjjhwx.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fp.hnjuh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xs.shxzskj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zn.shxzskj.cn

[J09] 时区处理
来源：http://mw.521024.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://du.wgjwhj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://df.gzmigu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cq.panjiajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bj.nicolike.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://uu.haigaiapp.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ld.shxzskj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qf.jianghongdianzi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://li.yuexingan06.cn

[J10] 取今天 / 本月第一天
来源：http://su.muxihuayi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ht.wgjwhj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://iu.huanxung.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jw.haigaiapp.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hw.newstarts.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://du.colortex.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://me.lnxyls.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tp.jianghongdianzi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://is.huixiangedu.cn

================================================================================
来源：http://sn.szxytkj.cn

K. JSON 与序列化
来源：http://gl.bjjhwx.cn

================================================================================
来源：http://hg.panjiajie.cn

[K01] 对象转 JSON 字符串
来源：http://ln.muxihuayi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cx.nszjky.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gi.hnjuh.cn

JS:   JSON.stringify(obj)
来源：http://tn.lnxyls.cn

TS:   JSON.stringify(obj)
来源：http://zl.wgjwhj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hg.nicolike.cn

Go:   json.Marshal(obj)
来源：http://hl.huixinmuqiang.cn

Ruby: obj.to_json                                     // require "json"
来源：http://kx.panjiajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://kf.jianghongdianzi.cn

[K02] JSON 字符串转对象
来源：http://oc.huixinmuqiang.cn

Py:   json.loads(s)
来源：http://rw.shxzukj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wa.panjiajie.cn

JS:   JSON.parse(s)
来源：http://pj.huanxung.cn

TS:   JSON.parse(s)
来源：http://zc.lnxyls.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ne.yuexingan06.cn

Go:   json.Unmarshal(data, &v)
来源：http://pn.shtwfgs.cn

Ruby: JSON.parse(s)
来源：http://sc.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cj.jianghongdianzi.cn

[K03] JSON 美化输出（带缩进）
来源：http://dd.yuexingan06.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dw.panjiajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mv.hnjuh.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jn.jctech888.com.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sq.asd995.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vi.chemitech.net.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oo.szsharing.cn

Ruby: JSON.pretty_generate(obj)
来源：http://sc.szsharing.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ti.nszjky.cn

[K04] 读取 JSON 文件
来源：http://kt.jctech888.com.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cw.jianghongdianzi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hf.muxihuayi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kt.521024.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gz.newstarts.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ks.shxzskj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ew.hnjuh.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ja.hnjuh.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hf.9csxet.cn

[K05] 深拷贝对象
来源：http://ca.shtwfgs.cn

Py:   copy.deepcopy(obj)
来源：http://ac.yuexingan06.cn

PHP:  unserialize(serialize($obj));
来源：http://zm.newstarts.cn

JS:   structuredClone(obj)
来源：http://zw.huixinmuqiang.cn

TS:   structuredClone(obj)
来源：http://cv.huixiangedu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://af.bookmarksfly.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dr.colortex.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kx.gzmigu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ew.hahajie.cn

[K06] 解析 URL 查询串
来源：http://gs.nicolike.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://eu.yuntaijiaju.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zm.muxihuayi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qd.bookmarksfly.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hf.hnjuh.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ch.panjiajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zm.jctech888.com.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dl.panjiajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hk.bjjhwx.cn

[K07] 进制转换
来源：http://ab.yuntaijiaju.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qo.yuntaijiaju.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gl.jctech888.com.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fl.huixinmuqiang.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://in.nszjky.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uj.shxzukj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lp.yuexingan06.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jf.panjiajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://am.szxytkj.cn

[K08] 二进制序列化（非 JSON）
来源：http://nz.huixinmuqiang.cn

Py:   pickle.dumps(obj)
来源：http://bg.nicolike.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cw.chemitech.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://sv.bjjhwx.cn

TS:   v8.serialize(obj)        // Node
来源：http://dm.huixinmuqiang.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://eq.9csxet.cn

Go:   encoding/gob
来源：http://oq.bjjhwx.cn

Ruby: Marshal.dump(obj)
来源：http://fc.muxihuayi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://md.nicolike.cn

================================================================================
来源：http://aj.wgjwhj.cn

L. 网络请求
来源：http://ml.shxzukj.cn

================================================================================
来源：http://oe.hnjuh.cn

[L01] 发送 GET 请求
来源：http://ov.bjjhwx.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zs.hahajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dz.yuexingan06.cn

JS:   await fetch(url)
来源：http://mu.huanxung.cn

TS:   await fetch(url)
来源：http://cn.jianghongdianzi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yk.521024.cn

Go:   resp, err := http.Get(url)
来源：http://ty.bookmarksfly.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://au.521024.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mv.muxihuayi.cn

[L02] 发送 POST JSON
来源：http://ja.panjiajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fn.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kn.yuntaijiaju.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gm.newstarts.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nl.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kq.colortex.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rf.huixiangedu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pf.jctech888.com.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ws.521024.cn

[L03] 设置自定义请求头
来源：http://js.gzmigu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yk.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cl.newstarts.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jo.nszjky.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fo.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tj.jianghongdianzi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yq.szsharing.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jm.jianghongdianzi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hq.jianghongdianzi.cn

[L04] 设置超时
来源：http://ay.9csxet.cn

Py:   requests.get(url, timeout=5)
来源：http://cw.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zc.szxytkj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rc.shxzskj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nv.muxihuayi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rp.muxihuayi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hb.panjiajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gj.hahajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ua.haigaiapp.cn

[L05] 上传文件（multipart）
来源：http://ni.colortex.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mb.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zq.yuexingan06.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kc.bookmarksfly.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vm.huanxung.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gx.bookmarksfly.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://re.haigaiapp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ro.huixinmuqiang.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hy.shtwfgs.cn

[L06] 解析响应为 JSON
来源：http://iz.nicolike.cn

Py:   resp.json()
来源：http://aq.huixiangedu.cn

PHP:  json_decode($body, true);
来源：http://zc.jctech888.com.cn

JS:   await resp.json()
来源：http://zu.yuntaijiaju.cn

TS:   await resp.json()
来源：http://oi.huixinmuqiang.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gl.huixinmuqiang.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://la.bookmarksfly.cn

Ruby: JSON.parse(resp.body)
来源：http://ot.gzmigu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ph.huanxung.cn

[L07] 处理 HTTP 状态码
来源：http://hb.chemitech.net.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://he.muxihuayi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hm.muxihuayi.cn

JS:   resp.ok;  resp.status
来源：http://cx.bjjhwx.cn

TS:   resp.ok;  resp.status
来源：http://vx.wgjwhj.cn

Java: resp.statusCode()
来源：http://mm.muxihuayi.cn

Go:   resp.StatusCode
来源：http://kx.yuntaijiaju.cn

Ruby: resp.code.to_i
来源：http://fk.9csxet.cn

C#:   (int)resp.StatusCode
来源：http://ri.wgjwhj.cn

[L08] 并发请求多个地址
来源：http://yh.asd995.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lv.gzmigu.cn

PHP:  curl_multi_init() 系列
来源：http://qu.nicolike.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://of.szsharing.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ss.jianghongdianzi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ml.bookmarksfly.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qd.szxytkj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dd.bookmarksfly.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mf.panjiajie.cn

================================================================================
来源：http://rw.nszjky.cn

M. 命令行 / 进程 / 环境
来源：http://fh.nszjky.cn

================================================================================
来源：http://tq.wgjwhj.cn

[M01] 读取命令行参数
来源：http://fd.panjiajie.cn

Py:   sys.argv[1:]
来源：http://ef.newstarts.cn

PHP:  $argv;  $argc;
来源：http://fo.huixinmuqiang.cn

JS:   process.argv.slice(2)
来源：http://st.yuntaijiaju.cn

TS:   process.argv.slice(2)
来源：http://rv.shtwfgs.cn

Java: args 数组（main 方法参数）
来源：http://as.gzmigu.cn

Go:   os.Args[1:]
来源：http://hp.newstarts.cn

Ruby: ARGV
来源：http://ar.yuntaijiaju.cn

C#:   args 数组（Main 方法参数）
来源：http://fl.jctech888.com.cn

[M02] 读取环境变量
来源：http://dd.szxytkj.cn

Py:   os.environ.get("HOME")
来源：http://we.chemitech.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bu.gzmigu.cn

JS:   process.env.HOME
来源：http://tx.jctech888.com.cn

TS:   process.env.HOME
来源：http://zn.shtwfgs.cn

Java: System.getenv("HOME")
来源：http://qa.szxytkj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://od.muxihuayi.cn

Ruby: ENV["HOME"]
来源：http://ag.shxzskj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://st.lnxyls.cn

[M03] 执行外部命令
来源：http://aq.bookmarksfly.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mz.lnxyls.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dj.nszjky.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://og.huixiangedu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ei.gzmigu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ja.jianghongdianzi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lj.shxzukj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rs.haigaiapp.cn

C#:   Process.Start("ls", "-l");
来源：http://th.muxihuayi.cn

[M04] 获取当前工作目录
来源：http://an.shtwfgs.cn

Py:   os.getcwd()
来源：http://vd.nicolike.cn

PHP:  getcwd();
来源：http://le.gzmigu.cn

JS:   process.cwd()
来源：http://ay.gzmigu.cn

TS:   process.cwd()
来源：http://is.nicolike.cn

Java: Path.of("").toAbsolutePath()
来源：http://te.bjjhwx.cn

Go:   os.Getwd()
来源：http://gv.gzmigu.cn

Ruby: Dir.pwd
来源：http://zz.szxytkj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hnjuh.cn

[M05] 设置退出码
来源：http://ps.jctech888.com.cn

Py:   sys.exit(1)
来源：http://cx.wgjwhj.cn

PHP:  exit(1);
来源：http://qk.szxytkj.cn

JS:   process.exit(1)
来源：http://yu.hahajie.cn

TS:   process.exit(1)
来源：http://ij.shxzukj.cn

Java: System.exit(1)
来源：http://ww.szxytkj.cn

Go:   os.Exit(1)
来源：http://kk.shxzukj.cn

Ruby: exit 1
来源：http://ly.newstarts.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://br.yuntaijiaju.cn

[M06] 向标准错误输出
来源：http://uw.bookmarksfly.cn

Py:   print("err", file=sys.stderr)
来源：http://te.yuntaijiaju.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ca.muxihuayi.cn

JS:   console.error("err")
来源：http://zr.colortex.cn

TS:   console.error("err")
来源：http://gw.yuexingan06.cn

Java: System.err.println("err")
来源：http://vk.shtwfgs.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bm.chemitech.net.cn

Ruby: warn "err"
来源：http://nu.muxihuayi.cn

C#:   Console.Error.WriteLine("err")
来源：http://vs.szxytkj.cn

[M07] 判断是否为主入口
来源：http://ru.hnjuh.cn


<!-- 参考信息 -->