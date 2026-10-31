代发 wailian999

J. 日期与时间
来源：http://xj.shxzskj.cn

================================================================================
来源：http://zq.bjjhwx.cn

[J01] 获取当前时间
来源：http://as.hnjuh.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ra.newstarts.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nu.asd995.cn

JS:   new Date();  Date.now()
来源：http://je.nszjky.cn

TS:   new Date();  Date.now()
来源：http://lj.yuexingan06.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vm.jianghongdianzi.cn

Go:   time.Now()
来源：http://gz.huanxung.cn

Ruby: Time.now
来源：http://nc.yuntaijiaju.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fv.panjiajie.cn

[J02] 格式化输出
来源：http://wy.huanxung.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gh.shxzukj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ts.asd995.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://si.chemitech.net.cn

TS:   d.toISOString()
来源：http://dt.521024.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dw.asd995.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vo.gzmigu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pg.shxzukj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ie.shxzskj.cn

[J03] 字符串解析为日期
来源：http://xd.hnjuh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://eu.panjiajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jb.jianghongdianzi.cn

JS:   new Date("2024-01-02")
来源：http://jm.jianghongdianzi.cn

TS:   new Date("2024-01-02")
来源：http://ul.9csxet.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bd.9csxet.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vp.gzmigu.cn

Ruby: Date.parse("2024-01-02")
来源：http://uh.shtwfgs.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ec.bjjhwx.cn

[J04] 时间戳与日期互转
来源：http://rv.hahajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fv.wgjwhj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lb.szsharing.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fd.hnjuh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tc.haigaiapp.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ut.muxihuayi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ii.jianghongdianzi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pz.hahajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://se.szxytkj.cn

[J05] 时间加减（加 7 天）
来源：http://cr.szxytkj.cn

Py:   now + timedelta(days=7)
来源：http://ya.9csxet.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nw.muxihuayi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yy.szsharing.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yh.colortex.cn

Java: LocalDate.now().plusDays(7)
来源：http://ry.yuntaijiaju.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gv.9csxet.cn

Ruby: Time.now + 7 * 86400
来源：http://an.colortex.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qm.hnjuh.cn

[J06] 计算两时间之差
来源：http://ie.muxihuayi.cn

Py:   (end - start).total_seconds()
来源：http://sd.chemitech.net.cn

PHP:  $end->diff($start)->days;
来源：http://rr.nszjky.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bu.haigaiapp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ap.szsharing.cn

Java: Duration.between(start, end).toSeconds()
来源：http://iu.nicolike.cn

Go:   end.Sub(start).Hours()
来源：http://dv.szsharing.cn

Ruby: end - start                 # 返回秒数
来源：http://ol.szsharing.cn

C#:   (end - start).TotalSeconds
来源：http://cp.gzmigu.cn

[J07] 比较两个日期
来源：http://mf.chemitech.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://od.panjiajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ce.newstarts.cn

JS:   d1.getTime() < d2.getTime()
来源：http://cm.wgjwhj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vq.gzmigu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ne.huixinmuqiang.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bt.newstarts.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xl.chemitech.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://pw.szsharing.cn

[J08] 提取年月日与星期
来源：http://jj.nszjky.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hj.szsharing.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ho.shxzukj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ec.panjiajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pz.yuntaijiaju.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://py.nicolike.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cy.panjiajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zq.huixiangedu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sh.yuexingan06.cn

[J09] 时区处理
来源：http://xh.hahajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rv.szxytkj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ch.huixinmuqiang.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ag.yuexingan06.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nv.bjjhwx.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yr.wgjwhj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kv.haigaiapp.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://rj.nszjky.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xd.muxihuayi.cn

[J10] 取今天 / 本月第一天
来源：http://ff.9csxet.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vk.szxytkj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ny.lnxyls.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uz.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uq.colortex.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pw.bjjhwx.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hq.hnjuh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lo.shxzskj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ny.hnjuh.cn

================================================================================
来源：http://jg.muxihuayi.cn

K. JSON 与序列化
来源：http://hf.nicolike.cn

================================================================================
来源：http://rg.yuexingan06.cn

[K01] 对象转 JSON 字符串
来源：http://me.colortex.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cm.jctech888.com.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xi.newstarts.cn

JS:   JSON.stringify(obj)
来源：http://pb.hnjuh.cn

TS:   JSON.stringify(obj)
来源：http://kx.szxytkj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qr.newstarts.cn

Go:   json.Marshal(obj)
来源：http://qg.wgjwhj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://tp.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://mt.521024.cn

[K02] JSON 字符串转对象
来源：http://ru.lnxyls.cn

Py:   json.loads(s)
来源：http://gy.hnjuh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rb.wgjwhj.cn

