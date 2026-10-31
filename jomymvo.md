代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://du.szsharing.cn

JS:   new Date();  Date.now()
来源：http://iz.asd995.cn

TS:   new Date();  Date.now()
来源：http://gi.jctech888.com.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://kw.haigaiapp.cn

Go:   time.Now()
来源：http://wv.hnjuh.cn

Ruby: Time.now
来源：http://dk.huixiangedu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zk.muxihuayi.cn

[J02] 格式化输出
来源：http://nr.521024.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lm.huanxung.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cb.hnjuh.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ex.521024.cn

TS:   d.toISOString()
来源：http://bx.shxzukj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://np.chemitech.net.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ir.haigaiapp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mr.huanxung.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zl.muxihuayi.cn

[J03] 字符串解析为日期
来源：http://gb.huixinmuqiang.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xj.newstarts.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wf.asd995.cn

JS:   new Date("2024-01-02")
来源：http://vb.shxzukj.cn

TS:   new Date("2024-01-02")
来源：http://ek.huixiangedu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vi.jctech888.com.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ff.lnxyls.cn

Ruby: Date.parse("2024-01-02")
来源：http://dd.bjjhwx.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rs.bjjhwx.cn

[J04] 时间戳与日期互转
来源：http://vh.521024.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kb.shxzukj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dy.hnjuh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jy.asd995.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ci.huanxung.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://py.shtwfgs.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jp.hahajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qd.colortex.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fj.gzmigu.cn

[J05] 时间加减（加 7 天）
来源：http://vt.nicolike.cn

Py:   now + timedelta(days=7)
来源：http://pd.wgjwhj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nk.hahajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ig.nicolike.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pu.shxzskj.cn

Java: LocalDate.now().plusDays(7)
来源：http://oc.521024.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ke.chemitech.net.cn

Ruby: Time.now + 7 * 86400
来源：http://bg.asd995.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wb.chemitech.net.cn

[J06] 计算两时间之差
来源：http://uz.huanxung.cn

Py:   (end - start).total_seconds()
来源：http://xa.huixiangedu.cn

PHP:  $end->diff($start)->days;
来源：http://ag.bjjhwx.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xj.huixiangedu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://es.jianghongdianzi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://uf.gzmigu.cn

Go:   end.Sub(start).Hours()
来源：http://ky.newstarts.cn

Ruby: end - start                 # 返回秒数
来源：http://wp.nicolike.cn

C#:   (end - start).TotalSeconds
来源：http://qk.szxytkj.cn

[J07] 比较两个日期
来源：http://ra.lnxyls.cn

Py:   d1 < d2;  d1 == d2
来源：http://wx.nicolike.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ub.chemitech.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jb.wgjwhj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://im.nszjky.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://db.9csxet.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nb.9csxet.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zq.szsharing.cn

C#:   d1 < d2;  d1 == d2
来源：http://gx.shtwfgs.cn

[J08] 提取年月日与星期
来源：http://ww.yuntaijiaju.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ji.szsharing.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://de.9csxet.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zz.szxytkj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tl.hahajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://co.shxzskj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bu.newstarts.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pb.jianghongdianzi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rz.huixiangedu.cn

[J09] 时区处理
来源：http://lk.nicolike.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ts.yuntaijiaju.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tb.bjjhwx.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wf.hnjuh.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qm.yuexingan06.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rr.asd995.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hn.chemitech.net.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://to.huixinmuqiang.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ke.9csxet.cn

[J10] 取今天 / 本月第一天
来源：http://go.muxihuayi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://oq.chemitech.net.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hf.bookmarksfly.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yy.colortex.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dn.huixiangedu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jl.newstarts.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://af.9csxet.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pz.newstarts.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uw.muxihuayi.cn

================================================================================
来源：http://xz.huixiangedu.cn

K. JSON 与序列化
来源：http://ig.huanxung.cn

================================================================================
来源：http://cq.newstarts.cn

[K01] 对象转 JSON 字符串
来源：http://sn.nszjky.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pu.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zw.hnjuh.cn

JS:   JSON.stringify(obj)
来源：http://iu.huixiangedu.cn

TS:   JSON.stringify(obj)
来源：http://wj.jianghongdianzi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fj.wgjwhj.cn

Go:   json.Marshal(obj)
来源：http://yu.nicolike.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zl.newstarts.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://cx.hnjuh.cn

[K02] JSON 字符串转对象
来源：http://jd.huixinmuqiang.cn

Py:   json.loads(s)
来源：http://pg.nicolike.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xz.jctech888.com.cn

JS:   JSON.parse(s)
来源：http://no.bookmarksfly.cn

TS:   JSON.parse(s)
来源：http://kz.bookmarksfly.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kk.shxzukj.cn

