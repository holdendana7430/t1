代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ko.hnjuh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yp.yuntaijiaju.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uv.chemitech.net.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ve.newstarts.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ot.hnjuh.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xe.hahajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://in.lnxyls.cn

================================================================================
来源：http://kl.shxzukj.cn

J. 日期与时间
来源：http://pl.asd995.cn

================================================================================
来源：http://le.hahajie.cn

[J01] 获取当前时间
来源：http://lh.nszjky.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://gs.bjjhwx.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mw.yuexingan06.cn

JS:   new Date();  Date.now()
来源：http://cp.521024.cn

TS:   new Date();  Date.now()
来源：http://ec.hahajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://go.yuntaijiaju.cn

Go:   time.Now()
来源：http://es.asd995.cn

Ruby: Time.now
来源：http://vh.szsharing.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lv.shxzskj.cn

[J02] 格式化输出
来源：http://nd.jianghongdianzi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zi.shtwfgs.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qv.shxzskj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sy.newstarts.cn

TS:   d.toISOString()
来源：http://yo.szsharing.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pg.jianghongdianzi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://uk.newstarts.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vy.bjjhwx.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xa.szxytkj.cn

[J03] 字符串解析为日期
来源：http://ad.hahajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uj.521024.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gj.shxzukj.cn

JS:   new Date("2024-01-02")
来源：http://zc.panjiajie.cn

TS:   new Date("2024-01-02")
来源：http://es.huanxung.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dp.yuntaijiaju.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yh.huixinmuqiang.cn

Ruby: Date.parse("2024-01-02")
来源：http://ad.asd995.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fj.huanxung.cn

[J04] 时间戳与日期互转
来源：http://er.muxihuayi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kz.yuexingan06.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kv.yuntaijiaju.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ul.huanxung.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gx.jianghongdianzi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mx.newstarts.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ps.szxytkj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rn.shxzukj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://iv.521024.cn

[J05] 时间加减（加 7 天）
来源：http://ou.hnjuh.cn

Py:   now + timedelta(days=7)
来源：http://es.huixinmuqiang.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mh.nszjky.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ij.newstarts.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rp.nicolike.cn

Java: LocalDate.now().plusDays(7)
来源：http://xu.muxihuayi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://br.bookmarksfly.cn

Ruby: Time.now + 7 * 86400
来源：http://sv.shxzskj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pp.szxytkj.cn

[J06] 计算两时间之差
来源：http://hd.panjiajie.cn

Py:   (end - start).total_seconds()
来源：http://zl.hahajie.cn

PHP:  $end->diff($start)->days;
来源：http://mq.9csxet.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tx.huixinmuqiang.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eb.shxzukj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://wi.yuntaijiaju.cn

Go:   end.Sub(start).Hours()
来源：http://lc.panjiajie.cn

Ruby: end - start                 # 返回秒数
来源：http://do.jianghongdianzi.cn

C#:   (end - start).TotalSeconds
来源：http://br.shxzukj.cn

[J07] 比较两个日期
来源：http://yj.nszjky.cn

Py:   d1 < d2;  d1 == d2
来源：http://cx.bjjhwx.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hm.521024.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zt.521024.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zx.huixinmuqiang.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gv.shxzukj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hv.hahajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cl.shxzukj.cn

C#:   d1 < d2;  d1 == d2
来源：http://in.asd995.cn

[J08] 提取年月日与星期
来源：http://nx.shtwfgs.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kk.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://py.shxzskj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ih.szsharing.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zx.gzmigu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://oi.szxytkj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://be.yuntaijiaju.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tf.jctech888.com.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ki.panjiajie.cn

[J09] 时区处理
来源：http://px.colortex.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vt.huanxung.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ug.yuexingan06.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gj.bjjhwx.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fo.gzmigu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bt.hahajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hs.gzmigu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ll.huixiangedu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fl.shtwfgs.cn

[J10] 取今天 / 本月第一天
来源：http://cg.chemitech.net.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tc.bookmarksfly.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mm.shxzskj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vg.hnjuh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qc.jianghongdianzi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vr.huixinmuqiang.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gn.nicolike.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cw.huanxung.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nc.521024.cn

================================================================================
来源：http://ii.hahajie.cn

K. JSON 与序列化
来源：http://dz.shxzskj.cn

================================================================================
来源：http://vm.jianghongdianzi.cn

[K01] 对象转 JSON 字符串
来源：http://if.shxzskj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nt.gzmigu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gp.szsharing.cn

JS:   JSON.stringify(obj)
来源：http://wa.hnjuh.cn

TS:   JSON.stringify(obj)
来源：http://wr.huixiangedu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ay.jctech888.com.cn

