代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ct.szsharing.cn

JS:   new Date();  Date.now()
来源：http://by.huixinmuqiang.cn

TS:   new Date();  Date.now()
来源：http://yu.bookmarksfly.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://cr.jctech888.com.cn

Go:   time.Now()
来源：http://tr.colortex.cn

Ruby: Time.now
来源：http://ul.jctech888.com.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ci.yuexingan06.cn

[J02] 格式化输出
来源：http://ks.9csxet.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://we.wgjwhj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qi.asd995.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://co.huanxung.cn

TS:   d.toISOString()
来源：http://qf.bjjhwx.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fm.yuexingan06.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ze.lnxyls.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ta.shtwfgs.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://oc.asd995.cn

[J03] 字符串解析为日期
来源：http://pa.szxytkj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ii.gzmigu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zf.jianghongdianzi.cn

JS:   new Date("2024-01-02")
来源：http://nx.newstarts.cn

TS:   new Date("2024-01-02")
来源：http://ft.lnxyls.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dw.9csxet.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ly.muxihuayi.cn

Ruby: Date.parse("2024-01-02")
来源：http://aa.hnjuh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rl.newstarts.cn

[J04] 时间戳与日期互转
来源：http://od.gzmigu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yc.huixiangedu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ql.shxzskj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ks.haigaiapp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bt.yuexingan06.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qg.bookmarksfly.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pj.shxzskj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xf.hahajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cr.panjiajie.cn

[J05] 时间加减（加 7 天）
来源：http://cf.yuntaijiaju.cn

Py:   now + timedelta(days=7)
来源：http://dj.muxihuayi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://en.yuexingan06.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rp.yuntaijiaju.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xw.yuexingan06.cn

Java: LocalDate.now().plusDays(7)
来源：http://dd.nicolike.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hd.wgjwhj.cn

Ruby: Time.now + 7 * 86400
来源：http://cr.huixiangedu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wm.wgjwhj.cn

[J06] 计算两时间之差
来源：http://ke.hahajie.cn

Py:   (end - start).total_seconds()
来源：http://nn.huanxung.cn

PHP:  $end->diff($start)->days;
来源：http://nr.chemitech.net.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fa.gzmigu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ey.haigaiapp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://kf.shxzukj.cn

Go:   end.Sub(start).Hours()
来源：http://fs.521024.cn

Ruby: end - start                 # 返回秒数
来源：http://dg.huanxung.cn

C#:   (end - start).TotalSeconds
来源：http://ah.shtwfgs.cn

[J07] 比较两个日期
来源：http://pp.jianghongdianzi.cn

Py:   d1 < d2;  d1 == d2
来源：http://lj.huanxung.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rf.hnjuh.cn

JS:   d1.getTime() < d2.getTime()
来源：http://yu.asd995.cn

TS:   d1.getTime() < d2.getTime()
来源：http://px.lnxyls.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ye.newstarts.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pt.yuntaijiaju.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cz.haigaiapp.cn

C#:   d1 < d2;  d1 == d2
来源：http://nd.gzmigu.cn

[J08] 提取年月日与星期
来源：http://uk.newstarts.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wk.chemitech.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qu.shxzskj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://oc.9csxet.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wz.9csxet.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jw.jctech888.com.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://go.chemitech.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sl.shxzukj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yu.jianghongdianzi.cn

[J09] 时区处理
来源：http://vk.haigaiapp.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mh.shxzukj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xs.shtwfgs.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uc.wgjwhj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kw.hahajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ok.colortex.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wu.nicolike.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://up.bjjhwx.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jm.521024.cn

[J10] 取今天 / 本月第一天
来源：http://gu.shxzskj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kd.yuexingan06.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ek.yuntaijiaju.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dc.shtwfgs.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vm.shxzukj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://py.szsharing.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jn.shtwfgs.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ws.jianghongdianzi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gl.bookmarksfly.cn

================================================================================
来源：http://lf.huixinmuqiang.cn

K. JSON 与序列化
来源：http://tm.szsharing.cn

================================================================================
来源：http://tl.chemitech.net.cn

[K01] 对象转 JSON 字符串
来源：http://lj.huixinmuqiang.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hp.huixiangedu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jm.haigaiapp.cn

JS:   JSON.stringify(obj)
来源：http://nv.521024.cn

TS:   JSON.stringify(obj)
来源：http://dv.shxzskj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yk.szsharing.cn

Go:   json.Marshal(obj)
来源：http://fo.bjjhwx.cn

Ruby: obj.to_json                                     // require "json"
来源：http://yx.asd995.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rx.yuntaijiaju.cn

[K02] JSON 字符串转对象
来源：http://oi.wgjwhj.cn

Py:   json.loads(s)
来源：http://of.bjjhwx.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bc.9csxet.cn