Go:   json.Unmarshal(data, &v)
来源：http://fx.haigaiapp.cn

Ruby: JSON.parse(s)
来源：http://gm.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pp.asd995.cn

[K03] JSON 美化输出（带缩进）
来源：http://yp.gzmigu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xg.hnjuh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sc.chemitech.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nj.colortex.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://pa.lnxyls.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lt.jianghongdianzi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://it.shxzukj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zs.asd995.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hu.chemitech.net.cn

[K04] 读取 JSON 文件
来源：http://op.shxzukj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bk.shxzukj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qt.colortex.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zm.nszjky.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pa.jctech888.com.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://oi.nszjky.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dh.newstarts.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yf.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fl.newstarts.cn

[K05] 深拷贝对象
来源：http://sn.shtwfgs.cn

Py:   copy.deepcopy(obj)
来源：http://ml.gzmigu.cn

PHP:  unserialize(serialize($obj));
来源：http://se.huixiangedu.cn

JS:   structuredClone(obj)
来源：http://sp.wgjwhj.cn

TS:   structuredClone(obj)
来源：http://re.wgjwhj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tc.bookmarksfly.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bv.huixinmuqiang.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cv.haigaiapp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://uq.shxzskj.cn

[K06] 解析 URL 查询串
来源：http://ph.szxytkj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fe.lnxyls.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://by.huixinmuqiang.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vg.hnjuh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tc.jianghongdianzi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://by.muxihuayi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zc.panjiajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ln.lnxyls.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://aj.muxihuayi.cn

[K07] 进制转换
来源：http://ti.muxihuayi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tm.huixiangedu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://no.colortex.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tw.hnjuh.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://oe.huixiangedu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zo.wgjwhj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pc.nicolike.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yj.muxihuayi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wy.shxzskj.cn

[K08] 二进制序列化（非 JSON）
来源：http://zu.hnjuh.cn

Py:   pickle.dumps(obj)
来源：http://xp.shxzskj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fi.lnxyls.cn

JS:   v8.serialize(obj)        // Node
来源：http://rs.newstarts.cn

TS:   v8.serialize(obj)        // Node
来源：http://gh.asd995.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kt.panjiajie.cn

Go:   encoding/gob
来源：http://nt.hnjuh.cn

Ruby: Marshal.dump(obj)
来源：http://yo.shxzukj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gd.huixinmuqiang.cn

================================================================================
来源：http://zt.huixiangedu.cn

L. 网络请求
来源：http://ti.wgjwhj.cn

================================================================================
来源：http://pw.hahajie.cn

[L01] 发送 GET 请求
来源：http://fk.huanxung.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tg.szxytkj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fl.muxihuayi.cn

JS:   await fetch(url)
来源：http://ru.yuexingan06.cn

TS:   await fetch(url)
来源：http://ev.huixiangedu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xc.bjjhwx.cn

Go:   resp, err := http.Get(url)
来源：http://tu.jianghongdianzi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ye.shxzukj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ll.colortex.cn

[L02] 发送 POST JSON
来源：http://dh.bookmarksfly.cn

Py:   requests.post(url, json={"a": 1})
来源：http://jl.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cj.asd995.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mw.nszjky.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zv.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fg.nszjky.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hp.bookmarksfly.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qn.nszjky.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mm.lnxyls.cn

[L03] 设置自定义请求头
来源：http://yy.huixinmuqiang.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sg.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sq.jctech888.com.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yy.hnjuh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://es.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gm.szsharing.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://il.521024.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lz.bookmarksfly.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zh.jianghongdianzi.cn

[L04] 设置超时
来源：http://ps.szxytkj.cn

Py:   requests.get(url, timeout=5)
来源：http://zs.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bp.huixinmuqiang.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ry.panjiajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yy.wgjwhj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tw.jctech888.com.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mc.szsharing.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yv.shxzukj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hx.newstarts.cn

[L05] 上传文件（multipart）
来源：http://uo.shxzskj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sb.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vu.gzmigu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ug.gzmigu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fw.lnxyls.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ox.hahajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ly.yuexingan06.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://is.bjjhwx.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ku.bjjhwx.cn

[L06] 解析响应为 JSON
来源：http://to.jctech888.com.cn

Py:   resp.json()
来源：http://fy.hahajie.cn

PHP:  json_decode($body, true);
来源：http://ua.yuexingan06.cn

JS:   await resp.json()
来源：http://hj.nszjky.cn

TS:   await resp.json()
来源：http://pi.jctech888.com.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jd.huixiangedu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dm.huixinmuqiang.cn

Ruby: JSON.parse(resp.body)
来源：http://ft.bjjhwx.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://or.wgjwhj.cn

