代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qz.jianghongdianzi.cn

[I07] 忽略大小写与多行模式
来源：http://bq.9csxet.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://aq.yuexingan06.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jr.yuntaijiaju.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mq.jianghongdianzi.cn

TS:   /error/gim
来源：http://mc.asd995.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ja.hahajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qj.szxytkj.cn

Ruby: s.scan(/error/i)
来源：http://gy.huixiangedu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rj.wgjwhj.cn

[I08] 贪婪与非贪婪匹配
来源：http://sh.huanxung.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xf.newstarts.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zy.nszjky.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vs.9csxet.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cc.huixiangedu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://iy.szxytkj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://um.521024.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dq.huixinmuqiang.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://az.jctech888.com.cn

================================================================================
来源：http://vf.hnjuh.cn

J. 日期与时间
来源：http://pg.yuexingan06.cn

================================================================================
来源：http://sy.muxihuayi.cn

[J01] 获取当前时间
来源：http://ya.bjjhwx.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://uv.shxzukj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nj.huixiangedu.cn

JS:   new Date();  Date.now()
来源：http://ja.jctech888.com.cn

TS:   new Date();  Date.now()
来源：http://fs.nicolike.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ji.hnjuh.cn

Go:   time.Now()
来源：http://nw.muxihuayi.cn

Ruby: Time.now
来源：http://dc.shtwfgs.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vl.jianghongdianzi.cn

[J02] 格式化输出
来源：http://bv.gzmigu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bq.shtwfgs.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qr.shxzukj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ql.huixiangedu.cn

TS:   d.toISOString()
来源：http://fh.nszjky.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://io.9csxet.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ct.nszjky.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cz.szxytkj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tm.jctech888.com.cn

[J03] 字符串解析为日期
来源：http://yh.bookmarksfly.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hh.521024.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yr.9csxet.cn

JS:   new Date("2024-01-02")
来源：http://hn.haigaiapp.cn

TS:   new Date("2024-01-02")
来源：http://wm.bookmarksfly.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zs.huanxung.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kv.chemitech.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://az.nszjky.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xw.yuexingan06.cn

[J04] 时间戳与日期互转
来源：http://tm.521024.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ks.huixinmuqiang.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fs.huixinmuqiang.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ei.shxzskj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ur.shxzskj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gq.chemitech.net.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jn.newstarts.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sl.yuexingan06.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vo.wgjwhj.cn

[J05] 时间加减（加 7 天）
来源：http://xg.haigaiapp.cn

Py:   now + timedelta(days=7)
来源：http://nd.szsharing.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://dw.panjiajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://or.huixinmuqiang.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fp.newstarts.cn

Java: LocalDate.now().plusDays(7)
来源：http://sc.gzmigu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qe.colortex.cn

Ruby: Time.now + 7 * 86400
来源：http://pc.shtwfgs.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ym.haigaiapp.cn

[J06] 计算两时间之差
来源：http://vr.hnjuh.cn

Py:   (end - start).total_seconds()
来源：http://mw.hnjuh.cn

PHP:  $end->diff($start)->days;
来源：http://zw.bjjhwx.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cz.yuntaijiaju.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jd.jianghongdianzi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qy.shxzskj.cn

Go:   end.Sub(start).Hours()
来源：http://st.521024.cn

Ruby: end - start                 # 返回秒数
来源：http://me.yuexingan06.cn

C#:   (end - start).TotalSeconds
来源：http://tg.yuntaijiaju.cn

[J07] 比较两个日期
来源：http://xu.521024.cn

Py:   d1 < d2;  d1 == d2
来源：http://vs.lnxyls.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://oj.nicolike.cn

JS:   d1.getTime() < d2.getTime()
来源：http://dd.huanxung.cn

TS:   d1.getTime() < d2.getTime()
来源：http://br.shxzukj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yy.szsharing.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lq.shtwfgs.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bu.szxytkj.cn

C#:   d1 < d2;  d1 == d2
来源：http://zi.yuntaijiaju.cn

[J08] 提取年月日与星期
来源：http://tf.shxzukj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zf.gzmigu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qy.shxzskj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xw.huixiangedu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dj.hahajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://da.szsharing.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lw.jianghongdianzi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ii.yuntaijiaju.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://du.nszjky.cn

[J09] 时区处理
来源：http://lv.shxzskj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qt.huixiangedu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ip.szsharing.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://um.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bi.newstarts.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cw.haigaiapp.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tb.jctech888.com.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jf.shtwfgs.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yc.shtwfgs.cn

