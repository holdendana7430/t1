代发 wailian999

Ruby: s.scan(/error/i)
来源：http://xj.9csxet.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://om.gzmigu.cn

[I08] 贪婪与非贪婪匹配
来源：http://sy.9csxet.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jg.hahajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yr.hahajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fc.chemitech.net.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uj.shxzskj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://dg.shxzukj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hq.shxzukj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rn.yuexingan06.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qy.panjiajie.cn

================================================================================
来源：http://ym.gzmigu.cn

J. 日期与时间
来源：http://jx.9csxet.cn

================================================================================
来源：http://ba.muxihuayi.cn

[J01] 获取当前时间
来源：http://iy.hahajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ij.szsharing.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qm.wgjwhj.cn

JS:   new Date();  Date.now()
来源：http://mu.chemitech.net.cn

TS:   new Date();  Date.now()
来源：http://lh.nicolike.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://sw.asd995.cn

Go:   time.Now()
来源：http://ge.szsharing.cn

Ruby: Time.now
来源：http://mh.haigaiapp.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ja.muxihuayi.cn

[J02] 格式化输出
来源：http://aw.hahajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pu.szxytkj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bn.hahajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ho.bookmarksfly.cn

TS:   d.toISOString()
来源：http://dq.bjjhwx.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xf.yuntaijiaju.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://iq.hahajie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sn.nicolike.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ea.shxzukj.cn

[J03] 字符串解析为日期
来源：http://qu.huanxung.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://it.hahajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cu.521024.cn

JS:   new Date("2024-01-02")
来源：http://hk.hnjuh.cn

TS:   new Date("2024-01-02")
来源：http://vf.haigaiapp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qn.shxzskj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ks.lnxyls.cn

Ruby: Date.parse("2024-01-02")
来源：http://rx.nszjky.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ev.521024.cn

[J04] 时间戳与日期互转
来源：http://mp.jctech888.com.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xb.shtwfgs.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ia.shxzukj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wg.nicolike.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zf.huixiangedu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://eh.wgjwhj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bw.hahajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wz.asd995.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tn.shtwfgs.cn

[J05] 时间加减（加 7 天）
来源：http://hw.panjiajie.cn

Py:   now + timedelta(days=7)
来源：http://vp.nszjky.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bl.asd995.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wh.newstarts.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://de.jianghongdianzi.cn

Java: LocalDate.now().plusDays(7)
来源：http://up.shtwfgs.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ij.nicolike.cn

Ruby: Time.now + 7 * 86400
来源：http://ef.huixiangedu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xk.hahajie.cn

[J06] 计算两时间之差
来源：http://td.hnjuh.cn

Py:   (end - start).total_seconds()
来源：http://kh.muxihuayi.cn

PHP:  $end->diff($start)->days;
来源：http://zd.9csxet.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mf.asd995.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fg.shtwfgs.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ha.muxihuayi.cn

Go:   end.Sub(start).Hours()
来源：http://kf.nicolike.cn

Ruby: end - start                 # 返回秒数
来源：http://ms.nicolike.cn

C#:   (end - start).TotalSeconds
来源：http://zq.szsharing.cn

[J07] 比较两个日期
来源：http://qc.jctech888.com.cn

Py:   d1 < d2;  d1 == d2
来源：http://fe.jianghongdianzi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rx.yuexingan06.cn

JS:   d1.getTime() < d2.getTime()
来源：http://yt.shxzskj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://dh.521024.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fp.jianghongdianzi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qy.panjiajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vw.jianghongdianzi.cn

C#:   d1 < d2;  d1 == d2
来源：http://mu.shxzukj.cn

[J08] 提取年月日与星期
来源：http://vn.chemitech.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ei.shxzskj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ay.colortex.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mq.shxzskj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nd.jctech888.com.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dq.521024.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dk.panjiajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pk.muxihuayi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ab.nicolike.cn

[J09] 时区处理
来源：http://qf.panjiajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yw.colortex.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://on.521024.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qx.panjiajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jm.huixiangedu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xi.gzmigu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xp.hnjuh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xz.jctech888.com.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vh.nicolike.cn

[J10] 取今天 / 本月第一天
来源：http://rn.shxzskj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cc.haigaiapp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sg.9csxet.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rp.9csxet.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ov.shtwfgs.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qv.huanxung.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rs.wgjwhj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vm.newstarts.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dh.hahajie.cn

================================================================================
来源：http://hq.yuntaijiaju.cn

K. JSON 与序列化
来源：http://ba.521024.cn

================================================================================
来源：http://ed.nicolike.cn