Go:   json.Marshal(obj)
来源：http://rz.huixiangedu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://de.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://uj.szsharing.cn

[K02] JSON 字符串转对象
来源：http://ah.jianghongdianzi.cn

Py:   json.loads(s)
来源：http://hg.shtwfgs.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://em.hnjuh.cn

JS:   JSON.parse(s)
来源：http://sa.yuntaijiaju.cn

TS:   JSON.parse(s)
来源：http://gp.yuexingan06.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xk.colortex.cn

Go:   json.Unmarshal(data, &v)
来源：http://nc.yuntaijiaju.cn

Ruby: JSON.parse(s)
来源：http://ne.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sj.bjjhwx.cn

[K03] JSON 美化输出（带缩进）
来源：http://bm.gzmigu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ff.bjjhwx.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ic.521024.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pj.jctech888.com.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://dv.nicolike.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xu.haigaiapp.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uh.521024.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hy.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xb.yuexingan06.cn

[K04] 读取 JSON 文件
来源：http://zu.huixiangedu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gm.shxzskj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mo.chemitech.net.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://td.huixiangedu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://no.chemitech.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fz.gzmigu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xd.colortex.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zv.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://io.wgjwhj.cn

[K05] 深拷贝对象
来源：http://fd.szsharing.cn

Py:   copy.deepcopy(obj)
来源：http://bz.gzmigu.cn

PHP:  unserialize(serialize($obj));
来源：http://zz.colortex.cn

JS:   structuredClone(obj)
来源：http://dt.bjjhwx.cn

TS:   structuredClone(obj)
来源：http://pz.jctech888.com.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://or.jianghongdianzi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://li.shxzukj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vo.jctech888.com.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vo.jctech888.com.cn

[K06] 解析 URL 查询串
来源：http://ec.huixiangedu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mu.wgjwhj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jx.lnxyls.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jt.9csxet.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cg.panjiajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hn.bookmarksfly.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://kf.lnxyls.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tl.panjiajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zk.muxihuayi.cn

[K07] 进制转换
来源：http://ie.521024.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lz.shxzukj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rm.shxzskj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pw.newstarts.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yz.nszjky.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ac.shtwfgs.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nf.szsharing.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ft.shxzukj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gf.haigaiapp.cn

[K08] 二进制序列化（非 JSON）
来源：http://ai.szxytkj.cn

Py:   pickle.dumps(obj)
来源：http://lu.shxzukj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://kr.huixinmuqiang.cn

JS:   v8.serialize(obj)        // Node
来源：http://iw.shxzskj.cn

TS:   v8.serialize(obj)        // Node
来源：http://fo.yuntaijiaju.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://oj.nicolike.cn

Go:   encoding/gob
来源：http://oz.newstarts.cn

Ruby: Marshal.dump(obj)
来源：http://ry.jctech888.com.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xj.asd995.cn

================================================================================
来源：http://jq.szsharing.cn

L. 网络请求
来源：http://pl.yuntaijiaju.cn

================================================================================
来源：http://vy.szxytkj.cn

[L01] 发送 GET 请求
来源：http://wd.huixinmuqiang.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uz.jctech888.com.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mm.jianghongdianzi.cn

JS:   await fetch(url)
来源：http://gd.lnxyls.cn

TS:   await fetch(url)
来源：http://lr.jianghongdianzi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hv.jctech888.com.cn

Go:   resp, err := http.Get(url)
来源：http://ol.panjiajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://yo.asd995.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lh.huanxung.cn

[L02] 发送 POST JSON
来源：http://uo.huixiangedu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ax.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://do.asd995.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://es.9csxet.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zi.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ux.hahajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ep.muxihuayi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sx.chemitech.net.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sd.huanxung.cn

[L03] 设置自定义请求头
来源：http://zj.jctech888.com.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bn.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yl.lnxyls.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jj.newstarts.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uj.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bz.asd995.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://he.szxytkj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rm.yuntaijiaju.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tm.jctech888.com.cn

[L04] 设置超时
来源：http://ye.hahajie.cn

Py:   requests.get(url, timeout=5)
来源：http://rx.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bz.9csxet.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://op.newstarts.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ne.colortex.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qk.yuexingan06.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kd.huanxung.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ml.chemitech.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lj.jctech888.com.cn

[L05] 上传文件（multipart）
来源：http://ju.panjiajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qi.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nf.bookmarksfly.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://oi.szsharing.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://aw.hahajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://oc.nszjky.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hr.nszjky.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dw.bjjhwx.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rj.colortex.cn

[L06] 解析响应为 JSON
来源：http://vo.szxytkj.cn

