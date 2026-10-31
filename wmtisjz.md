代发 wailian999

J. 日期与时间
来源：http://zx.nicolike.cn

================================================================================
来源：http://jv.muxihuayi.cn

[J01] 获取当前时间
来源：http://gu.hahajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wf.chemitech.net.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ic.jianghongdianzi.cn

JS:   new Date();  Date.now()
来源：http://ml.yuntaijiaju.cn

TS:   new Date();  Date.now()
来源：http://ef.bjjhwx.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lb.nicolike.cn

Go:   time.Now()
来源：http://yy.asd995.cn

Ruby: Time.now
来源：http://ub.szsharing.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dq.asd995.cn

[J02] 格式化输出
来源：http://pz.jianghongdianzi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hv.shtwfgs.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qp.9csxet.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qt.szxytkj.cn

TS:   d.toISOString()
来源：http://cl.lnxyls.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fs.yuntaijiaju.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ef.huixiangedu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fq.chemitech.net.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ud.hnjuh.cn

[J03] 字符串解析为日期
来源：http://ca.hahajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xe.haigaiapp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vm.bjjhwx.cn

JS:   new Date("2024-01-02")
来源：http://um.muxihuayi.cn

TS:   new Date("2024-01-02")
来源：http://od.bjjhwx.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ur.shxzukj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uo.gzmigu.cn

Ruby: Date.parse("2024-01-02")
来源：http://cs.chemitech.net.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ns.wgjwhj.cn

[J04] 时间戳与日期互转
来源：http://xk.shxzukj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jl.asd995.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://us.haigaiapp.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lv.shtwfgs.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lw.yuexingan06.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://oq.gzmigu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qu.hahajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bs.huixiangedu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ju.shtwfgs.cn

[J05] 时间加减（加 7 天）
来源：http://yr.wgjwhj.cn

Py:   now + timedelta(days=7)
来源：http://es.szsharing.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wd.shtwfgs.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nw.muxihuayi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lt.huixinmuqiang.cn

Java: LocalDate.now().plusDays(7)
来源：http://br.shtwfgs.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fk.nicolike.cn

Ruby: Time.now + 7 * 86400
来源：http://fw.yuexingan06.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vm.nicolike.cn

[J06] 计算两时间之差
来源：http://xf.yuntaijiaju.cn

Py:   (end - start).total_seconds()
来源：http://eg.nszjky.cn

PHP:  $end->diff($start)->days;
来源：http://ej.521024.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fy.huanxung.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eu.shxzskj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ph.huanxung.cn

Go:   end.Sub(start).Hours()
来源：http://lx.chemitech.net.cn

Ruby: end - start                 # 返回秒数
来源：http://uq.bookmarksfly.cn

C#:   (end - start).TotalSeconds
来源：http://lr.yuntaijiaju.cn

[J07] 比较两个日期
来源：http://lu.gzmigu.cn

Py:   d1 < d2;  d1 == d2
来源：http://by.shxzskj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pn.nicolike.cn

JS:   d1.getTime() < d2.getTime()
来源：http://eg.muxihuayi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://dn.hahajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mk.wgjwhj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hd.yuexingan06.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ey.haigaiapp.cn

C#:   d1 < d2;  d1 == d2
来源：http://vg.huixinmuqiang.cn

[J08] 提取年月日与星期
来源：http://ly.bookmarksfly.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pm.shxzskj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tb.bjjhwx.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wr.gzmigu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nk.szxytkj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ak.newstarts.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pl.huixiangedu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sj.colortex.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xv.yuexingan06.cn

[J09] 时区处理
来源：http://mm.hnjuh.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uf.szxytkj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ml.colortex.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://af.shxzskj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fi.newstarts.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zk.szsharing.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nw.yuntaijiaju.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vn.newstarts.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pe.newstarts.cn

[J10] 取今天 / 本月第一天
来源：http://pd.jctech888.com.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ta.shxzskj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kl.jctech888.com.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wz.szsharing.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kj.bjjhwx.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://en.bookmarksfly.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kh.521024.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xn.szxytkj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yr.hahajie.cn

================================================================================
来源：http://ff.bookmarksfly.cn

K. JSON 与序列化
来源：http://in.szxytkj.cn

================================================================================
来源：http://wz.shxzskj.cn

[K01] 对象转 JSON 字符串
来源：http://fx.haigaiapp.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sg.colortex.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ks.gzmigu.cn

JS:   JSON.stringify(obj)
来源：http://ml.nicolike.cn

TS:   JSON.stringify(obj)
来源：http://dj.asd995.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ee.bookmarksfly.cn

Go:   json.Marshal(obj)
来源：http://dn.9csxet.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ib.nszjky.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ms.yuexingan06.cn

[K02] JSON 字符串转对象
来源：http://tj.9csxet.cn

