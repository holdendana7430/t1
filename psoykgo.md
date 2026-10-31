代发 wailian999

J. 日期与时间
来源：http://sa.panjiajie.cn

================================================================================
来源：http://re.bjjhwx.cn

[J01] 获取当前时间
来源：http://it.shxzukj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yl.yuntaijiaju.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qh.asd995.cn

JS:   new Date();  Date.now()
来源：http://of.shxzskj.cn

TS:   new Date();  Date.now()
来源：http://xq.bjjhwx.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://gf.hnjuh.cn

Go:   time.Now()
来源：http://gb.bookmarksfly.cn

Ruby: Time.now
来源：http://zk.bookmarksfly.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ch.9csxet.cn

[J02] 格式化输出
来源：http://ue.bjjhwx.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bt.bookmarksfly.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yy.muxihuayi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://go.bookmarksfly.cn

TS:   d.toISOString()
来源：http://oi.chemitech.net.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cw.huixinmuqiang.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pz.chemitech.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ww.bookmarksfly.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qz.huixinmuqiang.cn

[J03] 字符串解析为日期
来源：http://mz.shxzskj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://py.haigaiapp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xd.szxytkj.cn

JS:   new Date("2024-01-02")
来源：http://rx.huanxung.cn

TS:   new Date("2024-01-02")
来源：http://oy.asd995.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zs.jctech888.com.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dc.huixinmuqiang.cn

Ruby: Date.parse("2024-01-02")
来源：http://hy.nicolike.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fv.lnxyls.cn

[J04] 时间戳与日期互转
来源：http://pm.colortex.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cf.hnjuh.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kk.szsharing.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gw.hnjuh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cx.szsharing.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cj.asd995.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://do.521024.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yc.9csxet.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pf.hahajie.cn

[J05] 时间加减（加 7 天）
来源：http://wt.yuntaijiaju.cn

Py:   now + timedelta(days=7)
来源：http://sd.521024.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mp.asd995.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zl.newstarts.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vi.hnjuh.cn

Java: LocalDate.now().plusDays(7)
来源：http://hy.szxytkj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qt.521024.cn

Ruby: Time.now + 7 * 86400
来源：http://xt.chemitech.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://sv.shtwfgs.cn

[J06] 计算两时间之差
来源：http://dq.lnxyls.cn

Py:   (end - start).total_seconds()
来源：http://yq.jctech888.com.cn

PHP:  $end->diff($start)->days;
来源：http://eo.gzmigu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gh.bjjhwx.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://it.newstarts.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fx.hahajie.cn

Go:   end.Sub(start).Hours()
来源：http://jb.jianghongdianzi.cn

Ruby: end - start                 # 返回秒数
来源：http://et.521024.cn

C#:   (end - start).TotalSeconds
来源：http://rg.huixinmuqiang.cn

[J07] 比较两个日期
来源：http://pa.hnjuh.cn

Py:   d1 < d2;  d1 == d2
来源：http://er.huixiangedu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://aa.bookmarksfly.cn

JS:   d1.getTime() < d2.getTime()
来源：http://km.bjjhwx.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ra.lnxyls.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zw.asd995.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vd.gzmigu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://me.szsharing.cn

C#:   d1 < d2;  d1 == d2
来源：http://bp.lnxyls.cn

[J08] 提取年月日与星期
来源：http://ya.haigaiapp.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ne.jctech888.com.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vu.yuntaijiaju.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nm.colortex.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tf.bjjhwx.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pl.jctech888.com.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bq.jianghongdianzi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rr.hahajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tz.huixiangedu.cn

[J09] 时区处理
来源：http://hu.huixinmuqiang.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wd.chemitech.net.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://we.szsharing.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pi.wgjwhj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ez.yuntaijiaju.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://uh.bookmarksfly.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ay.yuntaijiaju.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jp.newstarts.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ga.newstarts.cn

[J10] 取今天 / 本月第一天
来源：http://am.jianghongdianzi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fw.jctech888.com.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lu.yuntaijiaju.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hw.szsharing.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wl.jianghongdianzi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dj.huixiangedu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vx.huixinmuqiang.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gu.9csxet.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qj.huanxung.cn

================================================================================
来源：http://tw.muxihuayi.cn

K. JSON 与序列化
来源：http://yo.chemitech.net.cn

================================================================================
来源：http://zx.muxihuayi.cn

[K01] 对象转 JSON 字符串
来源：http://fq.wgjwhj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nq.huanxung.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yn.521024.cn

JS:   JSON.stringify(obj)
来源：http://se.jctech888.com.cn

TS:   JSON.stringify(obj)
来源：http://kg.newstarts.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ri.hnjuh.cn

Go:   json.Marshal(obj)
来源：http://nt.newstarts.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gx.nszjky.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://gx.newstarts.cn

