代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vz.hnjuh.cn

JS:   new Date();  Date.now()
来源：http://hw.chemitech.net.cn

TS:   new Date();  Date.now()
来源：http://wv.wgjwhj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lr.nszjky.cn

Go:   time.Now()
来源：http://aq.gzmigu.cn

Ruby: Time.now
来源：http://xi.szxytkj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ac.chemitech.net.cn

[J02] 格式化输出
来源：http://ke.bjjhwx.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fb.jianghongdianzi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sa.bookmarksfly.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lu.szxytkj.cn

TS:   d.toISOString()
来源：http://rx.muxihuayi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zs.hahajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sf.huanxung.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ot.haigaiapp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kl.yuntaijiaju.cn

[J03] 字符串解析为日期
来源：http://ve.bookmarksfly.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qq.bjjhwx.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uu.bjjhwx.cn

JS:   new Date("2024-01-02")
来源：http://ti.521024.cn

TS:   new Date("2024-01-02")
来源：http://qq.newstarts.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jy.yuexingan06.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://he.yuexingan06.cn

Ruby: Date.parse("2024-01-02")
来源：http://mu.muxihuayi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ct.huixiangedu.cn

[J04] 时间戳与日期互转
来源：http://nn.asd995.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xd.yuntaijiaju.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://aw.yuntaijiaju.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zc.asd995.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ix.chemitech.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://py.521024.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lk.panjiajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pw.chemitech.net.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ry.haigaiapp.cn

[J05] 时间加减（加 7 天）
来源：http://qg.chemitech.net.cn

Py:   now + timedelta(days=7)
来源：http://hi.jctech888.com.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xq.huixinmuqiang.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rx.nicolike.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yi.muxihuayi.cn

Java: LocalDate.now().plusDays(7)
来源：http://du.bookmarksfly.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tm.wgjwhj.cn

Ruby: Time.now + 7 * 86400
来源：http://pj.hahajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://oa.asd995.cn

[J06] 计算两时间之差
来源：http://ph.nicolike.cn

Py:   (end - start).total_seconds()
来源：http://oa.9csxet.cn

PHP:  $end->diff($start)->days;
来源：http://oz.nszjky.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ai.huixiangedu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vg.huixinmuqiang.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mn.shxzukj.cn

Go:   end.Sub(start).Hours()
来源：http://gl.hahajie.cn

Ruby: end - start                 # 返回秒数
来源：http://ap.newstarts.cn

C#:   (end - start).TotalSeconds
来源：http://ee.bjjhwx.cn

[J07] 比较两个日期
来源：http://gt.nszjky.cn

Py:   d1 < d2;  d1 == d2
来源：http://gl.yuexingan06.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pz.haigaiapp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hs.hahajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zt.newstarts.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hy.bjjhwx.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xb.gzmigu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zd.huixiangedu.cn

C#:   d1 < d2;  d1 == d2
来源：http://nf.szsharing.cn

[J08] 提取年月日与星期
来源：http://bl.bookmarksfly.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pg.shxzukj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xf.szsharing.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tp.shxzskj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bh.wgjwhj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cj.lnxyls.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://li.muxihuayi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ta.gzmigu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gz.newstarts.cn

[J09] 时区处理
来源：http://hs.asd995.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tt.yuntaijiaju.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vj.lnxyls.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://al.lnxyls.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iy.bookmarksfly.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zv.szxytkj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cc.nicolike.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://dz.asd995.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://st.lnxyls.cn

[J10] 取今天 / 本月第一天
来源：http://mu.jianghongdianzi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://qp.bjjhwx.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tj.shxzskj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vl.bjjhwx.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qd.shxzskj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ch.nicolike.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zf.jianghongdianzi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://be.wgjwhj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cb.colortex.cn

================================================================================
来源：http://gi.haigaiapp.cn

K. JSON 与序列化
来源：http://gq.gzmigu.cn

================================================================================
来源：http://yx.bjjhwx.cn

[K01] 对象转 JSON 字符串
来源：http://js.gzmigu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://oi.huixiangedu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ct.lnxyls.cn

JS:   JSON.stringify(obj)
来源：http://xc.muxihuayi.cn

TS:   JSON.stringify(obj)
来源：http://ah.yuexingan06.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gu.jctech888.com.cn

Go:   json.Marshal(obj)
来源：http://fx.shxzskj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gd.newstarts.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://kw.hnjuh.cn

[K02] JSON 字符串转对象
来源：http://og.huixinmuqiang.cn

Py:   json.loads(s)
来源：http://wk.huixiangedu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sn.huixinmuqiang.cn

JS:   JSON.parse(s)
来源：http://qe.shxzukj.cn

TS:   JSON.parse(s)
来源：http://xz.jianghongdianzi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://su.nicolike.cn

