代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bc.wgjwhj.cn

TS:   /error/gim
来源：http://nl.hnjuh.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jd.haigaiapp.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tc.hahajie.cn

Ruby: s.scan(/error/i)
来源：http://ei.szxytkj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hk.jctech888.com.cn

[I08] 贪婪与非贪婪匹配
来源：http://pt.lnxyls.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mw.hahajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xg.hahajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://eo.haigaiapp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qy.newstarts.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ag.shtwfgs.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gc.shxzskj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://el.yuntaijiaju.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ef.huixinmuqiang.cn

================================================================================
来源：http://zk.jianghongdianzi.cn

J. 日期与时间
来源：http://xy.hahajie.cn

================================================================================
来源：http://up.szxytkj.cn

[J01] 获取当前时间
来源：http://mf.shxzukj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kv.shxzskj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yw.huixiangedu.cn

JS:   new Date();  Date.now()
来源：http://vm.nszjky.cn

TS:   new Date();  Date.now()
来源：http://nb.9csxet.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://sc.huixinmuqiang.cn

Go:   time.Now()
来源：http://xz.szxytkj.cn

Ruby: Time.now
来源：http://kj.shxzskj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gd.bjjhwx.cn

[J02] 格式化输出
来源：http://gi.huanxung.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yb.newstarts.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qw.bjjhwx.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ex.bookmarksfly.cn

TS:   d.toISOString()
来源：http://rk.bookmarksfly.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mm.nicolike.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xc.chemitech.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://se.chemitech.net.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ua.bookmarksfly.cn

[J03] 字符串解析为日期
来源：http://xd.yuntaijiaju.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mi.szsharing.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vb.hahajie.cn

JS:   new Date("2024-01-02")
来源：http://vh.hahajie.cn

TS:   new Date("2024-01-02")
来源：http://ei.haigaiapp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pb.hnjuh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zy.jianghongdianzi.cn

Ruby: Date.parse("2024-01-02")
来源：http://rr.haigaiapp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fc.nszjky.cn

[J04] 时间戳与日期互转
来源：http://ps.colortex.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wu.newstarts.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://li.yuntaijiaju.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wj.shxzukj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://an.yuexingan06.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mu.bjjhwx.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ab.jianghongdianzi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bz.jctech888.com.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vp.wgjwhj.cn

[J05] 时间加减（加 7 天）
来源：http://es.haigaiapp.cn

Py:   now + timedelta(days=7)
来源：http://ah.bookmarksfly.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qz.gzmigu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qh.nszjky.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yg.panjiajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://zl.newstarts.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dg.521024.cn

Ruby: Time.now + 7 * 86400
来源：http://vv.haigaiapp.cn

C#:   DateTime.Now.AddDays(7)
来源：http://mp.newstarts.cn

[J06] 计算两时间之差
来源：http://ps.jctech888.com.cn

Py:   (end - start).total_seconds()
来源：http://rv.9csxet.cn

PHP:  $end->diff($start)->days;
来源：http://hf.nicolike.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fi.asd995.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ou.nicolike.cn

Java: Duration.between(start, end).toSeconds()
来源：http://pk.shxzskj.cn

Go:   end.Sub(start).Hours()
来源：http://sd.shxzskj.cn

Ruby: end - start                 # 返回秒数
来源：http://xx.jianghongdianzi.cn

C#:   (end - start).TotalSeconds
来源：http://js.wgjwhj.cn

[J07] 比较两个日期
来源：http://zn.szxytkj.cn

Py:   d1 < d2;  d1 == d2
来源：http://vp.haigaiapp.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sm.9csxet.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vb.521024.cn

TS:   d1.getTime() < d2.getTime()
来源：http://pi.colortex.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xk.panjiajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://eo.hahajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kn.colortex.cn

C#:   d1 < d2;  d1 == d2
来源：http://vj.jctech888.com.cn

[J08] 提取年月日与星期
来源：http://du.haigaiapp.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ty.jctech888.com.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hs.huixiangedu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ha.nszjky.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bs.hahajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wg.shtwfgs.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ga.yuntaijiaju.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ns.shtwfgs.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ws.bjjhwx.cn

[J09] 时区处理
来源：http://hn.muxihuayi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hl.huixiangedu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pz.bjjhwx.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://da.bjjhwx.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qr.huixinmuqiang.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gz.panjiajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ss.panjiajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wp.jctech888.com.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wj.9csxet.cn

[J10] 取今天 / 本月第一天
来源：http://bw.bookmarksfly.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kh.521024.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ey.hahajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vj.yuexingan06.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://am.chemitech.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hq.colortex.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qv.shxzskj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qw.muxihuayi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pv.9csxet.cn