JS:   JSON.parse(s)
来源：http://pe.hnjuh.cn

TS:   JSON.parse(s)
来源：http://cm.wgjwhj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mc.yuexingan06.cn

Go:   json.Unmarshal(data, &v)
来源：http://jp.huixinmuqiang.cn

Ruby: JSON.parse(s)
来源：http://aj.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yp.szsharing.cn

[K03] JSON 美化输出（带缩进）
来源：http://kp.huanxung.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bu.bjjhwx.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://my.521024.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nq.colortex.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wz.panjiajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ws.jianghongdianzi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pb.asd995.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ly.lnxyls.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ny.gzmigu.cn

[K04] 读取 JSON 文件
来源：http://nn.hahajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://go.nszjky.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://oq.muxihuayi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pe.wgjwhj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mg.huixinmuqiang.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://po.huanxung.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yv.wgjwhj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://en.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fz.jctech888.com.cn

[K05] 深拷贝对象
来源：http://om.huixinmuqiang.cn

Py:   copy.deepcopy(obj)
来源：http://bc.jctech888.com.cn

PHP:  unserialize(serialize($obj));
来源：http://zy.jianghongdianzi.cn

JS:   structuredClone(obj)
来源：http://st.nszjky.cn

TS:   structuredClone(obj)
来源：http://st.asd995.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://du.bookmarksfly.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sb.yuntaijiaju.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ql.shxzukj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://eh.shxzukj.cn

[K06] 解析 URL 查询串
来源：http://mo.szxytkj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ds.yuntaijiaju.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xe.newstarts.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mk.hnjuh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ni.jianghongdianzi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uj.panjiajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://nm.shxzskj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://js.521024.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vk.hnjuh.cn

[K07] 进制转换
来源：http://sm.szsharing.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yv.huixinmuqiang.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ov.panjiajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tn.bookmarksfly.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://el.9csxet.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ok.wgjwhj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ts.newstarts.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nb.nicolike.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kc.haigaiapp.cn

[K08] 二进制序列化（非 JSON）
来源：http://rh.huixinmuqiang.cn

Py:   pickle.dumps(obj)
来源：http://ya.szxytkj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zw.nicolike.cn

JS:   v8.serialize(obj)        // Node
来源：http://yk.panjiajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://za.jctech888.com.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cg.shxzskj.cn

Go:   encoding/gob
来源：http://ow.haigaiapp.cn

Ruby: Marshal.dump(obj)
来源：http://dj.muxihuayi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jp.szsharing.cn

================================================================================
来源：http://ra.bookmarksfly.cn

L. 网络请求
来源：http://du.gzmigu.cn

================================================================================
来源：http://bo.huixinmuqiang.cn

[L01] 发送 GET 请求
来源：http://ma.shxzskj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hs.shxzukj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vp.chemitech.net.cn

JS:   await fetch(url)
来源：http://jl.muxihuayi.cn

TS:   await fetch(url)
来源：http://do.haigaiapp.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ua.jctech888.com.cn

Go:   resp, err := http.Get(url)
来源：http://ry.huixiangedu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://sz.jianghongdianzi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://au.bjjhwx.cn

[L02] 发送 POST JSON
来源：http://qa.bookmarksfly.cn

Py:   requests.post(url, json={"a": 1})
来源：http://uh.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://km.szxytkj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kx.szsharing.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hy.colortex.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rn.szxytkj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jp.gzmigu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hc.huixiangedu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bl.nszjky.cn

[L03] 设置自定义请求头
来源：http://tv.nicolike.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mp.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fo.521024.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bk.gzmigu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://aw.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bc.nszjky.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cn.yuntaijiaju.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://so.haigaiapp.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ue.hahajie.cn

[L04] 设置超时
来源：http://pl.nszjky.cn

Py:   requests.get(url, timeout=5)
来源：http://xc.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dx.huixinmuqiang.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uz.9csxet.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sr.szsharing.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bk.521024.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ag.bookmarksfly.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pb.521024.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ui.yuntaijiaju.cn

[L05] 上传文件（multipart）
来源：http://ss.jctech888.com.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ym.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ge.lnxyls.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://iw.chemitech.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yq.wgjwhj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ps.szsharing.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dx.shtwfgs.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bd.shtwfgs.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jc.521024.cn

[L06] 解析响应为 JSON
来源：http://hr.szxytkj.cn

Py:   resp.json()
来源：http://wx.haigaiapp.cn

PHP:  json_decode($body, true);
来源：http://mo.yuexingan06.cn

JS:   await resp.json()
来源：http://od.nicolike.cn

TS:   await resp.json()
来源：http://ja.yuexingan06.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rr.hnjuh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ks.huixiangedu.cn