Py:   json.loads(s)
来源：http://uh.szsharing.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mq.huixiangedu.cn

JS:   JSON.parse(s)
来源：http://wx.521024.cn

TS:   JSON.parse(s)
来源：http://td.chemitech.net.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xx.nszjky.cn

Go:   json.Unmarshal(data, &v)
来源：http://jv.haigaiapp.cn

Ruby: JSON.parse(s)
来源：http://gb.hnjuh.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ys.muxihuayi.cn

[K03] JSON 美化输出（带缩进）
来源：http://xg.yuntaijiaju.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nh.newstarts.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tw.chemitech.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://db.jctech888.com.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ob.lnxyls.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ra.wgjwhj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zd.jianghongdianzi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://yu.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ze.521024.cn

[K04] 读取 JSON 文件
来源：http://uw.9csxet.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pb.hnjuh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://po.521024.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sr.szsharing.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ll.lnxyls.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gi.9csxet.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kb.lnxyls.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://iz.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://na.asd995.cn

[K05] 深拷贝对象
来源：http://vb.jianghongdianzi.cn

Py:   copy.deepcopy(obj)
来源：http://lf.szxytkj.cn

PHP:  unserialize(serialize($obj));
来源：http://ls.521024.cn

JS:   structuredClone(obj)
来源：http://cb.shxzukj.cn

TS:   structuredClone(obj)
来源：http://th.huixinmuqiang.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bj.hahajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kh.panjiajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hm.haigaiapp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wy.jctech888.com.cn

[K06] 解析 URL 查询串
来源：http://yp.muxihuayi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kv.bookmarksfly.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://eo.shxzskj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jf.bjjhwx.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://aw.yuexingan06.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cr.lnxyls.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://la.nszjky.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ob.shtwfgs.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yl.huixiangedu.cn

[K07] 进制转换
来源：http://gc.chemitech.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ne.shxzskj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sb.hnjuh.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://md.huixinmuqiang.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vq.huixinmuqiang.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qy.jctech888.com.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mw.jianghongdianzi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rg.yuexingan06.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://be.bookmarksfly.cn

[K08] 二进制序列化（非 JSON）
来源：http://js.panjiajie.cn

Py:   pickle.dumps(obj)
来源：http://tx.nszjky.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bt.yuexingan06.cn

JS:   v8.serialize(obj)        // Node
来源：http://fo.lnxyls.cn

TS:   v8.serialize(obj)        // Node
来源：http://dd.huanxung.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mn.huanxung.cn

Go:   encoding/gob
来源：http://hn.yuntaijiaju.cn

Ruby: Marshal.dump(obj)
来源：http://do.521024.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zf.bjjhwx.cn

================================================================================
来源：http://dg.szsharing.cn

L. 网络请求
来源：http://xk.nicolike.cn

================================================================================
来源：http://dy.hahajie.cn

[L01] 发送 GET 请求
来源：http://pq.chemitech.net.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://st.jianghongdianzi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xa.szsharing.cn

JS:   await fetch(url)
来源：http://wh.shxzskj.cn

TS:   await fetch(url)
来源：http://on.jianghongdianzi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tu.shtwfgs.cn

Go:   resp, err := http.Get(url)
来源：http://km.nszjky.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://um.yuntaijiaju.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hk.haigaiapp.cn

[L02] 发送 POST JSON
来源：http://qf.huanxung.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mx.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ws.jctech888.com.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zs.panjiajie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dq.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xt.newstarts.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ca.shtwfgs.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nq.hahajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://km.hahajie.cn

[L03] 设置自定义请求头
来源：http://of.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://an.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jl.nszjky.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dm.9csxet.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mm.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cn.huanxung.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ij.lnxyls.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fv.szxytkj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fo.chemitech.net.cn

[L04] 设置超时
来源：http://wm.bookmarksfly.cn

Py:   requests.get(url, timeout=5)
来源：http://fb.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wb.hnjuh.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hm.nszjky.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nv.huixiangedu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zx.huixinmuqiang.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://an.wgjwhj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nz.chemitech.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ij.hnjuh.cn

[L05] 上传文件（multipart）
来源：http://mk.jctech888.com.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ii.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ke.yuntaijiaju.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uk.wgjwhj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ig.huixinmuqiang.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ey.newstarts.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ni.521024.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://au.shxzukj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hp.jianghongdianzi.cn

[L06] 解析响应为 JSON
来源：http://hi.wgjwhj.cn

Py:   resp.json()
来源：http://mz.haigaiapp.cn

PHP:  json_decode($body, true);
来源：http://na.wgjwhj.cn

JS:   await resp.json()
来源：http://sv.huixinmuqiang.cn

TS:   await resp.json()
来源：http://eq.9csxet.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sy.panjiajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lt.haigaiapp.cn