Py:   resp.json()
来源：http://bn.hnjuh.cn

PHP:  json_decode($body, true);
来源：http://is.jctech888.com.cn

JS:   await resp.json()
来源：http://oj.asd995.cn

TS:   await resp.json()
来源：http://wu.huixiangedu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rr.newstarts.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gu.9csxet.cn

Ruby: JSON.parse(resp.body)
来源：http://bz.muxihuayi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://if.yuntaijiaju.cn

[L07] 处理 HTTP 状态码
来源：http://an.szxytkj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hg.9csxet.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cv.gzmigu.cn

JS:   resp.ok;  resp.status
来源：http://lf.huixinmuqiang.cn

TS:   resp.ok;  resp.status
来源：http://pm.szxytkj.cn

Java: resp.statusCode()
来源：http://wm.jctech888.com.cn

Go:   resp.StatusCode
来源：http://hn.szsharing.cn

Ruby: resp.code.to_i
来源：http://kh.huanxung.cn

C#:   (int)resp.StatusCode
来源：http://ab.hnjuh.cn

[L08] 并发请求多个地址
来源：http://ci.asd995.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://aw.lnxyls.cn

PHP:  curl_multi_init() 系列
来源：http://qr.jianghongdianzi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pg.huixinmuqiang.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pm.nszjky.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hs.shxzukj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://og.muxihuayi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://av.521024.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pq.chemitech.net.cn

================================================================================
来源：http://re.lnxyls.cn

M. 命令行 / 进程 / 环境
来源：http://ji.colortex.cn

================================================================================
来源：http://zc.szsharing.cn

[M01] 读取命令行参数
来源：http://si.bjjhwx.cn

Py:   sys.argv[1:]
来源：http://tn.shxzskj.cn

PHP:  $argv;  $argc;
来源：http://at.nicolike.cn

JS:   process.argv.slice(2)
来源：http://et.lnxyls.cn

TS:   process.argv.slice(2)
来源：http://hb.jianghongdianzi.cn

Java: args 数组（main 方法参数）
来源：http://tj.yuntaijiaju.cn

Go:   os.Args[1:]
来源：http://wb.panjiajie.cn

Ruby: ARGV
来源：http://jz.shxzskj.cn

C#:   args 数组（Main 方法参数）
来源：http://ha.huanxung.cn

[M02] 读取环境变量
来源：http://uf.huixinmuqiang.cn

Py:   os.environ.get("HOME")
来源：http://ka.yuexingan06.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://we.haigaiapp.cn

JS:   process.env.HOME
来源：http://wg.hahajie.cn

TS:   process.env.HOME
来源：http://ea.9csxet.cn

Java: System.getenv("HOME")
来源：http://sv.nszjky.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jf.wgjwhj.cn

Ruby: ENV["HOME"]
来源：http://bt.nicolike.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hn.szsharing.cn

[M03] 执行外部命令
来源：http://lw.jianghongdianzi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ql.newstarts.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gl.huanxung.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ck.hnjuh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pe.huixiangedu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sr.chemitech.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jb.gzmigu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ya.huixinmuqiang.cn

C#:   Process.Start("ls", "-l");
来源：http://oh.chemitech.net.cn

[M04] 获取当前工作目录
来源：http://xb.shxzukj.cn

Py:   os.getcwd()
来源：http://wv.szxytkj.cn

PHP:  getcwd();
来源：http://qa.huixiangedu.cn

JS:   process.cwd()
来源：http://kt.bookmarksfly.cn

TS:   process.cwd()
来源：http://tj.hahajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://cq.haigaiapp.cn

Go:   os.Getwd()
来源：http://ep.wgjwhj.cn

Ruby: Dir.pwd
来源：http://ui.bookmarksfly.cn

C#:   Directory.GetCurrentDirectory()
来源：http://pb.hahajie.cn

[M05] 设置退出码
来源：http://ll.521024.cn

Py:   sys.exit(1)
来源：http://hk.shxzskj.cn

PHP:  exit(1);
来源：http://gz.bookmarksfly.cn

JS:   process.exit(1)
来源：http://xt.nicolike.cn

TS:   process.exit(1)
来源：http://hi.newstarts.cn

Java: System.exit(1)
来源：http://yx.shxzskj.cn

Go:   os.Exit(1)
来源：http://gw.panjiajie.cn

Ruby: exit 1
来源：http://ii.colortex.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rc.newstarts.cn

[M06] 向标准错误输出
来源：http://mx.yuexingan06.cn

Py:   print("err", file=sys.stderr)
来源：http://lk.huanxung.cn


<!-- 参考信息 -->