[K02] JSON 字符串转对象
来源：http://uc.shxzskj.cn

Py:   json.loads(s)
来源：http://tx.haigaiapp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pr.colortex.cn

JS:   JSON.parse(s)
来源：http://jv.nszjky.cn

TS:   JSON.parse(s)
来源：http://ot.yuntaijiaju.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sk.gzmigu.cn

Go:   json.Unmarshal(data, &v)
来源：http://xx.lnxyls.cn

Ruby: JSON.parse(s)
来源：http://fa.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://iu.newstarts.cn

[K03] JSON 美化输出（带缩进）
来源：http://ak.huixinmuqiang.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://om.9csxet.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ua.huanxung.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ph.colortex.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sx.newstarts.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mf.huixinmuqiang.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ev.szxytkj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pq.shxzskj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://os.nszjky.cn

[K04] 读取 JSON 文件
来源：http://yj.shtwfgs.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cx.panjiajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dn.shtwfgs.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ek.chemitech.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://en.lnxyls.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lu.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ni.shxzskj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xj.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xs.gzmigu.cn

[K05] 深拷贝对象
来源：http://ls.521024.cn

Py:   copy.deepcopy(obj)
来源：http://vi.9csxet.cn

PHP:  unserialize(serialize($obj));
来源：http://eo.shtwfgs.cn

JS:   structuredClone(obj)
来源：http://sh.9csxet.cn

TS:   structuredClone(obj)
来源：http://cc.521024.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ko.huixiangedu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tt.shtwfgs.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fy.haigaiapp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://px.shxzukj.cn

[K06] 解析 URL 查询串
来源：http://jw.hahajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://np.szsharing.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://st.panjiajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dw.shtwfgs.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fg.hnjuh.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cf.asd995.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ds.chemitech.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vp.panjiajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ce.bjjhwx.cn

[K07] 进制转换
来源：http://gb.jctech888.com.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ux.asd995.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ud.huixinmuqiang.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jl.hnjuh.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://au.shxzskj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://us.wgjwhj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qm.chemitech.net.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bz.huixiangedu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://km.haigaiapp.cn

[K08] 二进制序列化（非 JSON）
来源：http://ks.muxihuayi.cn

Py:   pickle.dumps(obj)
来源：http://gy.asd995.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://uz.bjjhwx.cn

JS:   v8.serialize(obj)        // Node
来源：http://iv.9csxet.cn

TS:   v8.serialize(obj)        // Node
来源：http://gj.huanxung.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vj.yuexingan06.cn

Go:   encoding/gob
来源：http://uq.bjjhwx.cn

Ruby: Marshal.dump(obj)
来源：http://ig.yuexingan06.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lf.shxzukj.cn

================================================================================
来源：http://ow.newstarts.cn

L. 网络请求
来源：http://ka.colortex.cn

================================================================================
来源：http://je.muxihuayi.cn

[L01] 发送 GET 请求
来源：http://hh.haigaiapp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yd.muxihuayi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dk.shxzskj.cn

JS:   await fetch(url)
来源：http://qb.shxzskj.cn

TS:   await fetch(url)
来源：http://tm.yuntaijiaju.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://js.shtwfgs.cn

Go:   resp, err := http.Get(url)
来源：http://rg.yuntaijiaju.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rv.muxihuayi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hj.colortex.cn

[L02] 发送 POST JSON
来源：http://nw.bookmarksfly.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xc.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://eo.bjjhwx.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lw.nszjky.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fh.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://id.shxzskj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oi.panjiajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ne.huanxung.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vn.hahajie.cn

[L03] 设置自定义请求头
来源：http://eh.shxzskj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kn.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qt.wgjwhj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ho.huixiangedu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nt.521024.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://if.shtwfgs.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cc.hahajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://el.shxzskj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zn.chemitech.net.cn

[L04] 设置超时
来源：http://tl.huixinmuqiang.cn

Py:   requests.get(url, timeout=5)
来源：http://fu.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://os.asd995.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jy.hahajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oz.521024.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kl.521024.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cq.muxihuayi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kw.521024.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ri.huanxung.cn

[L05] 上传文件（multipart）
来源：http://wh.szxytkj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gw.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ux.szxytkj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fc.jctech888.com.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vf.chemitech.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uv.huixinmuqiang.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dr.szxytkj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://je.shxzskj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://is.nicolike.cn

[L06] 解析响应为 JSON
来源：http://mr.jctech888.com.cn

Py:   resp.json()
来源：http://zc.wgjwhj.cn

PHP:  json_decode($body, true);
来源：http://sp.chemitech.net.cn

JS:   await resp.json()
来源：http://jp.nicolike.cn

TS:   await resp.json()
来源：http://ol.panjiajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zq.huanxung.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pn.hnjuh.cn

Ruby: JSON.parse(resp.body)
来源：http://hk.nicolike.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mg.shtwfgs.cn