JS:   JSON.parse(s)
来源：http://sc.gzmigu.cn

TS:   JSON.parse(s)
来源：http://hs.huanxung.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lf.chemitech.net.cn

Go:   json.Unmarshal(data, &v)
来源：http://fv.panjiajie.cn

Ruby: JSON.parse(s)
来源：http://yp.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kg.lnxyls.cn

[K03] JSON 美化输出（带缩进）
来源：http://ec.asd995.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://va.9csxet.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bk.wgjwhj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://tz.jctech888.com.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gl.nicolike.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bk.shxzukj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bm.wgjwhj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xt.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ez.bjjhwx.cn

[K04] 读取 JSON 文件
来源：http://zz.9csxet.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hw.szsharing.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cr.huixiangedu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mk.lnxyls.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zi.szxytkj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ts.szsharing.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hu.chemitech.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ct.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bc.9csxet.cn

[K05] 深拷贝对象
来源：http://wj.chemitech.net.cn

Py:   copy.deepcopy(obj)
来源：http://qh.chemitech.net.cn

PHP:  unserialize(serialize($obj));
来源：http://ke.wgjwhj.cn

JS:   structuredClone(obj)
来源：http://ln.bookmarksfly.cn

TS:   structuredClone(obj)
来源：http://nr.lnxyls.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://iq.gzmigu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ow.gzmigu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://br.jctech888.com.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hl.asd995.cn

[K06] 解析 URL 查询串
来源：http://ft.szxytkj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nx.huixiangedu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pc.newstarts.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xa.bjjhwx.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fl.lnxyls.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wx.chemitech.net.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://uc.huanxung.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tn.wgjwhj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://am.huanxung.cn

[K07] 进制转换
来源：http://cq.9csxet.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://og.szxytkj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://db.jctech888.com.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fr.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://oa.huanxung.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mu.jctech888.com.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lt.yuntaijiaju.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nb.szsharing.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yv.panjiajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://te.colortex.cn

Py:   pickle.dumps(obj)
来源：http://ec.asd995.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bm.colortex.cn

JS:   v8.serialize(obj)        // Node
来源：http://xz.panjiajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://bx.bookmarksfly.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sm.muxihuayi.cn

Go:   encoding/gob
来源：http://lg.521024.cn

Ruby: Marshal.dump(obj)
来源：http://le.huanxung.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bt.shxzukj.cn

================================================================================
来源：http://ks.shtwfgs.cn

L. 网络请求
来源：http://fw.shtwfgs.cn

================================================================================
来源：http://oi.gzmigu.cn

[L01] 发送 GET 请求
来源：http://cv.asd995.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mz.hnjuh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://us.huixiangedu.cn

JS:   await fetch(url)
来源：http://dp.9csxet.cn

TS:   await fetch(url)
来源：http://xi.nicolike.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vw.wgjwhj.cn

Go:   resp, err := http.Get(url)
来源：http://bx.bookmarksfly.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://te.yuntaijiaju.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nn.nszjky.cn

[L02] 发送 POST JSON
来源：http://ae.gzmigu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pb.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wk.jctech888.com.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sz.colortex.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://to.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cw.hahajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gz.colortex.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ew.hahajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pv.colortex.cn

[L03] 设置自定义请求头
来源：http://ti.szsharing.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jk.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kw.shxzukj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ql.yuntaijiaju.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://es.colortex.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qq.shtwfgs.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://um.yuntaijiaju.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xj.hnjuh.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://he.yuexingan06.cn

[L04] 设置超时
来源：http://nl.hnjuh.cn

Py:   requests.get(url, timeout=5)
来源：http://iu.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hi.shxzskj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://id.521024.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lo.shtwfgs.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ww.jctech888.com.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yl.gzmigu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ep.hahajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ax.shxzukj.cn

[L05] 上传文件（multipart）
来源：http://ey.asd995.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://up.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ha.jianghongdianzi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wv.gzmigu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wm.yuntaijiaju.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hm.shtwfgs.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rp.nszjky.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ko.huanxung.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rk.jianghongdianzi.cn

[L06] 解析响应为 JSON
来源：http://mz.bookmarksfly.cn

Py:   resp.json()
来源：http://sr.asd995.cn

PHP:  json_decode($body, true);
来源：http://qm.gzmigu.cn

JS:   await resp.json()
来源：http://rl.nszjky.cn

TS:   await resp.json()
来源：http://pr.asd995.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://va.hnjuh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cq.szsharing.cn

Ruby: JSON.parse(resp.body)
来源：http://pe.colortex.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bu.bjjhwx.cn

[L07] 处理 HTTP 状态码
来源：http://kv.chemitech.net.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sv.panjiajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ue.wgjwhj.cn

