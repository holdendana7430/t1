代发 wailian999

J. 日期与时间
来源：http://hs.yuexingan06.cn

================================================================================
来源：http://ft.asd995.cn

[J01] 获取当前时间
来源：http://ts.szxytkj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kf.colortex.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dn.huixinmuqiang.cn

JS:   new Date();  Date.now()
来源：http://rm.newstarts.cn

TS:   new Date();  Date.now()
来源：http://fr.wgjwhj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yb.gzmigu.cn

Go:   time.Now()
来源：http://rv.yuexingan06.cn

Ruby: Time.now
来源：http://mh.huixiangedu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sa.shxzukj.cn

[J02] 格式化输出
来源：http://ph.yuntaijiaju.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ep.szxytkj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sg.bjjhwx.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zk.haigaiapp.cn

TS:   d.toISOString()
来源：http://ha.szsharing.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nz.yuexingan06.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cr.bjjhwx.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pi.huanxung.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gh.hnjuh.cn

[J03] 字符串解析为日期
来源：http://ev.shxzskj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://in.nicolike.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ar.haigaiapp.cn

JS:   new Date("2024-01-02")
来源：http://bv.szsharing.cn

TS:   new Date("2024-01-02")
来源：http://ow.wgjwhj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://al.gzmigu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vd.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://fn.9csxet.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ky.asd995.cn

[J04] 时间戳与日期互转
来源：http://oc.newstarts.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zz.muxihuayi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ez.huixiangedu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dm.nszjky.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jz.gzmigu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uj.muxihuayi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xl.bjjhwx.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nn.jctech888.com.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jk.lnxyls.cn

[J05] 时间加减（加 7 天）
来源：http://zc.hnjuh.cn

Py:   now + timedelta(days=7)
来源：http://ke.yuntaijiaju.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://py.panjiajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gj.huixinmuqiang.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dl.muxihuayi.cn

Java: LocalDate.now().plusDays(7)
来源：http://qb.nszjky.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://re.jctech888.com.cn

Ruby: Time.now + 7 * 86400
来源：http://ag.bookmarksfly.cn

C#:   DateTime.Now.AddDays(7)
来源：http://mu.panjiajie.cn

[J06] 计算两时间之差
来源：http://eu.panjiajie.cn

Py:   (end - start).total_seconds()
来源：http://va.muxihuayi.cn

PHP:  $end->diff($start)->days;
来源：http://lw.colortex.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tg.colortex.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xw.szxytkj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://el.hnjuh.cn

Go:   end.Sub(start).Hours()
来源：http://iv.9csxet.cn

Ruby: end - start                 # 返回秒数
来源：http://qr.jctech888.com.cn

C#:   (end - start).TotalSeconds
来源：http://fa.9csxet.cn

[J07] 比较两个日期
来源：http://yf.shxzukj.cn

Py:   d1 < d2;  d1 == d2
来源：http://ir.newstarts.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hh.yuntaijiaju.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mg.huixiangedu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xg.newstarts.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://al.bookmarksfly.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uj.nszjky.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qg.bjjhwx.cn

C#:   d1 < d2;  d1 == d2
来源：http://kr.shxzskj.cn

[J08] 提取年月日与星期
来源：http://ki.wgjwhj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qh.bookmarksfly.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://th.muxihuayi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://eo.wgjwhj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vd.shxzukj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ed.nicolike.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zf.yuexingan06.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pl.jctech888.com.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xr.nicolike.cn

[J09] 时区处理
来源：http://kk.wgjwhj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sx.jctech888.com.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cy.bjjhwx.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://up.haigaiapp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ab.shtwfgs.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jo.nicolike.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pn.huanxung.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ox.huixiangedu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lz.jianghongdianzi.cn

[J10] 取今天 / 本月第一天
来源：http://vw.bjjhwx.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ey.shxzskj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://el.huixinmuqiang.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ih.szsharing.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mm.wgjwhj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yl.newstarts.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lu.colortex.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cz.yuexingan06.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bs.lnxyls.cn

================================================================================
来源：http://ko.huanxung.cn

K. JSON 与序列化
来源：http://nc.nicolike.cn

================================================================================
来源：http://mg.521024.cn

[K01] 对象转 JSON 字符串
来源：http://ls.shtwfgs.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://id.huanxung.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ky.huanxung.cn

JS:   JSON.stringify(obj)
来源：http://wg.nszjky.cn

TS:   JSON.stringify(obj)
来源：http://ua.panjiajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://oa.bookmarksfly.cn

Go:   json.Marshal(obj)
来源：http://be.bookmarksfly.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xc.nicolike.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jb.huixinmuqiang.cn

[K02] JSON 字符串转对象
来源：http://kv.shxzukj.cn