Ruby: JSON.parse(resp.body)
来源：http://tz.yuexingan06.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://be.huixinmuqiang.cn

[L07] 处理 HTTP 状态码
来源：http://xt.haigaiapp.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ay.9csxet.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ip.wgjwhj.cn

JS:   resp.ok;  resp.status
来源：http://ba.yuexingan06.cn

TS:   resp.ok;  resp.status
来源：http://eh.9csxet.cn

Java: resp.statusCode()
来源：http://uz.bookmarksfly.cn

Go:   resp.StatusCode
来源：http://ec.muxihuayi.cn

Ruby: resp.code.to_i
来源：http://nh.chemitech.net.cn

C#:   (int)resp.StatusCode
来源：http://tv.jianghongdianzi.cn

[L08] 并发请求多个地址
来源：http://vk.jianghongdianzi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ks.gzmigu.cn

PHP:  curl_multi_init() 系列
来源：http://yl.9csxet.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eg.colortex.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zg.colortex.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gp.wgjwhj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ml.newstarts.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://as.huixinmuqiang.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vp.jctech888.com.cn

================================================================================
来源：http://ql.szsharing.cn

M. 命令行 / 进程 / 环境
来源：http://jb.bookmarksfly.cn

================================================================================
来源：http://eq.yuexingan06.cn

[M01] 读取命令行参数
来源：http://pa.panjiajie.cn

Py:   sys.argv[1:]
来源：http://jm.yuexingan06.cn

PHP:  $argv;  $argc;
来源：http://od.chemitech.net.cn

JS:   process.argv.slice(2)
来源：http://cz.yuexingan06.cn

TS:   process.argv.slice(2)
来源：http://ek.colortex.cn

Java: args 数组（main 方法参数）
来源：http://cs.huanxung.cn

Go:   os.Args[1:]
来源：http://nz.szxytkj.cn

Ruby: ARGV
来源：http://uk.huanxung.cn

C#:   args 数组（Main 方法参数）
来源：http://vk.huixinmuqiang.cn

[M02] 读取环境变量
来源：http://sl.colortex.cn

Py:   os.environ.get("HOME")
来源：http://be.gzmigu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qf.lnxyls.cn

JS:   process.env.HOME
来源：http://rc.nszjky.cn

TS:   process.env.HOME
来源：http://wm.haigaiapp.cn

Java: System.getenv("HOME")
来源：http://gg.colortex.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mb.szxytkj.cn

Ruby: ENV["HOME"]
来源：http://rz.wgjwhj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jk.panjiajie.cn

[M03] 执行外部命令
来源：http://sg.muxihuayi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bq.bookmarksfly.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kp.shxzskj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://tl.hnjuh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gz.yuntaijiaju.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kd.9csxet.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://je.jianghongdianzi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://sq.asd995.cn

C#:   Process.Start("ls", "-l");
来源：http://uz.colortex.cn

[M04] 获取当前工作目录
来源：http://gw.gzmigu.cn

Py:   os.getcwd()
来源：http://mj.hnjuh.cn

PHP:  getcwd();
来源：http://gq.haigaiapp.cn

JS:   process.cwd()
来源：http://bd.nszjky.cn

TS:   process.cwd()
来源：http://gq.asd995.cn

Java: Path.of("").toAbsolutePath()
来源：http://sa.shxzskj.cn

Go:   os.Getwd()
来源：http://tv.szsharing.cn

Ruby: Dir.pwd
来源：http://yn.chemitech.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jh.jianghongdianzi.cn

[M05] 设置退出码
来源：http://cv.jianghongdianzi.cn

Py:   sys.exit(1)
来源：http://tj.colortex.cn

PHP:  exit(1);
来源：http://va.shxzskj.cn

JS:   process.exit(1)
来源：http://wg.huixiangedu.cn

TS:   process.exit(1)
来源：http://kc.bookmarksfly.cn

Java: System.exit(1)
来源：http://vw.szxytkj.cn

Go:   os.Exit(1)
来源：http://yf.yuntaijiaju.cn

Ruby: exit 1
来源：http://jt.shxzukj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://st.yuntaijiaju.cn

[M06] 向标准错误输出
来源：http://fb.yuexingan06.cn

Py:   print("err", file=sys.stderr)
来源：http://we.panjiajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gc.asd995.cn

JS:   console.error("err")
来源：http://eq.huixiangedu.cn

TS:   console.error("err")
来源：http://ao.shxzukj.cn

Java: System.err.println("err")
来源：http://ak.gzmigu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dc.panjiajie.cn

Ruby: warn "err"
来源：http://yy.szxytkj.cn

C#:   Console.Error.WriteLine("err")
来源：http://cn.hnjuh.cn

[M07] 判断是否为主入口
来源：http://vb.chemitech.net.cn


<!-- 参考信息 -->