[L07] 处理 HTTP 状态码
来源：http://zj.haigaiapp.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qf.colortex.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ro.huanxung.cn

JS:   resp.ok;  resp.status
来源：http://ko.521024.cn

TS:   resp.ok;  resp.status
来源：http://tc.panjiajie.cn

Java: resp.statusCode()
来源：http://rw.huixiangedu.cn

Go:   resp.StatusCode
来源：http://yv.shxzskj.cn

Ruby: resp.code.to_i
来源：http://ft.lnxyls.cn

C#:   (int)resp.StatusCode
来源：http://sm.asd995.cn

[L08] 并发请求多个地址
来源：http://ng.shxzskj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yg.nicolike.cn

PHP:  curl_multi_init() 系列
来源：http://gx.bookmarksfly.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ei.muxihuayi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qk.bookmarksfly.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://av.huixiangedu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ux.wgjwhj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mz.shxzskj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ye.jianghongdianzi.cn

================================================================================
来源：http://zz.huixinmuqiang.cn

M. 命令行 / 进程 / 环境
来源：http://vg.shtwfgs.cn

================================================================================
来源：http://zd.newstarts.cn

[M01] 读取命令行参数
来源：http://pe.shxzskj.cn

Py:   sys.argv[1:]
来源：http://gz.lnxyls.cn

PHP:  $argv;  $argc;
来源：http://mr.szsharing.cn

JS:   process.argv.slice(2)
来源：http://kq.yuexingan06.cn

TS:   process.argv.slice(2)
来源：http://od.wgjwhj.cn

Java: args 数组（main 方法参数）
来源：http://ls.asd995.cn

Go:   os.Args[1:]
来源：http://lr.huixiangedu.cn

Ruby: ARGV
来源：http://mh.gzmigu.cn

C#:   args 数组（Main 方法参数）
来源：http://jb.bookmarksfly.cn

[M02] 读取环境变量
来源：http://zt.szsharing.cn

Py:   os.environ.get("HOME")
来源：http://sn.colortex.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://do.nicolike.cn

JS:   process.env.HOME
来源：http://yk.521024.cn

TS:   process.env.HOME
来源：http://lr.huixiangedu.cn

Java: System.getenv("HOME")
来源：http://qs.panjiajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oj.bookmarksfly.cn

Ruby: ENV["HOME"]
来源：http://vk.yuntaijiaju.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xv.521024.cn

[M03] 执行外部命令
来源：http://ss.huixiangedu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ry.huixiangedu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://om.szxytkj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hx.asd995.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nd.9csxet.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ca.gzmigu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wn.hnjuh.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yi.521024.cn

C#:   Process.Start("ls", "-l");
来源：http://wh.huixinmuqiang.cn

[M04] 获取当前工作目录
来源：http://lw.nicolike.cn

Py:   os.getcwd()
来源：http://ai.bookmarksfly.cn

PHP:  getcwd();
来源：http://ow.asd995.cn

JS:   process.cwd()
来源：http://mm.chemitech.net.cn

TS:   process.cwd()
来源：http://wf.hahajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://dx.chemitech.net.cn

Go:   os.Getwd()
来源：http://iu.hnjuh.cn

Ruby: Dir.pwd
来源：http://ha.chemitech.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ym.colortex.cn

[M05] 设置退出码
来源：http://bh.szsharing.cn

Py:   sys.exit(1)
来源：http://rx.asd995.cn

PHP:  exit(1);
来源：http://ac.huixiangedu.cn

JS:   process.exit(1)
来源：http://ya.shtwfgs.cn

TS:   process.exit(1)
来源：http://xy.shtwfgs.cn

Java: System.exit(1)
来源：http://pj.521024.cn

Go:   os.Exit(1)
来源：http://ov.colortex.cn

Ruby: exit 1
来源：http://ff.lnxyls.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pb.huixinmuqiang.cn

[M06] 向标准错误输出
来源：http://mm.szxytkj.cn

Py:   print("err", file=sys.stderr)
来源：http://wm.bookmarksfly.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kd.yuntaijiaju.cn

JS:   console.error("err")
来源：http://kl.muxihuayi.cn

TS:   console.error("err")
来源：http://te.shxzukj.cn

Java: System.err.println("err")
来源：http://ha.huanxung.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jj.szsharing.cn

Ruby: warn "err"
来源：http://pj.panjiajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://iu.yuntaijiaju.cn

[M07] 判断是否为主入口
来源：http://wa.yuntaijiaju.cn

Py:   if __name__ == "__main__":
来源：http://qb.lnxyls.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://me.521024.cn

JS:   require.main === module
来源：http://ic.shxzukj.cn

TS:   require.main === module
来源：http://ot.shxzskj.cn


<!-- 参考信息 -->