Py:   json.loads(s)
来源：http://jm.yuntaijiaju.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pw.haigaiapp.cn

JS:   JSON.parse(s)
来源：http://qd.panjiajie.cn

TS:   JSON.parse(s)
来源：http://rr.huixiangedu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ta.hnjuh.cn

Go:   json.Unmarshal(data, &v)
来源：http://aq.szxytkj.cn

Ruby: JSON.parse(s)
来源：http://lt.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uc.jianghongdianzi.cn

[K03] JSON 美化输出（带缩进）
来源：http://jl.yuexingan06.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ly.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tq.szsharing.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ix.shxzukj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rd.haigaiapp.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fn.szsharing.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ri.huixinmuqiang.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xa.hnjuh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wz.szxytkj.cn

[K04] 读取 JSON 文件
来源：http://bh.muxihuayi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jk.huixinmuqiang.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pp.bjjhwx.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ri.jianghongdianzi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fa.9csxet.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ot.shxzskj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ny.hnjuh.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://nu.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lb.hahajie.cn

[K05] 深拷贝对象
来源：http://do.hnjuh.cn

Py:   copy.deepcopy(obj)
来源：http://yx.hnjuh.cn

PHP:  unserialize(serialize($obj));
来源：http://ru.yuntaijiaju.cn

JS:   structuredClone(obj)
来源：http://wi.huanxung.cn

TS:   structuredClone(obj)
来源：http://pe.shtwfgs.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ww.nszjky.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cx.wgjwhj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jo.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hq.huanxung.cn

[K06] 解析 URL 查询串
来源：http://qm.szxytkj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zi.huanxung.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ha.huixiangedu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sr.nicolike.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cm.szxytkj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://av.szsharing.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fs.shxzukj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://si.521024.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nd.shxzskj.cn

[K07] 进制转换
来源：http://am.jctech888.com.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ks.nicolike.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nr.yuntaijiaju.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zv.nszjky.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ly.szxytkj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wj.bjjhwx.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zo.shxzukj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lm.lnxyls.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://os.haigaiapp.cn

[K08] 二进制序列化（非 JSON）
来源：http://pf.wgjwhj.cn

Py:   pickle.dumps(obj)
来源：http://lv.szxytkj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://je.huixinmuqiang.cn

JS:   v8.serialize(obj)        // Node
来源：http://ec.gzmigu.cn

TS:   v8.serialize(obj)        // Node
来源：http://ge.bookmarksfly.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kz.yuexingan06.cn

Go:   encoding/gob
来源：http://xl.nszjky.cn

Ruby: Marshal.dump(obj)
来源：http://gg.shtwfgs.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hi.shxzukj.cn

================================================================================
来源：http://ch.hnjuh.cn

L. 网络请求
来源：http://an.gzmigu.cn

================================================================================
来源：http://jj.panjiajie.cn

[L01] 发送 GET 请求
来源：http://lj.521024.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://he.huanxung.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jx.newstarts.cn

JS:   await fetch(url)
来源：http://pa.muxihuayi.cn

TS:   await fetch(url)
来源：http://mc.newstarts.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ug.shxzskj.cn

Go:   resp, err := http.Get(url)
来源：http://ii.hnjuh.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rm.szsharing.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dt.gzmigu.cn

[L02] 发送 POST JSON
来源：http://nu.wgjwhj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://db.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ek.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gh.bookmarksfly.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cg.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lz.9csxet.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sl.bjjhwx.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qg.szsharing.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://td.asd995.cn

[L03] 设置自定义请求头
来源：http://ke.gzmigu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ye.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ru.jianghongdianzi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hk.shxzukj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xr.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uz.yuntaijiaju.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vq.szxytkj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lt.hahajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://di.bookmarksfly.cn

[L04] 设置超时
来源：http://yu.huixinmuqiang.cn

Py:   requests.get(url, timeout=5)
来源：http://bq.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vk.panjiajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wz.szsharing.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dq.lnxyls.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yc.chemitech.net.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sa.nicolike.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ml.asd995.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ak.szxytkj.cn

[L05] 上传文件（multipart）
来源：http://br.asd995.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://oh.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jw.bookmarksfly.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wd.yuexingan06.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jj.shtwfgs.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://oi.haigaiapp.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lj.gzmigu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wx.muxihuayi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ek.shtwfgs.cn

[L06] 解析响应为 JSON
来源：http://qo.huanxung.cn

Py:   resp.json()
来源：http://td.521024.cn

PHP:  json_decode($body, true);
来源：http://yq.hahajie.cn

JS:   await resp.json()
来源：http://ug.haigaiapp.cn

TS:   await resp.json()
来源：http://qe.9csxet.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hs.chemitech.net.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gx.gzmigu.cn

Ruby: JSON.parse(resp.body)
来源：http://te.521024.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bs.bjjhwx.cn

