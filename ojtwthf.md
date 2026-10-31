代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ae.chemitech.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fs.chemitech.net.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ic.lnxyls.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://by.yuntaijiaju.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mq.jianghongdianzi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ni.szsharing.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ju.lnxyls.cn

================================================================================
来源：http://zz.asd995.cn

J. 日期与时间
来源：http://bu.jctech888.com.cn

================================================================================
来源：http://cu.hnjuh.cn

[J01] 获取当前时间
来源：http://tw.jianghongdianzi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://aa.panjiajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ic.jianghongdianzi.cn

JS:   new Date();  Date.now()
来源：http://xc.huixinmuqiang.cn

TS:   new Date();  Date.now()
来源：http://ao.asd995.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mz.jianghongdianzi.cn

Go:   time.Now()
来源：http://xj.huixinmuqiang.cn

Ruby: Time.now
来源：http://fx.newstarts.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ty.hahajie.cn

[J02] 格式化输出
来源：http://xc.szsharing.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vw.muxihuayi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://px.huixinmuqiang.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://th.muxihuayi.cn

TS:   d.toISOString()
来源：http://eo.wgjwhj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ce.bookmarksfly.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qv.chemitech.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mq.hnjuh.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://py.yuntaijiaju.cn

[J03] 字符串解析为日期
来源：http://em.bjjhwx.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pl.shxzukj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ny.jctech888.com.cn

JS:   new Date("2024-01-02")
来源：http://jt.shxzskj.cn

TS:   new Date("2024-01-02")
来源：http://my.shxzskj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fk.szxytkj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ip.szsharing.cn

Ruby: Date.parse("2024-01-02")
来源：http://zk.jianghongdianzi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://de.hnjuh.cn

[J04] 时间戳与日期互转
来源：http://za.huixinmuqiang.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://eo.huixiangedu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://su.yuntaijiaju.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bp.hnjuh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://kq.nszjky.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cr.gzmigu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gy.lnxyls.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://aa.muxihuayi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://il.hnjuh.cn

[J05] 时间加减（加 7 天）
来源：http://sl.haigaiapp.cn

Py:   now + timedelta(days=7)
来源：http://ff.yuexingan06.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://hx.chemitech.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bh.yuexingan06.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mt.jianghongdianzi.cn

Java: LocalDate.now().plusDays(7)
来源：http://ek.bookmarksfly.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ao.bjjhwx.cn

Ruby: Time.now + 7 * 86400
来源：http://oh.shxzskj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://fw.bookmarksfly.cn

[J06] 计算两时间之差
来源：http://ok.bookmarksfly.cn

Py:   (end - start).total_seconds()
来源：http://xh.gzmigu.cn

PHP:  $end->diff($start)->days;
来源：http://ga.szsharing.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://up.colortex.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bt.szxytkj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xa.jctech888.com.cn

Go:   end.Sub(start).Hours()
来源：http://za.asd995.cn

Ruby: end - start                 # 返回秒数
来源：http://uu.nicolike.cn

C#:   (end - start).TotalSeconds
来源：http://mx.jctech888.com.cn

[J07] 比较两个日期
来源：http://nf.521024.cn

Py:   d1 < d2;  d1 == d2
来源：http://zp.asd995.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ha.wgjwhj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bx.chemitech.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jq.shxzukj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rg.nszjky.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ga.yuexingan06.cn

Ruby: d1 < d2;  d1 == d2
来源：http://dm.huanxung.cn

C#:   d1 < d2;  d1 == d2
来源：http://ws.hahajie.cn

[J08] 提取年月日与星期
来源：http://bj.yuntaijiaju.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ra.szxytkj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qb.lnxyls.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gt.szsharing.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yo.haigaiapp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ua.gzmigu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bc.shtwfgs.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qr.yuntaijiaju.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rw.haigaiapp.cn

[J09] 时区处理
来源：http://jb.yuexingan06.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rd.yuexingan06.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nj.nszjky.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vj.jctech888.com.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qz.nszjky.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://md.bookmarksfly.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yq.panjiajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mt.shtwfgs.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bv.lnxyls.cn

[J10] 取今天 / 本月第一天
来源：http://zc.shtwfgs.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bt.szxytkj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dp.colortex.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xh.bookmarksfly.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ps.asd995.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rw.bjjhwx.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://do.haigaiapp.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gy.muxihuayi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ur.hnjuh.cn

================================================================================
来源：http://qv.9csxet.cn

K. JSON 与序列化
来源：http://km.colortex.cn

================================================================================
来源：http://vp.lnxyls.cn

[K01] 对象转 JSON 字符串
来源：http://bi.nicolike.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ph.newstarts.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mw.huixiangedu.cn

