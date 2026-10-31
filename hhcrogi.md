代发 wailian999

J. 日期与时间
来源：http://io.szxytkj.cn

================================================================================
来源：http://xx.haigaiapp.cn

[J01] 获取当前时间
来源：http://kz.szsharing.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lr.bookmarksfly.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ck.shxzskj.cn

JS:   new Date();  Date.now()
来源：http://ro.shxzukj.cn

TS:   new Date();  Date.now()
来源：http://pm.shxzskj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://sx.huixinmuqiang.cn

Go:   time.Now()
来源：http://sx.hahajie.cn

Ruby: Time.now
来源：http://xc.bookmarksfly.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xb.lnxyls.cn

[J02] 格式化输出
来源：http://dc.jctech888.com.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fv.bjjhwx.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bp.muxihuayi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hd.nszjky.cn

TS:   d.toISOString()
来源：http://bh.colortex.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dh.haigaiapp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xh.panjiajie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tc.gzmigu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ea.huixiangedu.cn

[J03] 字符串解析为日期
来源：http://mz.gzmigu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mj.wgjwhj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://na.jianghongdianzi.cn

JS:   new Date("2024-01-02")
来源：http://br.wgjwhj.cn

TS:   new Date("2024-01-02")
来源：http://lt.jctech888.com.cn

Java: LocalDate.parse("2024-01-02")
来源：http://lq.nicolike.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kh.nicolike.cn

Ruby: Date.parse("2024-01-02")
来源：http://jh.hahajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pm.nicolike.cn

[J04] 时间戳与日期互转
来源：http://ed.9csxet.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yy.9csxet.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zc.bjjhwx.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kv.shxzskj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://yu.nszjky.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://az.muxihuayi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rn.asd995.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ed.chemitech.net.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cw.nicolike.cn

[J05] 时间加减（加 7 天）
来源：http://ka.shxzukj.cn

Py:   now + timedelta(days=7)
来源：http://wi.jctech888.com.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kj.yuntaijiaju.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ef.colortex.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xh.shxzukj.cn

Java: LocalDate.now().plusDays(7)
来源：http://th.nszjky.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://oa.shtwfgs.cn

Ruby: Time.now + 7 * 86400
来源：http://vm.shtwfgs.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xq.hahajie.cn

[J06] 计算两时间之差
来源：http://zj.9csxet.cn

Py:   (end - start).total_seconds()
来源：http://zn.szxytkj.cn

PHP:  $end->diff($start)->days;
来源：http://ht.hnjuh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://di.yuexingan06.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sh.9csxet.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ns.hnjuh.cn

Go:   end.Sub(start).Hours()
来源：http://zz.nicolike.cn

Ruby: end - start                 # 返回秒数
来源：http://hw.muxihuayi.cn

C#:   (end - start).TotalSeconds
来源：http://ig.huixiangedu.cn

[J07] 比较两个日期
来源：http://ok.szxytkj.cn

Py:   d1 < d2;  d1 == d2
来源：http://jk.521024.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ky.shxzskj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ft.shxzskj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://kn.bookmarksfly.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qb.haigaiapp.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gt.newstarts.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ih.huixiangedu.cn

C#:   d1 < d2;  d1 == d2
来源：http://sr.panjiajie.cn

[J08] 提取年月日与星期
来源：http://dt.shtwfgs.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lg.yuntaijiaju.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rh.nicolike.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yd.jctech888.com.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dm.lnxyls.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jy.yuexingan06.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ad.colortex.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ub.haigaiapp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kj.szsharing.cn

[J09] 时区处理
来源：http://yh.szsharing.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ou.newstarts.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tj.yuexingan06.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://py.9csxet.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rh.hahajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gd.wgjwhj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://or.hahajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tz.nszjky.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jk.panjiajie.cn

[J10] 取今天 / 本月第一天
来源：http://xk.bookmarksfly.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tb.hahajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nu.nszjky.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yi.shxzskj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dm.nicolike.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uw.shxzukj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vw.hnjuh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bf.hahajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ln.gzmigu.cn

================================================================================
来源：http://ou.wgjwhj.cn

K. JSON 与序列化
来源：http://lj.szsharing.cn

================================================================================
来源：http://xu.huixinmuqiang.cn

[K01] 对象转 JSON 字符串
来源：http://vw.szxytkj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://st.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lj.9csxet.cn

JS:   JSON.stringify(obj)
来源：http://fk.521024.cn

TS:   JSON.stringify(obj)
来源：http://yd.huanxung.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qh.asd995.cn

Go:   json.Marshal(obj)
来源：http://jo.9csxet.cn

Ruby: obj.to_json                                     // require "json"
来源：http://yl.shxzskj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ej.nszjky.cn

[K02] JSON 字符串转对象
来源：http://nk.bjjhwx.cn