Ruby: JSON.parse(resp.body)
来源：http://hi.panjiajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ml.chemitech.net.cn

[L07] 处理 HTTP 状态码
来源：http://gu.521024.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ny.jianghongdianzi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mz.huixinmuqiang.cn

JS:   resp.ok;  resp.status
来源：http://rq.asd995.cn

TS:   resp.ok;  resp.status
来源：http://sc.bjjhwx.cn

Java: resp.statusCode()
来源：http://lr.huanxung.cn

Go:   resp.StatusCode
来源：http://zr.jianghongdianzi.cn

Ruby: resp.code.to_i
来源：http://yz.hnjuh.cn

C#:   (int)resp.StatusCode
来源：http://uz.szsharing.cn

[L08] 并发请求多个地址
来源：http://ur.panjiajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ou.521024.cn

PHP:  curl_multi_init() 系列
来源：http://zl.shxzskj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ll.jctech888.com.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://im.asd995.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pl.yuexingan06.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pl.521024.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vi.shxzukj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://km.521024.cn

================================================================================
来源：http://le.szxytkj.cn

M. 命令行 / 进程 / 环境
来源：http://hl.bookmarksfly.cn

================================================================================
来源：http://kz.szxytkj.cn

[M01] 读取命令行参数
来源：http://kp.huanxung.cn

Py:   sys.argv[1:]
来源：http://zz.huixiangedu.cn

PHP:  $argv;  $argc;
来源：http://ed.yuexingan06.cn

JS:   process.argv.slice(2)
来源：http://om.nszjky.cn

TS:   process.argv.slice(2)
来源：http://je.jctech888.com.cn

Java: args 数组（main 方法参数）
来源：http://qy.colortex.cn

Go:   os.Args[1:]
来源：http://ue.colortex.cn

Ruby: ARGV
来源：http://dr.newstarts.cn

C#:   args 数组（Main 方法参数）
来源：http://uv.szsharing.cn

[M02] 读取环境变量
来源：http://is.yuexingan06.cn

Py:   os.environ.get("HOME")
来源：http://fs.muxihuayi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wy.haigaiapp.cn

JS:   process.env.HOME
来源：http://ht.shtwfgs.cn

TS:   process.env.HOME
来源：http://eu.nicolike.cn

Java: System.getenv("HOME")
来源：http://yj.hahajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kg.bookmarksfly.cn

Ruby: ENV["HOME"]
来源：http://iz.jctech888.com.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gr.bookmarksfly.cn

[M03] 执行外部命令
来源：http://ad.shxzukj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://by.huixiangedu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://en.haigaiapp.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hm.muxihuayi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ki.newstarts.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pu.gzmigu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://bq.bookmarksfly.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ja.szsharing.cn

C#:   Process.Start("ls", "-l");
来源：http://pg.huanxung.cn

[M04] 获取当前工作目录
来源：http://og.lnxyls.cn

Py:   os.getcwd()
来源：http://jz.yuntaijiaju.cn

PHP:  getcwd();
来源：http://zt.521024.cn

JS:   process.cwd()
来源：http://kh.shxzskj.cn

TS:   process.cwd()
来源：http://ym.yuntaijiaju.cn

Java: Path.of("").toAbsolutePath()
来源：http://ff.yuntaijiaju.cn

Go:   os.Getwd()
来源：http://hr.szxytkj.cn

Ruby: Dir.pwd
来源：http://dh.jctech888.com.cn

C#:   Directory.GetCurrentDirectory()
来源：http://te.chemitech.net.cn

[M05] 设置退出码
来源：http://pf.hahajie.cn

Py:   sys.exit(1)
来源：http://ve.newstarts.cn

PHP:  exit(1);
来源：http://yi.shtwfgs.cn

JS:   process.exit(1)
来源：http://le.nszjky.cn

TS:   process.exit(1)
来源：http://lr.newstarts.cn

Java: System.exit(1)
来源：http://xy.shxzskj.cn

Go:   os.Exit(1)
来源：http://nt.nszjky.cn

Ruby: exit 1
来源：http://th.colortex.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ff.shxzukj.cn

[M06] 向标准错误输出
来源：http://ha.521024.cn

Py:   print("err", file=sys.stderr)
来源：http://el.huanxung.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gk.jianghongdianzi.cn

JS:   console.error("err")
来源：http://fh.huanxung.cn

TS:   console.error("err")
来源：http://as.yuexingan06.cn

Java: System.err.println("err")
来源：http://hf.shtwfgs.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kq.szsharing.cn

Ruby: warn "err"
来源：http://oy.colortex.cn

C#:   Console.Error.WriteLine("err")
来源：http://ah.bjjhwx.cn

[M07] 判断是否为主入口
来源：http://hm.9csxet.cn


<!-- 参考信息 -->