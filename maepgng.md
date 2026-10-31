代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vb.nszjky.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ak.muxihuayi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fq.lnxyls.cn

================================================================================
来源：http://mr.nicolike.cn

J. 日期与时间
来源：http://ew.bookmarksfly.cn

================================================================================
来源：http://ts.yuntaijiaju.cn

[J01] 获取当前时间
来源：http://pr.asd995.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://iy.nszjky.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rc.panjiajie.cn

JS:   new Date();  Date.now()
来源：http://xw.szxytkj.cn

TS:   new Date();  Date.now()
来源：http://wm.chemitech.net.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ua.huixinmuqiang.cn

Go:   time.Now()
来源：http://dd.szsharing.cn

Ruby: Time.now
来源：http://re.colortex.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ne.haigaiapp.cn

[J02] 格式化输出
来源：http://pe.asd995.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dv.9csxet.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yq.nszjky.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rs.haigaiapp.cn

TS:   d.toISOString()
来源：http://kn.newstarts.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cf.asd995.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nx.shxzskj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fl.yuexingan06.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ht.nszjky.cn

[J03] 字符串解析为日期
来源：http://lb.nszjky.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tg.colortex.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xv.colortex.cn

JS:   new Date("2024-01-02")
来源：http://vp.shxzukj.cn

TS:   new Date("2024-01-02")
来源：http://eu.bjjhwx.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cv.gzmigu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://oy.hahajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://ns.yuexingan06.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gz.huixinmuqiang.cn

[J04] 时间戳与日期互转
来源：http://zf.huixiangedu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jn.huanxung.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jf.hnjuh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wz.hahajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://oq.asd995.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bu.chemitech.net.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dv.hnjuh.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://os.bookmarksfly.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hp.9csxet.cn

[J05] 时间加减（加 7 天）
来源：http://hs.shxzukj.cn

Py:   now + timedelta(days=7)
来源：http://er.bjjhwx.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lf.hnjuh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://et.gzmigu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gzmigu.cn

Java: LocalDate.now().plusDays(7)
来源：http://gc.panjiajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ar.huixinmuqiang.cn

Ruby: Time.now + 7 * 86400
来源：http://vu.shtwfgs.cn

C#:   DateTime.Now.AddDays(7)
来源：http://mr.bjjhwx.cn

[J06] 计算两时间之差
来源：http://rz.shxzskj.cn

Py:   (end - start).total_seconds()
来源：http://cb.szxytkj.cn

PHP:  $end->diff($start)->days;
来源：http://sz.wgjwhj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://eo.szsharing.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zi.lnxyls.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zt.bjjhwx.cn

Go:   end.Sub(start).Hours()
来源：http://vw.panjiajie.cn

Ruby: end - start                 # 返回秒数
来源：http://kx.huixinmuqiang.cn

C#:   (end - start).TotalSeconds
来源：http://xm.nicolike.cn

[J07] 比较两个日期
来源：http://uk.shxzukj.cn

Py:   d1 < d2;  d1 == d2
来源：http://yv.shxzukj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://eo.shxzskj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://cj.gzmigu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ho.chemitech.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fh.yuntaijiaju.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cs.bookmarksfly.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ea.nicolike.cn

C#:   d1 < d2;  d1 == d2
来源：http://in.szsharing.cn

[J08] 提取年月日与星期
来源：http://cq.yuntaijiaju.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pn.huixinmuqiang.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uo.shxzukj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ts.nszjky.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nx.gzmigu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nk.huixiangedu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ri.szsharing.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nc.shxzukj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ek.szxytkj.cn

[J09] 时区处理
来源：http://yq.panjiajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mj.nicolike.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vr.szsharing.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qk.hnjuh.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sw.muxihuayi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kw.szsharing.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nb.wgjwhj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mj.szsharing.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wh.yuexingan06.cn

[J10] 取今天 / 本月第一天
来源：http://is.newstarts.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bh.huixinmuqiang.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qw.chemitech.net.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://re.muxihuayi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xn.chemitech.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kz.jctech888.com.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wg.colortex.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://de.asd995.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xc.bjjhwx.cn

================================================================================
来源：http://ze.nszjky.cn

K. JSON 与序列化
来源：http://ih.wgjwhj.cn

================================================================================
来源：http://kq.521024.cn

[K01] 对象转 JSON 字符串
来源：http://zg.shxzskj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mv.bjjhwx.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ns.muxihuayi.cn

JS:   JSON.stringify(obj)
来源：http://vi.panjiajie.cn

TS:   JSON.stringify(obj)
来源：http://le.muxihuayi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uh.bookmarksfly.cn

Go:   json.Marshal(obj)
来源：http://zs.bookmarksfly.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hc.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pq.shxzukj.cn