Py:   json.loads(s)
来源：http://rk.jctech888.com.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ux.yuexingan06.cn

JS:   JSON.parse(s)
来源：http://xe.bookmarksfly.cn

TS:   JSON.parse(s)
来源：http://ig.asd995.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zb.szxytkj.cn

Go:   json.Unmarshal(data, &v)
来源：http://jd.jctech888.com.cn

Ruby: JSON.parse(s)
来源：http://wi.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://my.nicolike.cn

[K03] JSON 美化输出（带缩进）
来源：http://qd.huanxung.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ce.szxytkj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://in.huixinmuqiang.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pe.yuexingan06.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xu.hnjuh.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yk.hahajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hg.hnjuh.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ab.szsharing.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://iw.chemitech.net.cn

[K04] 读取 JSON 文件
来源：http://lh.bjjhwx.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://we.shxzskj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tv.hahajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lt.521024.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sr.huixiangedu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gj.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vi.shxzukj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ai.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xr.shtwfgs.cn

[K05] 深拷贝对象
来源：http://pt.yuntaijiaju.cn

Py:   copy.deepcopy(obj)
来源：http://vi.shxzskj.cn

PHP:  unserialize(serialize($obj));
来源：http://cr.yuexingan06.cn

JS:   structuredClone(obj)
来源：http://aj.shtwfgs.cn

TS:   structuredClone(obj)
来源：http://vw.521024.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zy.nszjky.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fy.bjjhwx.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yl.szsharing.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yk.szsharing.cn

[K06] 解析 URL 查询串
来源：http://mk.gzmigu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ru.muxihuayi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sy.haigaiapp.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dx.jctech888.com.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sg.shxzukj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ah.newstarts.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://in.panjiajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dv.yuexingan06.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kp.bookmarksfly.cn

[K07] 进制转换
来源：http://cj.szsharing.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qb.gzmigu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hb.nszjky.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xx.huanxung.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xy.nszjky.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fc.lnxyls.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kn.wgjwhj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://et.gzmigu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://na.muxihuayi.cn

[K08] 二进制序列化（非 JSON）
来源：http://ti.huixiangedu.cn

Py:   pickle.dumps(obj)
来源：http://qd.yuexingan06.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://it.hnjuh.cn

JS:   v8.serialize(obj)        // Node
来源：http://oa.521024.cn

TS:   v8.serialize(obj)        // Node
来源：http://xm.szsharing.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qb.hahajie.cn

Go:   encoding/gob
来源：http://cp.panjiajie.cn

Ruby: Marshal.dump(obj)
来源：http://ep.hahajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wm.asd995.cn

================================================================================
来源：http://fp.shxzukj.cn

L. 网络请求
来源：http://um.huixinmuqiang.cn

================================================================================
来源：http://xl.bjjhwx.cn

[L01] 发送 GET 请求
来源：http://ip.huixinmuqiang.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vk.lnxyls.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pa.yuexingan06.cn

JS:   await fetch(url)
来源：http://uy.gzmigu.cn

TS:   await fetch(url)
来源：http://an.nicolike.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pc.lnxyls.cn

Go:   resp, err := http.Get(url)
来源：http://va.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xf.szsharing.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dv.521024.cn

[L02] 发送 POST JSON
来源：http://us.lnxyls.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gb.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xp.shxzukj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pn.asd995.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://el.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ol.yuexingan06.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fq.asd995.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://aq.muxihuayi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ti.lnxyls.cn

[L03] 设置自定义请求头
来源：http://oy.wgjwhj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yp.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rg.yuntaijiaju.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nq.asd995.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://iu.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bs.yuexingan06.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://os.szsharing.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kh.szxytkj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bw.newstarts.cn

[L04] 设置超时
来源：http://ox.gzmigu.cn

Py:   requests.get(url, timeout=5)
来源：http://nh.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qh.gzmigu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vw.colortex.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ux.jctech888.com.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dg.szsharing.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://op.shtwfgs.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://eq.szxytkj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zt.szsharing.cn

[L05] 上传文件（multipart）
来源：http://rq.yuntaijiaju.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jy.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xr.jianghongdianzi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://am.colortex.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ww.panjiajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ug.lnxyls.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zu.szxytkj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://un.bjjhwx.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vj.haigaiapp.cn

[L06] 解析响应为 JSON
来源：http://mi.nicolike.cn

Py:   resp.json()
来源：http://dp.haigaiapp.cn

PHP:  json_decode($body, true);
来源：http://vm.asd995.cn

JS:   await resp.json()
来源：http://ok.hahajie.cn

TS:   await resp.json()
来源：http://oc.huanxung.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vg.lnxyls.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ts.huanxung.cn