[L07] 处理 HTTP 状态码
来源：http://zf.chemitech.net.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xq.huanxung.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pm.shxzskj.cn

JS:   resp.ok;  resp.status
来源：http://ri.asd995.cn

TS:   resp.ok;  resp.status
来源：http://rp.nicolike.cn

Java: resp.statusCode()
来源：http://mv.bjjhwx.cn

Go:   resp.StatusCode
来源：http://rp.shxzukj.cn

Ruby: resp.code.to_i
来源：http://if.9csxet.cn

C#:   (int)resp.StatusCode
来源：http://fa.gzmigu.cn

[L08] 并发请求多个地址
来源：http://ea.huixinmuqiang.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fg.haigaiapp.cn

PHP:  curl_multi_init() 系列
来源：http://vg.9csxet.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pv.gzmigu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yl.chemitech.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ys.gzmigu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ed.gzmigu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yj.panjiajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ly.asd995.cn

================================================================================
来源：http://br.yuntaijiaju.cn

M. 命令行 / 进程 / 环境
来源：http://ym.bjjhwx.cn

================================================================================
来源：http://wj.panjiajie.cn

[M01] 读取命令行参数
来源：http://hy.yuexingan06.cn

Py:   sys.argv[1:]
来源：http://am.asd995.cn

PHP:  $argv;  $argc;
来源：http://qz.bjjhwx.cn

JS:   process.argv.slice(2)
来源：http://fg.huixinmuqiang.cn

TS:   process.argv.slice(2)
来源：http://dx.yuexingan06.cn

Java: args 数组（main 方法参数）
来源：http://rt.shxzukj.cn

Go:   os.Args[1:]
来源：http://wu.panjiajie.cn

Ruby: ARGV
来源：http://zm.szxytkj.cn

C#:   args 数组（Main 方法参数）
来源：http://hg.huixinmuqiang.cn

[M02] 读取环境变量
来源：http://ux.521024.cn

Py:   os.environ.get("HOME")
来源：http://mc.bjjhwx.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zq.chemitech.net.cn

JS:   process.env.HOME
来源：http://qn.shxzukj.cn

TS:   process.env.HOME
来源：http://gg.hnjuh.cn

Java: System.getenv("HOME")
来源：http://bt.gzmigu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ga.yuexingan06.cn

Ruby: ENV["HOME"]
来源：http://ew.lnxyls.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://no.chemitech.net.cn

[M03] 执行外部命令
来源：http://do.shxzskj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gq.shxzskj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qf.nszjky.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ee.bjjhwx.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mm.huanxung.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xn.haigaiapp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://re.nicolike.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kg.haigaiapp.cn

C#:   Process.Start("ls", "-l");
来源：http://tz.shxzukj.cn

[M04] 获取当前工作目录
来源：http://mm.nszjky.cn

Py:   os.getcwd()
来源：http://zq.huanxung.cn

PHP:  getcwd();
来源：http://gq.jctech888.com.cn

JS:   process.cwd()
来源：http://uo.lnxyls.cn

TS:   process.cwd()
来源：http://xy.shxzskj.cn

Java: Path.of("").toAbsolutePath()
来源：http://lk.huanxung.cn

Go:   os.Getwd()
来源：http://ej.yuntaijiaju.cn

Ruby: Dir.pwd
来源：http://ju.lnxyls.cn

C#:   Directory.GetCurrentDirectory()
来源：http://va.lnxyls.cn

[M05] 设置退出码
来源：http://yp.szxytkj.cn

Py:   sys.exit(1)
来源：http://yc.huixinmuqiang.cn

PHP:  exit(1);
来源：http://zy.lnxyls.cn

JS:   process.exit(1)
来源：http://rg.9csxet.cn

TS:   process.exit(1)
来源：http://fe.nicolike.cn

Java: System.exit(1)
来源：http://xe.jianghongdianzi.cn

Go:   os.Exit(1)
来源：http://jd.nicolike.cn

Ruby: exit 1
来源：http://vz.lnxyls.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ip.shxzskj.cn

[M06] 向标准错误输出
来源：http://bk.521024.cn

Py:   print("err", file=sys.stderr)
来源：http://hw.bjjhwx.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ks.gzmigu.cn

JS:   console.error("err")
来源：http://yp.9csxet.cn

TS:   console.error("err")
来源：http://zj.huixinmuqiang.cn

Java: System.err.println("err")
来源：http://id.wgjwhj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ge.shxzukj.cn

Ruby: warn "err"
来源：http://cl.bjjhwx.cn

C#:   Console.Error.WriteLine("err")
来源：http://hx.huixinmuqiang.cn

[M07] 判断是否为主入口
来源：http://ch.shxzukj.cn


<!-- 参考信息 -->