JS:   JSON.stringify(obj)
来源：http://xc.yuntaijiaju.cn

TS:   JSON.stringify(obj)
来源：http://tu.shxzskj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kt.wgjwhj.cn

Go:   json.Marshal(obj)
来源：http://mk.yuexingan06.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ki.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://mp.panjiajie.cn

[K02] JSON 字符串转对象
来源：http://tg.lnxyls.cn

Py:   json.loads(s)
来源：http://ob.hnjuh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vb.jctech888.com.cn

JS:   JSON.parse(s)
来源：http://bf.szsharing.cn

TS:   JSON.parse(s)
来源：http://ze.jctech888.com.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wb.jctech888.com.cn

Go:   json.Unmarshal(data, &v)
来源：http://sn.colortex.cn

Ruby: JSON.parse(s)
来源：http://wy.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://po.yuntaijiaju.cn

[K03] JSON 美化输出（带缩进）
来源：http://su.gzmigu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jq.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://di.bookmarksfly.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ak.shtwfgs.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mv.huixinmuqiang.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dj.muxihuayi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hf.chemitech.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jr.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cm.bookmarksfly.cn

[K04] 读取 JSON 文件
来源：http://qn.9csxet.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cs.yuexingan06.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nb.jianghongdianzi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ta.haigaiapp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bx.shxzskj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vc.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://og.shxzskj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://tm.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://if.nszjky.cn

[K05] 深拷贝对象
来源：http://gt.hahajie.cn

Py:   copy.deepcopy(obj)
来源：http://md.hnjuh.cn

PHP:  unserialize(serialize($obj));
来源：http://wg.huixiangedu.cn

JS:   structuredClone(obj)
来源：http://ys.szsharing.cn

TS:   structuredClone(obj)
来源：http://vb.lnxyls.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://aq.wgjwhj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nb.9csxet.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xd.colortex.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://kg.colortex.cn

[K06] 解析 URL 查询串
来源：http://ag.haigaiapp.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nb.huixiangedu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qd.wgjwhj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rd.muxihuayi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pq.shxzukj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gk.shxzukj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fz.bookmarksfly.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ip.asd995.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kw.521024.cn

[K07] 进制转换
来源：http://ve.huanxung.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kw.asd995.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://id.9csxet.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ik.gzmigu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zl.bjjhwx.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tr.szsharing.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dg.shtwfgs.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kq.asd995.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sa.huanxung.cn

[K08] 二进制序列化（非 JSON）
来源：http://ps.muxihuayi.cn

Py:   pickle.dumps(obj)
来源：http://dh.nszjky.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://jq.yuexingan06.cn

JS:   v8.serialize(obj)        // Node
来源：http://xg.yuexingan06.cn

TS:   v8.serialize(obj)        // Node
来源：http://wt.shxzskj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://oz.wgjwhj.cn

Go:   encoding/gob
来源：http://rm.newstarts.cn

Ruby: Marshal.dump(obj)
来源：http://od.521024.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bl.szsharing.cn

================================================================================
来源：http://bf.9csxet.cn

L. 网络请求
来源：http://zt.asd995.cn

================================================================================
来源：http://kl.hnjuh.cn

[L01] 发送 GET 请求
来源：http://mi.wgjwhj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fl.nicolike.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ac.wgjwhj.cn

JS:   await fetch(url)
来源：http://ks.nszjky.cn

TS:   await fetch(url)
来源：http://gy.hahajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bv.yuexingan06.cn

Go:   resp, err := http.Get(url)
来源：http://lg.lnxyls.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ml.nicolike.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ot.colortex.cn

[L02] 发送 POST JSON
来源：http://do.colortex.cn

Py:   requests.post(url, json={"a": 1})
来源：http://uc.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cv.bookmarksfly.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ep.hnjuh.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kh.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qm.yuexingan06.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jl.asd995.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://eg.bookmarksfly.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bm.shtwfgs.cn

[L03] 设置自定义请求头
来源：http://ze.muxihuayi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pj.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ll.szxytkj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yd.asd995.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uj.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pu.lnxyls.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ub.jianghongdianzi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cg.shxzskj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vf.hahajie.cn

[L04] 设置超时
来源：http://fd.newstarts.cn

Py:   requests.get(url, timeout=5)
来源：http://ki.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ta.szsharing.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ih.huanxung.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ph.huixiangedu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yc.9csxet.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fp.hnjuh.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ah.jctech888.com.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ju.wgjwhj.cn

[L05] 上传文件（multipart）
来源：http://rk.szxytkj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nm.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rh.shxzskj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nx.yuexingan06.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pj.yuntaijiaju.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ua.nicolike.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ti.jctech888.com.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dj.panjiajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ya.bjjhwx.cn