[K01] 对象转 JSON 字符串
来源：http://dn.gzmigu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tm.bookmarksfly.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rn.bjjhwx.cn

JS:   JSON.stringify(obj)
来源：http://hl.panjiajie.cn

TS:   JSON.stringify(obj)
来源：http://qf.jctech888.com.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wz.nszjky.cn

Go:   json.Marshal(obj)
来源：http://fg.newstarts.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mf.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hn.szxytkj.cn

[K02] JSON 字符串转对象
来源：http://wl.muxihuayi.cn

Py:   json.loads(s)
来源：http://hs.jianghongdianzi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fo.jianghongdianzi.cn

JS:   JSON.parse(s)
来源：http://sw.shtwfgs.cn

TS:   JSON.parse(s)
来源：http://qn.521024.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fg.hahajie.cn

Go:   json.Unmarshal(data, &v)
来源：http://pj.yuntaijiaju.cn

Ruby: JSON.parse(s)
来源：http://hy.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dy.shtwfgs.cn

[K03] JSON 美化输出（带缩进）
来源：http://zl.bookmarksfly.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mu.haigaiapp.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yv.huanxung.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wk.hahajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ft.chemitech.net.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fu.muxihuayi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zv.shxzukj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://cf.gzmigu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wf.huixiangedu.cn

[K04] 读取 JSON 文件
来源：http://ov.shtwfgs.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://im.bookmarksfly.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ef.jianghongdianzi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://df.yuexingan06.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tx.lnxyls.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jn.szsharing.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ll.huixiangedu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://cb.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fr.9csxet.cn

[K05] 深拷贝对象
来源：http://cm.chemitech.net.cn

Py:   copy.deepcopy(obj)
来源：http://jv.521024.cn

PHP:  unserialize(serialize($obj));
来源：http://va.huanxung.cn

JS:   structuredClone(obj)
来源：http://fe.huixinmuqiang.cn

TS:   structuredClone(obj)
来源：http://oh.yuntaijiaju.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://so.9csxet.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sl.shxzskj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kk.hnjuh.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dz.yuntaijiaju.cn

[K06] 解析 URL 查询串
来源：http://gp.hnjuh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ps.muxihuayi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yg.shxzskj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fd.bookmarksfly.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dw.bjjhwx.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bm.9csxet.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://yx.wgjwhj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lp.hnjuh.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uw.9csxet.cn

[K07] 进制转换
来源：http://jw.huixiangedu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zk.jianghongdianzi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yx.bjjhwx.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wu.jctech888.com.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yj.newstarts.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://he.huanxung.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qr.szxytkj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ez.newstarts.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ny.bookmarksfly.cn

[K08] 二进制序列化（非 JSON）
来源：http://lh.shxzukj.cn

Py:   pickle.dumps(obj)
来源：http://hn.yuexingan06.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yv.jianghongdianzi.cn

JS:   v8.serialize(obj)        // Node
来源：http://zz.huixiangedu.cn

TS:   v8.serialize(obj)        // Node
来源：http://lx.bjjhwx.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://no.huixinmuqiang.cn

Go:   encoding/gob
来源：http://ir.asd995.cn

Ruby: Marshal.dump(obj)
来源：http://se.521024.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uy.lnxyls.cn

================================================================================
来源：http://pe.9csxet.cn

L. 网络请求
来源：http://jc.9csxet.cn

================================================================================
来源：http://uf.shtwfgs.cn

[L01] 发送 GET 请求
来源：http://pa.wgjwhj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qv.jianghongdianzi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://aq.bookmarksfly.cn

JS:   await fetch(url)
来源：http://ub.gzmigu.cn

TS:   await fetch(url)
来源：http://os.nicolike.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nq.panjiajie.cn

Go:   resp, err := http.Get(url)
来源：http://xz.shxzskj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wa.haigaiapp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mc.nicolike.cn

[L02] 发送 POST JSON
来源：http://hc.chemitech.net.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hw.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dy.shtwfgs.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bl.haigaiapp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gg.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yx.521024.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bq.huanxung.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fb.szxytkj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://eh.nszjky.cn

[L03] 设置自定义请求头
来源：http://no.wgjwhj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hl.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vh.jianghongdianzi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sx.panjiajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qx.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yg.szxytkj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zx.yuexingan06.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hm.jctech888.com.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://oc.nicolike.cn

[L04] 设置超时
来源：http://se.chemitech.net.cn

Py:   requests.get(url, timeout=5)
来源：http://od.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ku.nszjky.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xj.asd995.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zh.yuntaijiaju.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qo.521024.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rj.521024.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://np.nicolike.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://af.nicolike.cn