================================================================================
来源：http://jk.9csxet.cn

K. JSON 与序列化
来源：http://tt.hahajie.cn

================================================================================
来源：http://ws.szsharing.cn

[K01] 对象转 JSON 字符串
来源：http://pb.colortex.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jc.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dj.hnjuh.cn

JS:   JSON.stringify(obj)
来源：http://qs.szxytkj.cn

TS:   JSON.stringify(obj)
来源：http://io.newstarts.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jq.hnjuh.cn

Go:   json.Marshal(obj)
来源：http://ku.bookmarksfly.cn

Ruby: obj.to_json                                     // require "json"
来源：http://sv.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zu.9csxet.cn

[K02] JSON 字符串转对象
来源：http://ka.szxytkj.cn

Py:   json.loads(s)
来源：http://yo.wgjwhj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://al.muxihuayi.cn

JS:   JSON.parse(s)
来源：http://kq.hahajie.cn

TS:   JSON.parse(s)
来源：http://ch.huixinmuqiang.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fw.szxytkj.cn

Go:   json.Unmarshal(data, &v)
来源：http://mc.jianghongdianzi.cn

Ruby: JSON.parse(s)
来源：http://cn.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pt.wgjwhj.cn

[K03] JSON 美化输出（带缩进）
来源：http://kq.huanxung.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zz.shxzskj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://do.bookmarksfly.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://je.gzmigu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://re.huanxung.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xu.haigaiapp.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://md.haigaiapp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ba.shxzukj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nf.bookmarksfly.cn

[K04] 读取 JSON 文件
来源：http://bt.huanxung.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mb.colortex.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fi.wgjwhj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uw.yuexingan06.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tl.jianghongdianzi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xy.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bi.lnxyls.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fl.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rr.bookmarksfly.cn

[K05] 深拷贝对象
来源：http://lr.hahajie.cn

Py:   copy.deepcopy(obj)
来源：http://yp.9csxet.cn

PHP:  unserialize(serialize($obj));
来源：http://af.huixiangedu.cn

JS:   structuredClone(obj)
来源：http://pj.szsharing.cn

TS:   structuredClone(obj)
来源：http://au.shxzskj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qy.szxytkj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gn.huixiangedu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wc.huixiangedu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lq.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://xy.nicolike.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bo.hahajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zv.shtwfgs.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bb.9csxet.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uy.newstarts.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fa.521024.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xh.szxytkj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://at.yuntaijiaju.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kc.hnjuh.cn

[K07] 进制转换
来源：http://tc.newstarts.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yf.lnxyls.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tm.shxzskj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://al.jianghongdianzi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ie.9csxet.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tw.yuntaijiaju.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xt.lnxyls.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rt.nicolike.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pg.521024.cn

[K08] 二进制序列化（非 JSON）
来源：http://zf.jianghongdianzi.cn

Py:   pickle.dumps(obj)
来源：http://bv.shtwfgs.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lw.nszjky.cn

JS:   v8.serialize(obj)        // Node
来源：http://sd.hahajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://ox.9csxet.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wt.jianghongdianzi.cn

Go:   encoding/gob
来源：http://vx.shtwfgs.cn

Ruby: Marshal.dump(obj)
来源：http://to.yuntaijiaju.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uz.shxzskj.cn

================================================================================
来源：http://zv.huixinmuqiang.cn

L. 网络请求
来源：http://dv.muxihuayi.cn

================================================================================
来源：http://og.hahajie.cn

[L01] 发送 GET 请求
来源：http://ij.hahajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bt.nicolike.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wf.jctech888.com.cn

JS:   await fetch(url)
来源：http://ln.panjiajie.cn

TS:   await fetch(url)
来源：http://vt.colortex.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://is.huixinmuqiang.cn

Go:   resp, err := http.Get(url)
来源：http://at.haigaiapp.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dl.huanxung.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ap.bookmarksfly.cn

[L02] 发送 POST JSON
来源：http://oo.bookmarksfly.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zn.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hl.huanxung.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fw.gzmigu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ya.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ii.asd995.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pd.wgjwhj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wc.jianghongdianzi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rt.haigaiapp.cn

[L03] 设置自定义请求头
来源：http://gi.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bz.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yn.gzmigu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qi.huixiangedu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jd.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://aj.hnjuh.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bu.yuntaijiaju.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://js.shxzskj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qu.bookmarksfly.cn

[L04] 设置超时
来源：http://yt.yuntaijiaju.cn