Go:   json.Unmarshal(data, &v)
来源：http://sf.gzmigu.cn

Ruby: JSON.parse(s)
来源：http://oz.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nu.huixinmuqiang.cn

[K03] JSON 美化输出（带缩进）
来源：http://eu.huixinmuqiang.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rq.chemitech.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mb.9csxet.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qz.colortex.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://pn.huanxung.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vw.yuntaijiaju.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://df.huixinmuqiang.cn

Ruby: JSON.pretty_generate(obj)
来源：http://tz.hnjuh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ht.newstarts.cn

[K04] 读取 JSON 文件
来源：http://wz.muxihuayi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wd.newstarts.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lg.huixiangedu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://er.huixiangedu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aa.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tq.521024.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xw.hahajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jx.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vr.hahajie.cn

[K05] 深拷贝对象
来源：http://kt.huixinmuqiang.cn

Py:   copy.deepcopy(obj)
来源：http://mz.asd995.cn

PHP:  unserialize(serialize($obj));
来源：http://dn.asd995.cn

JS:   structuredClone(obj)
来源：http://dd.asd995.cn

TS:   structuredClone(obj)
来源：http://mk.lnxyls.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://oe.colortex.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yw.asd995.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://eg.hnjuh.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://sd.asd995.cn

[K06] 解析 URL 查询串
来源：http://rp.hnjuh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rp.shxzskj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ju.shtwfgs.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sv.shxzskj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fh.521024.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vh.nicolike.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://es.shxzukj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fl.yuntaijiaju.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kw.muxihuayi.cn

[K07] 进制转换
来源：http://zw.shxzukj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hs.nszjky.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yg.shtwfgs.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hi.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://me.shxzskj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://aw.jctech888.com.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ts.bookmarksfly.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cy.muxihuayi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lk.colortex.cn

[K08] 二进制序列化（非 JSON）
来源：http://xu.haigaiapp.cn

Py:   pickle.dumps(obj)
来源：http://ig.panjiajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fd.chemitech.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://jq.gzmigu.cn

TS:   v8.serialize(obj)        // Node
来源：http://if.shxzukj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zv.9csxet.cn

Go:   encoding/gob
来源：http://tc.gzmigu.cn

Ruby: Marshal.dump(obj)
来源：http://xc.newstarts.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ff.colortex.cn

================================================================================
来源：http://pb.hnjuh.cn

L. 网络请求
来源：http://iq.szxytkj.cn

================================================================================
来源：http://uh.szsharing.cn

[L01] 发送 GET 请求
来源：http://xy.shxzukj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cg.gzmigu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qj.lnxyls.cn

JS:   await fetch(url)
来源：http://dq.jianghongdianzi.cn

TS:   await fetch(url)
来源：http://wu.yuexingan06.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://op.szsharing.cn

Go:   resp, err := http.Get(url)
来源：http://ng.jianghongdianzi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ua.hahajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gx.yuexingan06.cn

[L02] 发送 POST JSON
来源：http://fi.asd995.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zl.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xj.nicolike.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dd.jctech888.com.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gj.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qq.yuntaijiaju.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qs.szsharing.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sd.lnxyls.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lx.huixiangedu.cn

[L03] 设置自定义请求头
来源：http://pl.hahajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kn.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jo.wgjwhj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bb.lnxyls.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ni.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fj.haigaiapp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tk.gzmigu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://eo.muxihuayi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fr.gzmigu.cn

[L04] 设置超时
来源：http://qi.panjiajie.cn

Py:   requests.get(url, timeout=5)
来源：http://yt.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vf.shxzukj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ox.jctech888.com.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ra.nicolike.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ew.colortex.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ji.haigaiapp.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cf.shtwfgs.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ju.newstarts.cn

[L05] 上传文件（multipart）
来源：http://uv.nszjky.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kv.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ky.bjjhwx.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kv.huixiangedu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://az.hahajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yo.hnjuh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uf.huanxung.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ku.shtwfgs.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kr.bjjhwx.cn

[L06] 解析响应为 JSON
来源：http://kc.nszjky.cn

Py:   resp.json()
来源：http://wq.hnjuh.cn

PHP:  json_decode($body, true);
来源：http://lq.shxzskj.cn

JS:   await resp.json()
来源：http://ju.asd995.cn

TS:   await resp.json()
来源：http://do.gzmigu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ql.hnjuh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tx.szxytkj.cn

Ruby: JSON.parse(resp.body)
来源：http://se.muxihuayi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ma.gzmigu.cn

[L07] 处理 HTTP 状态码
来源：http://ts.asd995.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vk.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://om.lnxyls.cn

JS:   resp.ok;  resp.status
来源：http://es.shxzskj.cn