[J10] 取今天 / 本月第一天
来源：http://ut.wgjwhj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xw.9csxet.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hb.colortex.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kv.newstarts.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ek.yuexingan06.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qt.haigaiapp.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wa.chemitech.net.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sh.jctech888.com.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://eh.colortex.cn

================================================================================
来源：http://da.521024.cn

K. JSON 与序列化
来源：http://vz.lnxyls.cn

================================================================================
来源：http://xh.hahajie.cn

[K01] 对象转 JSON 字符串
来源：http://fl.bjjhwx.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jk.hahajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ze.haigaiapp.cn

JS:   JSON.stringify(obj)
来源：http://pp.muxihuayi.cn

TS:   JSON.stringify(obj)
来源：http://ew.yuexingan06.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://eu.panjiajie.cn

Go:   json.Marshal(obj)
来源：http://qu.yuntaijiaju.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rd.shxzskj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jq.shxzskj.cn

[K02] JSON 字符串转对象
来源：http://la.gzmigu.cn

Py:   json.loads(s)
来源：http://ap.nicolike.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://od.yuexingan06.cn

JS:   JSON.parse(s)
来源：http://ve.chemitech.net.cn

TS:   JSON.parse(s)
来源：http://ul.hahajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://aa.hahajie.cn

Go:   json.Unmarshal(data, &v)
来源：http://yj.yuntaijiaju.cn

Ruby: JSON.parse(s)
来源：http://an.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kn.nszjky.cn

[K03] JSON 美化输出（带缩进）
来源：http://nq.9csxet.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gw.asd995.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ll.yuntaijiaju.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://je.nszjky.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qx.asd995.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gn.muxihuayi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wg.hnjuh.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rr.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vb.nicolike.cn

[K04] 读取 JSON 文件
来源：http://iw.shtwfgs.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yk.hahajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://go.nicolike.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tt.bjjhwx.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jm.muxihuayi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wf.lnxyls.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hk.521024.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://tb.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://eo.jctech888.com.cn

[K05] 深拷贝对象
来源：http://ia.gzmigu.cn

Py:   copy.deepcopy(obj)
来源：http://kc.szxytkj.cn

PHP:  unserialize(serialize($obj));
来源：http://wx.newstarts.cn

JS:   structuredClone(obj)
来源：http://oy.hnjuh.cn

TS:   structuredClone(obj)
来源：http://yp.lnxyls.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tx.yuntaijiaju.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bh.lnxyls.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gv.huixiangedu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yo.shxzskj.cn

[K06] 解析 URL 查询串
来源：http://zv.szxytkj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sj.haigaiapp.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yb.hahajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bq.yuntaijiaju.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kq.wgjwhj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xk.shxzskj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://lz.shxzskj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lt.gzmigu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ra.hahajie.cn

[K07] 进制转换
来源：http://mz.yuexingan06.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://te.szxytkj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zl.yuntaijiaju.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rh.newstarts.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kj.yuntaijiaju.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wm.jctech888.com.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ub.huixiangedu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://iy.nicolike.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://st.gzmigu.cn

[K08] 二进制序列化（非 JSON）
来源：http://lo.hahajie.cn

Py:   pickle.dumps(obj)
来源：http://wo.hnjuh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://kt.lnxyls.cn

JS:   v8.serialize(obj)        // Node
来源：http://qb.szsharing.cn

TS:   v8.serialize(obj)        // Node
来源：http://mm.huixiangedu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dj.asd995.cn

Go:   encoding/gob
来源：http://ih.bookmarksfly.cn

Ruby: Marshal.dump(obj)
来源：http://fm.wgjwhj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://no.chemitech.net.cn

================================================================================
来源：http://su.asd995.cn

L. 网络请求
来源：http://vp.nszjky.cn

================================================================================
来源：http://xf.lnxyls.cn

[L01] 发送 GET 请求
来源：http://yo.jianghongdianzi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://iv.shtwfgs.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://re.yuntaijiaju.cn

JS:   await fetch(url)
来源：http://ht.521024.cn

TS:   await fetch(url)
来源：http://rw.jianghongdianzi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zr.yuexingan06.cn

Go:   resp, err := http.Get(url)
来源：http://tr.nszjky.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ev.bookmarksfly.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yp.szsharing.cn

[L02] 发送 POST JSON
来源：http://pi.muxihuayi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xl.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sw.yuntaijiaju.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gy.521024.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cf.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://oc.jctech888.com.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ee.huixiangedu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://em.huixinmuqiang.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dp.nszjky.cn

[L03] 设置自定义请求头
来源：http://eu.jctech888.com.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ov.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uc.hnjuh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tn.nszjky.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vt.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kc.shxzskj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bm.hahajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wc.muxihuayi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://td.521024.cn