[L05] 上传文件（multipart）
来源：http://ke.bookmarksfly.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://th.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ji.wgjwhj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ye.huanxung.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sf.bjjhwx.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gs.chemitech.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jl.9csxet.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mj.9csxet.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wp.panjiajie.cn

[L06] 解析响应为 JSON
来源：http://vu.muxihuayi.cn

Py:   resp.json()
来源：http://kz.huixiangedu.cn

PHP:  json_decode($body, true);
来源：http://at.muxihuayi.cn

JS:   await resp.json()
来源：http://hy.szsharing.cn

TS:   await resp.json()
来源：http://de.yuntaijiaju.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qj.shxzukj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ol.jctech888.com.cn

Ruby: JSON.parse(resp.body)
来源：http://ph.hnjuh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rx.colortex.cn

[L07] 处理 HTTP 状态码
来源：http://ay.colortex.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bg.szxytkj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uu.jctech888.com.cn

JS:   resp.ok;  resp.status
来源：http://vc.huanxung.cn

TS:   resp.ok;  resp.status
来源：http://bd.hnjuh.cn

Java: resp.statusCode()
来源：http://jj.haigaiapp.cn

Go:   resp.StatusCode
来源：http://ay.colortex.cn

Ruby: resp.code.to_i
来源：http://gl.shxzskj.cn

C#:   (int)resp.StatusCode
来源：http://jb.shxzskj.cn

[L08] 并发请求多个地址
来源：http://rm.newstarts.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tp.521024.cn

PHP:  curl_multi_init() 系列
来源：http://jn.shxzukj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sx.colortex.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ns.haigaiapp.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://px.nicolike.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://or.hahajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uu.9csxet.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ne.colortex.cn

================================================================================
来源：http://vj.bjjhwx.cn

M. 命令行 / 进程 / 环境
来源：http://it.521024.cn

================================================================================
来源：http://ab.nszjky.cn

[M01] 读取命令行参数
来源：http://vg.colortex.cn

Py:   sys.argv[1:]
来源：http://vi.panjiajie.cn

PHP:  $argv;  $argc;
来源：http://ea.9csxet.cn

JS:   process.argv.slice(2)
来源：http://gk.newstarts.cn

TS:   process.argv.slice(2)
来源：http://zs.yuexingan06.cn

Java: args 数组（main 方法参数）
来源：http://kj.yuexingan06.cn

Go:   os.Args[1:]
来源：http://hl.bookmarksfly.cn

Ruby: ARGV
来源：http://dr.asd995.cn

C#:   args 数组（Main 方法参数）
来源：http://ln.bookmarksfly.cn

[M02] 读取环境变量
来源：http://kq.panjiajie.cn

Py:   os.environ.get("HOME")
来源：http://jq.chemitech.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fx.yuexingan06.cn

JS:   process.env.HOME
来源：http://hc.huanxung.cn

TS:   process.env.HOME
来源：http://gg.asd995.cn

Java: System.getenv("HOME")
来源：http://cz.gzmigu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yo.jctech888.com.cn

Ruby: ENV["HOME"]
来源：http://pz.yuexingan06.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://th.nszjky.cn

[M03] 执行外部命令
来源：http://yp.yuntaijiaju.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pg.wgjwhj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yn.szxytkj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ga.shtwfgs.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://hj.jianghongdianzi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gv.wgjwhj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://yx.muxihuayi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://cn.jianghongdianzi.cn

C#:   Process.Start("ls", "-l");
来源：http://af.huanxung.cn

[M04] 获取当前工作目录
来源：http://pk.panjiajie.cn

Py:   os.getcwd()
来源：http://fi.hnjuh.cn

PHP:  getcwd();
来源：http://xu.jianghongdianzi.cn

JS:   process.cwd()
来源：http://hg.haigaiapp.cn

TS:   process.cwd()
来源：http://dd.shxzskj.cn

Java: Path.of("").toAbsolutePath()
来源：http://xf.huanxung.cn

Go:   os.Getwd()
来源：http://rd.shxzukj.cn

Ruby: Dir.pwd
来源：http://kk.szxytkj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sw.yuntaijiaju.cn

[M05] 设置退出码
来源：http://bu.panjiajie.cn

Py:   sys.exit(1)
来源：http://vo.shxzukj.cn

PHP:  exit(1);
来源：http://zr.panjiajie.cn

JS:   process.exit(1)
来源：http://fz.chemitech.net.cn

TS:   process.exit(1)
来源：http://ho.shtwfgs.cn

Java: System.exit(1)
来源：http://ne.jctech888.com.cn

Go:   os.Exit(1)
来源：http://hm.huixinmuqiang.cn


<!-- 参考信息 -->