TS:   resp.ok;  resp.status
来源：http://kc.jianghongdianzi.cn

Java: resp.statusCode()
来源：http://bb.huixiangedu.cn

Go:   resp.StatusCode
来源：http://ut.shxzskj.cn

Ruby: resp.code.to_i
来源：http://nl.newstarts.cn

C#:   (int)resp.StatusCode
来源：http://nr.hahajie.cn

[L08] 并发请求多个地址
来源：http://hj.newstarts.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://co.huixiangedu.cn

PHP:  curl_multi_init() 系列
来源：http://sh.huixinmuqiang.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uy.szsharing.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ts.lnxyls.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://px.yuntaijiaju.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jo.huixiangedu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ih.huanxung.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://db.newstarts.cn

================================================================================
来源：http://ut.nicolike.cn

M. 命令行 / 进程 / 环境
来源：http://fk.bookmarksfly.cn

================================================================================
来源：http://uo.haigaiapp.cn

[M01] 读取命令行参数
来源：http://pf.asd995.cn

Py:   sys.argv[1:]
来源：http://xc.colortex.cn

PHP:  $argv;  $argc;
来源：http://pn.gzmigu.cn

JS:   process.argv.slice(2)
来源：http://yy.521024.cn

TS:   process.argv.slice(2)
来源：http://re.shtwfgs.cn

Java: args 数组（main 方法参数）
来源：http://ej.newstarts.cn

Go:   os.Args[1:]
来源：http://tt.yuntaijiaju.cn

Ruby: ARGV
来源：http://il.yuexingan06.cn

C#:   args 数组（Main 方法参数）
来源：http://by.asd995.cn

[M02] 读取环境变量
来源：http://mt.shtwfgs.cn

Py:   os.environ.get("HOME")
来源：http://oo.yuntaijiaju.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://el.szsharing.cn

JS:   process.env.HOME
来源：http://qe.bookmarksfly.cn

TS:   process.env.HOME
来源：http://am.9csxet.cn

Java: System.getenv("HOME")
来源：http://qa.hahajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gw.521024.cn

Ruby: ENV["HOME"]
来源：http://ah.szsharing.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ra.yuexingan06.cn

[M03] 执行外部命令
来源：http://sw.muxihuayi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fk.gzmigu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wc.newstarts.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://td.gzmigu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ih.panjiajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://au.colortex.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://sx.haigaiapp.cn

Ruby: system("ls -l");  `ls -l`
来源：http://dq.shtwfgs.cn

C#:   Process.Start("ls", "-l");
来源：http://pp.nszjky.cn

[M04] 获取当前工作目录
来源：http://vr.lnxyls.cn

Py:   os.getcwd()
来源：http://qu.szxytkj.cn

PHP:  getcwd();
来源：http://zj.jianghongdianzi.cn

JS:   process.cwd()
来源：http://cd.jianghongdianzi.cn

TS:   process.cwd()
来源：http://eq.9csxet.cn

Java: Path.of("").toAbsolutePath()
来源：http://hc.huixinmuqiang.cn

Go:   os.Getwd()
来源：http://jj.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://yk.yuexingan06.cn

C#:   Directory.GetCurrentDirectory()
来源：http://pg.asd995.cn

[M05] 设置退出码
来源：http://hj.colortex.cn

Py:   sys.exit(1)
来源：http://lz.hahajie.cn

PHP:  exit(1);
来源：http://gi.hahajie.cn

JS:   process.exit(1)
来源：http://jt.yuexingan06.cn

TS:   process.exit(1)
来源：http://pr.muxihuayi.cn

Java: System.exit(1)
来源：http://hx.gzmigu.cn

Go:   os.Exit(1)
来源：http://ma.bookmarksfly.cn

Ruby: exit 1
来源：http://lr.huixinmuqiang.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uh.bookmarksfly.cn

[M06] 向标准错误输出
来源：http://by.huixinmuqiang.cn

Py:   print("err", file=sys.stderr)
来源：http://pd.chemitech.net.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://da.9csxet.cn

JS:   console.error("err")
来源：http://ff.newstarts.cn

TS:   console.error("err")
来源：http://ol.shxzskj.cn

Java: System.err.println("err")
来源：http://ea.gzmigu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yh.hnjuh.cn

Ruby: warn "err"
来源：http://ac.bjjhwx.cn

C#:   Console.Error.WriteLine("err")
来源：http://eb.gzmigu.cn

[M07] 判断是否为主入口
来源：http://qw.huanxung.cn

Py:   if __name__ == "__main__":
来源：http://fa.huanxung.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ic.hnjuh.cn

JS:   require.main === module
来源：http://er.szxytkj.cn

TS:   require.main === module
来源：http://mp.huixiangedu.cn


<!-- 参考信息 -->