Py:   requests.get(url, timeout=5)
来源：http://ik.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kr.chemitech.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oh.gzmigu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gp.jctech888.com.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pb.huixiangedu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pe.bjjhwx.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vl.hnjuh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sb.yuntaijiaju.cn

[L05] 上传文件（multipart）
来源：http://dq.chemitech.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dj.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fr.huixinmuqiang.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nx.wgjwhj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wh.haigaiapp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pg.gzmigu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://oc.haigaiapp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://di.9csxet.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yn.jianghongdianzi.cn

[L06] 解析响应为 JSON
来源：http://uk.521024.cn

Py:   resp.json()
来源：http://te.shxzskj.cn

PHP:  json_decode($body, true);
来源：http://fm.huanxung.cn

JS:   await resp.json()
来源：http://oq.shxzukj.cn

TS:   await resp.json()
来源：http://le.colortex.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://km.jctech888.com.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://iu.jctech888.com.cn

Ruby: JSON.parse(resp.body)
来源：http://it.yuexingan06.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ra.newstarts.cn

[L07] 处理 HTTP 状态码
来源：http://tk.asd995.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kh.szsharing.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vi.jianghongdianzi.cn

JS:   resp.ok;  resp.status
来源：http://bx.huixiangedu.cn

TS:   resp.ok;  resp.status
来源：http://hj.521024.cn

Java: resp.statusCode()
来源：http://xp.muxihuayi.cn

Go:   resp.StatusCode
来源：http://dt.521024.cn

Ruby: resp.code.to_i
来源：http://gs.szxytkj.cn

C#:   (int)resp.StatusCode
来源：http://vh.muxihuayi.cn

[L08] 并发请求多个地址
来源：http://zm.huixinmuqiang.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yq.colortex.cn

PHP:  curl_multi_init() 系列
来源：http://dc.hahajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ve.shxzukj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ps.hahajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vc.shxzukj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fw.newstarts.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qp.jctech888.com.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tm.jctech888.com.cn

================================================================================
来源：http://iq.yuntaijiaju.cn

M. 命令行 / 进程 / 环境
来源：http://hg.bookmarksfly.cn

================================================================================
来源：http://tl.lnxyls.cn

[M01] 读取命令行参数
来源：http://sa.asd995.cn

Py:   sys.argv[1:]
来源：http://zh.bookmarksfly.cn

PHP:  $argv;  $argc;
来源：http://zs.shtwfgs.cn

JS:   process.argv.slice(2)
来源：http://wo.yuntaijiaju.cn

TS:   process.argv.slice(2)
来源：http://is.asd995.cn

Java: args 数组（main 方法参数）
来源：http://us.yuexingan06.cn

Go:   os.Args[1:]
来源：http://yk.hnjuh.cn

Ruby: ARGV
来源：http://az.chemitech.net.cn

C#:   args 数组（Main 方法参数）
来源：http://vu.hahajie.cn

[M02] 读取环境变量
来源：http://ck.yuntaijiaju.cn

Py:   os.environ.get("HOME")
来源：http://uv.hnjuh.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fe.jianghongdianzi.cn

JS:   process.env.HOME
来源：http://fh.szxytkj.cn

TS:   process.env.HOME
来源：http://gf.gzmigu.cn

Java: System.getenv("HOME")
来源：http://me.lnxyls.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qv.hnjuh.cn

Ruby: ENV["HOME"]
来源：http://qb.9csxet.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ke.panjiajie.cn

[M03] 执行外部命令
来源：http://mu.muxihuayi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zy.9csxet.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tz.huixinmuqiang.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://oe.lnxyls.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://hr.nicolike.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bt.hahajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xw.nicolike.cn

Ruby: system("ls -l");  `ls -l`
来源：http://iq.jianghongdianzi.cn

C#:   Process.Start("ls", "-l");
来源：http://ua.shxzukj.cn

[M04] 获取当前工作目录
来源：http://oe.521024.cn

Py:   os.getcwd()
来源：http://wt.huixiangedu.cn

PHP:  getcwd();
来源：http://ml.bookmarksfly.cn

JS:   process.cwd()
来源：http://qr.nicolike.cn

TS:   process.cwd()
来源：http://xa.nszjky.cn

Java: Path.of("").toAbsolutePath()
来源：http://nn.colortex.cn

Go:   os.Getwd()
来源：http://bt.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://to.panjiajie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ah.9csxet.cn

[M05] 设置退出码
来源：http://wn.9csxet.cn

Py:   sys.exit(1)
来源：http://ot.panjiajie.cn

PHP:  exit(1);
来源：http://xi.yuexingan06.cn


<!-- 参考信息 -->