[L04] 设置超时
来源：http://tv.colortex.cn

Py:   requests.get(url, timeout=5)
来源：http://vw.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uv.shtwfgs.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fi.yuexingan06.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qz.nszjky.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kp.9csxet.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kw.shxzskj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lm.lnxyls.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ho.yuexingan06.cn

[L05] 上传文件（multipart）
来源：http://hk.shxzukj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sp.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sb.huixinmuqiang.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ac.chemitech.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hm.asd995.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://en.huixiangedu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zy.haigaiapp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sj.nicolike.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yb.haigaiapp.cn

[L06] 解析响应为 JSON
来源：http://yq.wgjwhj.cn

Py:   resp.json()
来源：http://dp.colortex.cn

PHP:  json_decode($body, true);
来源：http://se.bookmarksfly.cn

JS:   await resp.json()
来源：http://bi.nszjky.cn

TS:   await resp.json()
来源：http://bf.huixiangedu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zp.shtwfgs.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yv.shxzukj.cn

Ruby: JSON.parse(resp.body)
来源：http://es.hahajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hb.szsharing.cn

[L07] 处理 HTTP 状态码
来源：http://vz.hahajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://on.colortex.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ib.nicolike.cn

JS:   resp.ok;  resp.status
来源：http://nn.chemitech.net.cn

TS:   resp.ok;  resp.status
来源：http://il.shxzskj.cn

Java: resp.statusCode()
来源：http://jx.jctech888.com.cn

Go:   resp.StatusCode
来源：http://hy.gzmigu.cn

Ruby: resp.code.to_i
来源：http://no.lnxyls.cn

C#:   (int)resp.StatusCode
来源：http://xq.gzmigu.cn

[L08] 并发请求多个地址
来源：http://ct.shxzukj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://oz.jctech888.com.cn

PHP:  curl_multi_init() 系列
来源：http://vt.wgjwhj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lx.muxihuayi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bq.huanxung.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://an.huanxung.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mq.jianghongdianzi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fk.yuntaijiaju.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nb.hnjuh.cn

================================================================================
来源：http://gc.chemitech.net.cn

M. 命令行 / 进程 / 环境
来源：http://ws.jctech888.com.cn

================================================================================
来源：http://cf.wgjwhj.cn

[M01] 读取命令行参数
来源：http://jd.huanxung.cn

Py:   sys.argv[1:]
来源：http://lr.chemitech.net.cn

PHP:  $argv;  $argc;
来源：http://mh.asd995.cn

JS:   process.argv.slice(2)
来源：http://hc.bjjhwx.cn

TS:   process.argv.slice(2)
来源：http://zx.panjiajie.cn

Java: args 数组（main 方法参数）
来源：http://rd.muxihuayi.cn

Go:   os.Args[1:]
来源：http://fo.wgjwhj.cn

Ruby: ARGV
来源：http://al.huixiangedu.cn

C#:   args 数组（Main 方法参数）
来源：http://vg.gzmigu.cn

[M02] 读取环境变量
来源：http://pu.gzmigu.cn

Py:   os.environ.get("HOME")
来源：http://bb.lnxyls.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kv.asd995.cn

JS:   process.env.HOME
来源：http://vf.shxzskj.cn

TS:   process.env.HOME
来源：http://hp.lnxyls.cn

Java: System.getenv("HOME")
来源：http://kc.huixinmuqiang.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ka.shxzskj.cn

Ruby: ENV["HOME"]
来源：http://ew.jctech888.com.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oj.szsharing.cn

[M03] 执行外部命令
来源：http://zn.yuexingan06.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cr.chemitech.net.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pv.chemitech.net.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://uj.panjiajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gy.huixinmuqiang.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://at.hahajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qy.szsharing.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ea.nicolike.cn

C#:   Process.Start("ls", "-l");
来源：http://fr.huanxung.cn

[M04] 获取当前工作目录
来源：http://hp.hahajie.cn

Py:   os.getcwd()
来源：http://bi.panjiajie.cn

PHP:  getcwd();
来源：http://ou.muxihuayi.cn

JS:   process.cwd()
来源：http://pj.bookmarksfly.cn

TS:   process.cwd()
来源：http://wd.gzmigu.cn

Java: Path.of("").toAbsolutePath()
来源：http://rm.yuexingan06.cn

Go:   os.Getwd()
来源：http://xw.panjiajie.cn

Ruby: Dir.pwd
来源：http://sd.colortex.cn


<!-- 参考信息 -->