[L06] 解析响应为 JSON
来源：http://wa.hnjuh.cn

Py:   resp.json()
来源：http://qo.huixinmuqiang.cn

PHP:  json_decode($body, true);
来源：http://dy.shtwfgs.cn

JS:   await resp.json()
来源：http://ff.9csxet.cn

TS:   await resp.json()
来源：http://ef.gzmigu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sw.chemitech.net.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kx.jctech888.com.cn

Ruby: JSON.parse(resp.body)
来源：http://lz.hnjuh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xo.chemitech.net.cn

[L07] 处理 HTTP 状态码
来源：http://us.yuntaijiaju.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bt.colortex.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fa.yuexingan06.cn

JS:   resp.ok;  resp.status
来源：http://dy.gzmigu.cn

TS:   resp.ok;  resp.status
来源：http://hz.szxytkj.cn

Java: resp.statusCode()
来源：http://kr.nszjky.cn

Go:   resp.StatusCode
来源：http://fs.szxytkj.cn

Ruby: resp.code.to_i
来源：http://qm.nicolike.cn

C#:   (int)resp.StatusCode
来源：http://ue.nszjky.cn

[L08] 并发请求多个地址
来源：http://tn.lnxyls.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ys.521024.cn

PHP:  curl_multi_init() 系列
来源：http://gs.jianghongdianzi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ro.9csxet.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qf.huixiangedu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://go.wgjwhj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lg.hnjuh.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xx.huixiangedu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kt.521024.cn

================================================================================
来源：http://pp.521024.cn

M. 命令行 / 进程 / 环境
来源：http://ix.haigaiapp.cn

================================================================================
来源：http://nc.9csxet.cn

[M01] 读取命令行参数
来源：http://re.szxytkj.cn

Py:   sys.argv[1:]
来源：http://ls.colortex.cn

PHP:  $argv;  $argc;
来源：http://bd.yuntaijiaju.cn

JS:   process.argv.slice(2)
来源：http://fo.colortex.cn

TS:   process.argv.slice(2)
来源：http://hy.panjiajie.cn

Java: args 数组（main 方法参数）
来源：http://pa.hahajie.cn

Go:   os.Args[1:]
来源：http://fo.muxihuayi.cn

Ruby: ARGV
来源：http://wq.nszjky.cn

C#:   args 数组（Main 方法参数）
来源：http://rc.panjiajie.cn

[M02] 读取环境变量
来源：http://uu.nszjky.cn

Py:   os.environ.get("HOME")
来源：http://iw.521024.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ww.asd995.cn

JS:   process.env.HOME
来源：http://lu.gzmigu.cn

TS:   process.env.HOME
来源：http://nl.colortex.cn

Java: System.getenv("HOME")
来源：http://jv.wgjwhj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mo.jianghongdianzi.cn

Ruby: ENV["HOME"]
来源：http://kh.huixinmuqiang.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rj.wgjwhj.cn

[M03] 执行外部命令
来源：http://qm.521024.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://su.yuexingan06.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zc.lnxyls.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jp.jctech888.com.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nc.newstarts.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ps.szsharing.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wb.huixinmuqiang.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kw.lnxyls.cn

C#:   Process.Start("ls", "-l");
来源：http://is.shtwfgs.cn

[M04] 获取当前工作目录
来源：http://bz.hnjuh.cn

Py:   os.getcwd()
来源：http://kg.yuexingan06.cn

PHP:  getcwd();
来源：http://qf.newstarts.cn

JS:   process.cwd()
来源：http://nm.jianghongdianzi.cn

TS:   process.cwd()
来源：http://xs.haigaiapp.cn

Java: Path.of("").toAbsolutePath()
来源：http://of.shxzukj.cn

Go:   os.Getwd()
来源：http://la.521024.cn

Ruby: Dir.pwd
来源：http://tj.chemitech.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rb.haigaiapp.cn

[M05] 设置退出码
来源：http://zu.shxzskj.cn

Py:   sys.exit(1)
来源：http://br.nicolike.cn

PHP:  exit(1);
来源：http://fh.huanxung.cn

JS:   process.exit(1)
来源：http://gt.9csxet.cn

TS:   process.exit(1)
来源：http://sb.szxytkj.cn

Java: System.exit(1)
来源：http://yx.newstarts.cn

Go:   os.Exit(1)
来源：http://yc.bjjhwx.cn

Ruby: exit 1
来源：http://dq.nszjky.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nx.shxzskj.cn

[M06] 向标准错误输出
来源：http://vb.szxytkj.cn

Py:   print("err", file=sys.stderr)
来源：http://aj.yuexingan06.cn


<!-- 参考信息 -->