[K02] JSON 字符串转对象
来源：http://ae.jctech888.com.cn

Py:   json.loads(s)
来源：http://zp.jianghongdianzi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zc.panjiajie.cn

JS:   JSON.parse(s)
来源：http://mx.hnjuh.cn

TS:   JSON.parse(s)
来源：http://rf.lnxyls.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ei.jianghongdianzi.cn

Go:   json.Unmarshal(data, &v)
来源：http://jo.wgjwhj.cn

Ruby: JSON.parse(s)
来源：http://ge.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ts.hahajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://mr.muxihuayi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kl.hahajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://aj.hnjuh.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pc.521024.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://hw.huixinmuqiang.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rm.yuntaijiaju.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xl.jctech888.com.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vx.nicolike.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ft.colortex.cn

[K04] 读取 JSON 文件
来源：http://rw.wgjwhj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uy.521024.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nq.colortex.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xd.shtwfgs.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bq.haigaiapp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://by.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://de.bjjhwx.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dg.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ru.521024.cn

[K05] 深拷贝对象
来源：http://qw.panjiajie.cn

Py:   copy.deepcopy(obj)
来源：http://bk.huanxung.cn

PHP:  unserialize(serialize($obj));
来源：http://eq.jianghongdianzi.cn

JS:   structuredClone(obj)
来源：http://qy.nicolike.cn

TS:   structuredClone(obj)
来源：http://gi.shxzskj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ut.szxytkj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yr.wgjwhj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vr.chemitech.net.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ak.hnjuh.cn

[K06] 解析 URL 查询串
来源：http://ml.nszjky.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ee.bjjhwx.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qu.shtwfgs.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pf.huixiangedu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ex.chemitech.net.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gv.huixinmuqiang.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vf.huanxung.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://he.521024.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tq.bookmarksfly.cn

[K07] 进制转换
来源：http://xs.jianghongdianzi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ft.hnjuh.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xc.gzmigu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kk.jctech888.com.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ox.nszjky.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rf.bjjhwx.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mc.shxzukj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://so.nszjky.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vp.chemitech.net.cn

[K08] 二进制序列化（非 JSON）
来源：http://es.yuntaijiaju.cn

Py:   pickle.dumps(obj)
来源：http://sz.yuexingan06.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sq.jctech888.com.cn

JS:   v8.serialize(obj)        // Node
来源：http://po.lnxyls.cn

TS:   v8.serialize(obj)        // Node
来源：http://oa.muxihuayi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uo.lnxyls.cn

Go:   encoding/gob
来源：http://kw.nicolike.cn

Ruby: Marshal.dump(obj)
来源：http://ha.hahajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://so.521024.cn

================================================================================
来源：http://aa.shxzskj.cn

L. 网络请求
来源：http://xp.hahajie.cn

================================================================================
来源：http://mx.yuexingan06.cn

[L01] 发送 GET 请求
来源：http://qh.nicolike.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ve.asd995.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ql.muxihuayi.cn

JS:   await fetch(url)
来源：http://cy.newstarts.cn

TS:   await fetch(url)
来源：http://mn.yuntaijiaju.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ut.huixiangedu.cn

Go:   resp, err := http.Get(url)
来源：http://dg.muxihuayi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://kn.yuexingan06.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ds.bookmarksfly.cn

[L02] 发送 POST JSON
来源：http://uf.yuntaijiaju.cn

Py:   requests.post(url, json={"a": 1})
来源：http://jf.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://oc.nszjky.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wi.9csxet.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tz.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://co.shxzskj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qh.muxihuayi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ux.yuexingan06.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xs.jianghongdianzi.cn

[L03] 设置自定义请求头
来源：http://zt.colortex.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qh.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bg.yuexingan06.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bj.szxytkj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mu.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ml.chemitech.net.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cs.panjiajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dh.muxihuayi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kh.asd995.cn

[L04] 设置超时
来源：http://lp.huixinmuqiang.cn

Py:   requests.get(url, timeout=5)
来源：http://lm.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jp.huixinmuqiang.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kw.muxihuayi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yb.bookmarksfly.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mt.nicolike.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yn.panjiajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nq.haigaiapp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bb.szxytkj.cn

[L05] 上传文件（multipart）
来源：http://vw.panjiajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yj.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ep.bookmarksfly.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mp.gzmigu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bg.bjjhwx.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ja.hnjuh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sp.huixiangedu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vg.yuexingan06.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dy.521024.cn

[L06] 解析响应为 JSON
来源：http://gl.muxihuayi.cn

Py:   resp.json()
来源：http://kr.521024.cn

PHP:  json_decode($body, true);
来源：http://uk.huixiangedu.cn