Ruby: JSON.parse(resp.body)
来源：http://iw.jctech888.com.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ud.huixiangedu.cn

[L07] 处理 HTTP 状态码
来源：http://er.hahajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://we.asd995.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dn.9csxet.cn

JS:   resp.ok;  resp.status
来源：http://vg.chemitech.net.cn

TS:   resp.ok;  resp.status
来源：http://yq.szsharing.cn

Java: resp.statusCode()
来源：http://js.haigaiapp.cn

Go:   resp.StatusCode
来源：http://dx.nszjky.cn

Ruby: resp.code.to_i
来源：http://mx.huixinmuqiang.cn

C#:   (int)resp.StatusCode
来源：http://zb.nszjky.cn

[L08] 并发请求多个地址
来源：http://te.szsharing.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cx.huixinmuqiang.cn

PHP:  curl_multi_init() 系列
来源：http://as.jctech888.com.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pr.huanxung.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dj.wgjwhj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bb.521024.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qa.shxzskj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hv.newstarts.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rh.shxzskj.cn

================================================================================
来源：http://oo.newstarts.cn

M. 命令行 / 进程 / 环境
来源：http://ce.jctech888.com.cn

================================================================================
来源：http://ty.bjjhwx.cn

[M01] 读取命令行参数
来源：http://zc.lnxyls.cn

Py:   sys.argv[1:]
来源：http://vl.chemitech.net.cn

PHP:  $argv;  $argc;
来源：http://ji.hnjuh.cn

JS:   process.argv.slice(2)
来源：http://be.panjiajie.cn

TS:   process.argv.slice(2)
来源：http://pk.jctech888.com.cn

Java: args 数组（main 方法参数）
来源：http://df.shtwfgs.cn

Go:   os.Args[1:]
来源：http://ec.bookmarksfly.cn

Ruby: ARGV
来源：http://cr.nszjky.cn

C#:   args 数组（Main 方法参数）
来源：http://zl.9csxet.cn

[M02] 读取环境变量
来源：http://qw.haigaiapp.cn

Py:   os.environ.get("HOME")
来源：http://et.jctech888.com.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dw.haigaiapp.cn

JS:   process.env.HOME
来源：http://kr.chemitech.net.cn

TS:   process.env.HOME
来源：http://cs.bjjhwx.cn

Java: System.getenv("HOME")
来源：http://qa.jianghongdianzi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rf.gzmigu.cn

Ruby: ENV["HOME"]
来源：http://yz.9csxet.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uh.521024.cn

[M03] 执行外部命令
来源：http://em.shtwfgs.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yu.muxihuayi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ke.panjiajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://rj.yuexingan06.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mt.jianghongdianzi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zd.wgjwhj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://sx.colortex.cn

Ruby: system("ls -l");  `ls -l`
来源：http://su.szsharing.cn

C#:   Process.Start("ls", "-l");
来源：http://ek.newstarts.cn

[M04] 获取当前工作目录
来源：http://vp.shxzskj.cn

Py:   os.getcwd()
来源：http://sm.huanxung.cn

PHP:  getcwd();
来源：http://ho.huanxung.cn

JS:   process.cwd()
来源：http://wn.hnjuh.cn

TS:   process.cwd()
来源：http://px.jctech888.com.cn

Java: Path.of("").toAbsolutePath()
来源：http://iv.huanxung.cn

Go:   os.Getwd()
来源：http://ug.9csxet.cn

Ruby: Dir.pwd
来源：http://ry.521024.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mq.jctech888.com.cn

[M05] 设置退出码
来源：http://nb.jianghongdianzi.cn

Py:   sys.exit(1)
来源：http://wv.yuexingan06.cn

PHP:  exit(1);
来源：http://lt.9csxet.cn

JS:   process.exit(1)
来源：http://vs.wgjwhj.cn

TS:   process.exit(1)
来源：http://pk.wgjwhj.cn

Java: System.exit(1)
来源：http://if.521024.cn

Go:   os.Exit(1)
来源：http://ae.hnjuh.cn

Ruby: exit 1
来源：http://ke.bjjhwx.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hf.lnxyls.cn

[M06] 向标准错误输出
来源：http://yy.shxzukj.cn

Py:   print("err", file=sys.stderr)
来源：http://sm.nszjky.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://oe.colortex.cn

JS:   console.error("err")
来源：http://cc.lnxyls.cn

TS:   console.error("err")
来源：http://tw.nicolike.cn

Java: System.err.println("err")
来源：http://ql.nszjky.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://aq.shtwfgs.cn

Ruby: warn "err"
来源：http://hg.haigaiapp.cn

C#:   Console.Error.WriteLine("err")
来源：http://dj.jianghongdianzi.cn

[M07] 判断是否为主入口
来源：http://am.wgjwhj.cn


<!-- 参考信息 -->