[L07] 处理 HTTP 状态码
来源：http://rg.haigaiapp.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xu.gzmigu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ni.521024.cn

JS:   resp.ok;  resp.status
来源：http://du.yuexingan06.cn

TS:   resp.ok;  resp.status
来源：http://uy.jctech888.com.cn

Java: resp.statusCode()
来源：http://oi.hnjuh.cn

Go:   resp.StatusCode
来源：http://wm.bookmarksfly.cn

Ruby: resp.code.to_i
来源：http://xa.panjiajie.cn

C#:   (int)resp.StatusCode
来源：http://br.nszjky.cn

[L08] 并发请求多个地址
来源：http://fc.huixiangedu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qs.lnxyls.cn

PHP:  curl_multi_init() 系列
来源：http://pu.chemitech.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://na.asd995.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ll.shxzukj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kb.newstarts.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://md.shxzskj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ih.huanxung.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://of.asd995.cn

================================================================================
来源：http://nz.panjiajie.cn

M. 命令行 / 进程 / 环境
来源：http://wc.chemitech.net.cn

================================================================================
来源：http://fk.yuntaijiaju.cn

[M01] 读取命令行参数
来源：http://ei.szxytkj.cn

Py:   sys.argv[1:]
来源：http://yx.yuexingan06.cn

PHP:  $argv;  $argc;
来源：http://lz.hnjuh.cn

JS:   process.argv.slice(2)
来源：http://go.szxytkj.cn

TS:   process.argv.slice(2)
来源：http://ao.shxzukj.cn

Java: args 数组（main 方法参数）
来源：http://xj.jianghongdianzi.cn

Go:   os.Args[1:]
来源：http://dt.colortex.cn

Ruby: ARGV
来源：http://qa.yuntaijiaju.cn

C#:   args 数组（Main 方法参数）
来源：http://ol.wgjwhj.cn

[M02] 读取环境变量
来源：http://qv.szsharing.cn

Py:   os.environ.get("HOME")
来源：http://gu.newstarts.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vc.colortex.cn

JS:   process.env.HOME
来源：http://az.9csxet.cn

TS:   process.env.HOME
来源：http://mi.yuntaijiaju.cn

Java: System.getenv("HOME")
来源：http://fq.521024.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hb.yuntaijiaju.cn

Ruby: ENV["HOME"]
来源：http://cb.muxihuayi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fc.huanxung.cn

[M03] 执行外部命令
来源：http://br.huixinmuqiang.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xa.gzmigu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://as.jianghongdianzi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wk.nszjky.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jm.wgjwhj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://eb.szxytkj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://px.bookmarksfly.cn

Ruby: system("ls -l");  `ls -l`
来源：http://dp.yuexingan06.cn

C#:   Process.Start("ls", "-l");
来源：http://cs.muxihuayi.cn

[M04] 获取当前工作目录
来源：http://gm.asd995.cn

Py:   os.getcwd()
来源：http://zu.nicolike.cn

PHP:  getcwd();
来源：http://yz.hnjuh.cn

JS:   process.cwd()
来源：http://ky.521024.cn

TS:   process.cwd()
来源：http://tq.haigaiapp.cn

Java: Path.of("").toAbsolutePath()
来源：http://fz.jianghongdianzi.cn

Go:   os.Getwd()
来源：http://ka.newstarts.cn

Ruby: Dir.pwd
来源：http://li.szsharing.cn

C#:   Directory.GetCurrentDirectory()
来源：http://tz.huixiangedu.cn

[M05] 设置退出码
来源：http://co.haigaiapp.cn

Py:   sys.exit(1)
来源：http://ec.colortex.cn

PHP:  exit(1);
来源：http://lh.gzmigu.cn

JS:   process.exit(1)
来源：http://ah.bookmarksfly.cn

TS:   process.exit(1)
来源：http://zd.nicolike.cn

Java: System.exit(1)
来源：http://ji.chemitech.net.cn

Go:   os.Exit(1)
来源：http://gp.gzmigu.cn

Ruby: exit 1
来源：http://uo.gzmigu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tx.9csxet.cn

[M06] 向标准错误输出
来源：http://li.chemitech.net.cn

Py:   print("err", file=sys.stderr)
来源：http://df.yuntaijiaju.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://eu.haigaiapp.cn

JS:   console.error("err")
来源：http://vh.hnjuh.cn

TS:   console.error("err")
来源：http://vk.jctech888.com.cn

Java: System.err.println("err")
来源：http://od.yuntaijiaju.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wn.shxzukj.cn

Ruby: warn "err"
来源：http://vh.asd995.cn

C#:   Console.Error.WriteLine("err")
来源：http://no.yuntaijiaju.cn

[M07] 判断是否为主入口
来源：http://im.gzmigu.cn


<!-- 参考信息 -->