JS:   resp.ok;  resp.status
来源：http://ne.wgjwhj.cn

TS:   resp.ok;  resp.status
来源：http://tq.yuexingan06.cn

Java: resp.statusCode()
来源：http://dt.szsharing.cn

Go:   resp.StatusCode
来源：http://zs.9csxet.cn

Ruby: resp.code.to_i
来源：http://wk.yuntaijiaju.cn

C#:   (int)resp.StatusCode
来源：http://pi.chemitech.net.cn

[L08] 并发请求多个地址
来源：http://pe.wgjwhj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ud.wgjwhj.cn

PHP:  curl_multi_init() 系列
来源：http://jm.haigaiapp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://id.colortex.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sf.haigaiapp.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nx.panjiajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kk.asd995.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tj.huixinmuqiang.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://es.shxzukj.cn

================================================================================
来源：http://lj.shxzskj.cn

M. 命令行 / 进程 / 环境
来源：http://vb.muxihuayi.cn

================================================================================
来源：http://nv.haigaiapp.cn

[M01] 读取命令行参数
来源：http://ao.panjiajie.cn

Py:   sys.argv[1:]
来源：http://ss.gzmigu.cn

PHP:  $argv;  $argc;
来源：http://yi.huanxung.cn

JS:   process.argv.slice(2)
来源：http://hl.haigaiapp.cn

TS:   process.argv.slice(2)
来源：http://tc.muxihuayi.cn

Java: args 数组（main 方法参数）
来源：http://dl.muxihuayi.cn

Go:   os.Args[1:]
来源：http://sx.nszjky.cn

Ruby: ARGV
来源：http://zt.nszjky.cn

C#:   args 数组（Main 方法参数）
来源：http://jd.hnjuh.cn

[M02] 读取环境变量
来源：http://au.huanxung.cn

Py:   os.environ.get("HOME")
来源：http://yj.9csxet.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yt.nicolike.cn

JS:   process.env.HOME
来源：http://bh.asd995.cn

TS:   process.env.HOME
来源：http://dv.panjiajie.cn

Java: System.getenv("HOME")
来源：http://vm.521024.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gl.yuexingan06.cn

Ruby: ENV["HOME"]
来源：http://in.shxzukj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pi.shxzukj.cn

[M03] 执行外部命令
来源：http://tf.chemitech.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fm.lnxyls.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kr.lnxyls.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://sb.gzmigu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ii.gzmigu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ap.yuntaijiaju.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://aa.panjiajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://li.szxytkj.cn

C#:   Process.Start("ls", "-l");
来源：http://zs.yuntaijiaju.cn

[M04] 获取当前工作目录
来源：http://qj.szxytkj.cn

Py:   os.getcwd()
来源：http://cc.chemitech.net.cn

PHP:  getcwd();
来源：http://tr.hnjuh.cn

JS:   process.cwd()
来源：http://vl.huixinmuqiang.cn

TS:   process.cwd()
来源：http://wg.huixinmuqiang.cn

Java: Path.of("").toAbsolutePath()
来源：http://fc.szxytkj.cn

Go:   os.Getwd()
来源：http://cf.wgjwhj.cn

Ruby: Dir.pwd
来源：http://fb.shxzskj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://lr.huixinmuqiang.cn

[M05] 设置退出码
来源：http://ea.jctech888.com.cn

Py:   sys.exit(1)
来源：http://zd.lnxyls.cn

PHP:  exit(1);
来源：http://tc.shxzskj.cn

JS:   process.exit(1)
来源：http://vr.gzmigu.cn

TS:   process.exit(1)
来源：http://ja.huanxung.cn

Java: System.exit(1)
来源：http://ra.hahajie.cn

Go:   os.Exit(1)
来源：http://uf.yuntaijiaju.cn

Ruby: exit 1
来源：http://wj.yuexingan06.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kv.bjjhwx.cn

[M06] 向标准错误输出
来源：http://ax.nicolike.cn

Py:   print("err", file=sys.stderr)
来源：http://kk.shtwfgs.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://nv.bjjhwx.cn

JS:   console.error("err")
来源：http://ga.hnjuh.cn

TS:   console.error("err")
来源：http://pi.chemitech.net.cn

Java: System.err.println("err")
来源：http://ak.colortex.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ad.gzmigu.cn

Ruby: warn "err"
来源：http://wv.chemitech.net.cn

C#:   Console.Error.WriteLine("err")
来源：http://da.newstarts.cn

[M07] 判断是否为主入口
来源：http://cp.muxihuayi.cn

Py:   if __name__ == "__main__":
来源：http://ga.chemitech.net.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wm.hahajie.cn

JS:   require.main === module
来源：http://mu.shtwfgs.cn

TS:   require.main === module
来源：http://rw.bookmarksfly.cn


<!-- 参考信息 -->