JS:   await resp.json()
来源：http://uz.hnjuh.cn

TS:   await resp.json()
来源：http://ew.szxytkj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://op.gzmigu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gb.muxihuayi.cn

Ruby: JSON.parse(resp.body)
来源：http://jd.hahajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sq.muxihuayi.cn

[L07] 处理 HTTP 状态码
来源：http://pw.9csxet.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fh.hahajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bo.jctech888.com.cn

JS:   resp.ok;  resp.status
来源：http://zt.yuntaijiaju.cn

TS:   resp.ok;  resp.status
来源：http://kh.jianghongdianzi.cn

Java: resp.statusCode()
来源：http://kd.panjiajie.cn

Go:   resp.StatusCode
来源：http://wr.bjjhwx.cn

Ruby: resp.code.to_i
来源：http://sr.asd995.cn

C#:   (int)resp.StatusCode
来源：http://kx.bjjhwx.cn

[L08] 并发请求多个地址
来源：http://go.huixinmuqiang.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ai.9csxet.cn

PHP:  curl_multi_init() 系列
来源：http://gf.szsharing.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mo.jianghongdianzi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ri.shxzukj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fx.szsharing.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hp.lnxyls.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yh.9csxet.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sd.szxytkj.cn

================================================================================
来源：http://ps.wgjwhj.cn

M. 命令行 / 进程 / 环境
来源：http://ep.asd995.cn

================================================================================
来源：http://tp.521024.cn

[M01] 读取命令行参数
来源：http://hl.shxzskj.cn

Py:   sys.argv[1:]
来源：http://tx.colortex.cn

PHP:  $argv;  $argc;
来源：http://fy.szxytkj.cn

JS:   process.argv.slice(2)
来源：http://ro.hnjuh.cn

TS:   process.argv.slice(2)
来源：http://tc.muxihuayi.cn

Java: args 数组（main 方法参数）
来源：http://sc.szsharing.cn

Go:   os.Args[1:]
来源：http://zc.chemitech.net.cn

Ruby: ARGV
来源：http://ql.jctech888.com.cn

C#:   args 数组（Main 方法参数）
来源：http://po.jianghongdianzi.cn

[M02] 读取环境变量
来源：http://cl.bookmarksfly.cn

Py:   os.environ.get("HOME")
来源：http://lr.chemitech.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gc.asd995.cn

JS:   process.env.HOME
来源：http://jw.huixinmuqiang.cn

TS:   process.env.HOME
来源：http://ij.shxzskj.cn

Java: System.getenv("HOME")
来源：http://pl.yuexingan06.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zp.jctech888.com.cn

Ruby: ENV["HOME"]
来源：http://lz.nicolike.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rw.hnjuh.cn

[M03] 执行外部命令
来源：http://sj.nicolike.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ko.bookmarksfly.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pe.panjiajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zy.asd995.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jb.haigaiapp.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gr.shtwfgs.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ml.szxytkj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pg.gzmigu.cn

C#:   Process.Start("ls", "-l");
来源：http://oe.chemitech.net.cn

[M04] 获取当前工作目录
来源：http://al.haigaiapp.cn

Py:   os.getcwd()
来源：http://eo.shtwfgs.cn

PHP:  getcwd();
来源：http://nq.wgjwhj.cn

JS:   process.cwd()
来源：http://av.shtwfgs.cn

TS:   process.cwd()
来源：http://ym.nszjky.cn

Java: Path.of("").toAbsolutePath()
来源：http://kg.nicolike.cn

Go:   os.Getwd()
来源：http://au.shxzskj.cn

Ruby: Dir.pwd
来源：http://hq.yuntaijiaju.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ml.bjjhwx.cn

[M05] 设置退出码
来源：http://ef.yuntaijiaju.cn

Py:   sys.exit(1)
来源：http://fg.hnjuh.cn

PHP:  exit(1);
来源：http://xr.gzmigu.cn

JS:   process.exit(1)
来源：http://qm.newstarts.cn

TS:   process.exit(1)
来源：http://sx.huixinmuqiang.cn

Java: System.exit(1)
来源：http://jp.hahajie.cn

Go:   os.Exit(1)
来源：http://oc.shxzskj.cn

Ruby: exit 1
来源：http://lt.jianghongdianzi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ic.huixinmuqiang.cn

[M06] 向标准错误输出
来源：http://nl.yuntaijiaju.cn

Py:   print("err", file=sys.stderr)
来源：http://fl.szxytkj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://on.panjiajie.cn

JS:   console.error("err")
来源：http://kp.shtwfgs.cn

TS:   console.error("err")
来源：http://jr.jctech888.com.cn

Java: System.err.println("err")
来源：http://dp.huanxung.cn


<!-- 参考信息 -->