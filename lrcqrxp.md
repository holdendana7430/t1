代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://it.wgjwhj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://by.huixiangedu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fj.jianghongdianzi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bk.muxihuayi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ii.hahajie.cn

[I07] 忽略大小写与多行模式
来源：http://bx.panjiajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://va.yuntaijiaju.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yu.bookmarksfly.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vw.haigaiapp.cn

TS:   /error/gim
来源：http://ui.colortex.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qe.haigaiapp.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rb.colortex.cn

Ruby: s.scan(/error/i)
来源：http://wp.lnxyls.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ks.yuexingan06.cn

[I08] 贪婪与非贪婪匹配
来源：http://vm.hahajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yj.9csxet.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://aw.newstarts.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mn.shtwfgs.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://le.huixiangedu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://mz.shxzukj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jy.nicolike.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dw.hahajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://aa.chemitech.net.cn

================================================================================
来源：http://fc.huixiangedu.cn

J. 日期与时间
来源：http://rz.shxzukj.cn

================================================================================
来源：http://vg.jctech888.com.cn

[J01] 获取当前时间
来源：http://ps.hnjuh.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pr.yuexingan06.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://og.jianghongdianzi.cn

JS:   new Date();  Date.now()
来源：http://hv.shtwfgs.cn

TS:   new Date();  Date.now()
来源：http://rp.yuntaijiaju.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pk.shxzskj.cn

Go:   time.Now()
来源：http://lt.521024.cn

Ruby: Time.now
来源：http://up.panjiajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yo.panjiajie.cn

[J02] 格式化输出
来源：http://ij.hahajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://td.hnjuh.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hw.asd995.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dl.muxihuayi.cn

TS:   d.toISOString()
来源：http://bu.bjjhwx.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qe.wgjwhj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://di.huixinmuqiang.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qu.521024.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sr.asd995.cn

[J03] 字符串解析为日期
来源：http://mr.nszjky.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://th.shxzukj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://et.nszjky.cn

JS:   new Date("2024-01-02")
来源：http://oe.hahajie.cn

TS:   new Date("2024-01-02")
来源：http://mr.jianghongdianzi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://kk.hnjuh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zq.muxihuayi.cn

Ruby: Date.parse("2024-01-02")
来源：http://oc.muxihuayi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vw.shxzukj.cn

[J04] 时间戳与日期互转
来源：http://ug.haigaiapp.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sv.szxytkj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qh.newstarts.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fi.szxytkj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wy.wgjwhj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ys.haigaiapp.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nv.gzmigu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fs.nszjky.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mp.yuntaijiaju.cn

[J05] 时间加减（加 7 天）
来源：http://ov.huanxung.cn

Py:   now + timedelta(days=7)
来源：http://bv.521024.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lk.shxzskj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bs.muxihuayi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ju.muxihuayi.cn

Java: LocalDate.now().plusDays(7)
来源：http://tu.shxzskj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wm.szsharing.cn

Ruby: Time.now + 7 * 86400
来源：http://qm.yuntaijiaju.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gq.shxzskj.cn

[J06] 计算两时间之差
来源：http://vt.asd995.cn

Py:   (end - start).total_seconds()
来源：http://xx.szsharing.cn

PHP:  $end->diff($start)->days;
来源：http://er.asd995.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dp.muxihuayi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zr.colortex.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jv.jianghongdianzi.cn

Go:   end.Sub(start).Hours()
来源：http://gx.shxzskj.cn

Ruby: end - start                 # 返回秒数
来源：http://xo.gzmigu.cn

C#:   (end - start).TotalSeconds
来源：http://di.shxzskj.cn

[J07] 比较两个日期
来源：http://ot.huixinmuqiang.cn

Py:   d1 < d2;  d1 == d2
来源：http://ex.yuexingan06.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lv.nszjky.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vc.muxihuayi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://lb.jianghongdianzi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vd.huixinmuqiang.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tl.bjjhwx.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mh.shxzukj.cn

C#:   d1 < d2;  d1 == d2
来源：http://jt.panjiajie.cn

[J08] 提取年月日与星期
来源：http://zr.bjjhwx.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://if.haigaiapp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://io.yuexingan06.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fa.gzmigu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://il.nszjky.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wc.jctech888.com.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://oi.yuexingan06.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qy.jianghongdianzi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://an.jctech888.com.cn

[J09] 时区处理
来源：http://fs.nszjky.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mg.shtwfgs.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://by.colortex.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wp.shxzukj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mw.gzmigu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cz.szxytkj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bq.shtwfgs.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ai.huixiangedu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cs.panjiajie.cn

[J10] 取今天 / 本月第一天
来源：http://jx.hnjuh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://as.gzmigu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jp.huanxung.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wb.huanxung.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pl.muxihuayi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yu.szsharing.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cz.yuntaijiaju.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mf.gzmigu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ty.huanxung.cn

================================================================================
来源：http://fw.9csxet.cn

K. JSON 与序列化
来源：http://bt.nicolike.cn

================================================================================
来源：http://wn.haigaiapp.cn

[K01] 对象转 JSON 字符串
来源：http://ih.yuexingan06.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mf.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kh.asd995.cn

JS:   JSON.stringify(obj)
来源：http://mk.lnxyls.cn

TS:   JSON.stringify(obj)
来源：http://df.shxzukj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mk.colortex.cn

Go:   json.Marshal(obj)
来源：http://gk.nszjky.cn

Ruby: obj.to_json                                     // require "json"
来源：http://db.nicolike.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://iu.muxihuayi.cn

[K02] JSON 字符串转对象
来源：http://yn.colortex.cn

Py:   json.loads(s)
来源：http://kv.huixinmuqiang.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bi.bookmarksfly.cn

JS:   JSON.parse(s)
来源：http://tv.9csxet.cn

TS:   JSON.parse(s)
来源：http://sp.yuexingan06.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mc.jctech888.com.cn

Go:   json.Unmarshal(data, &v)
来源：http://pq.nicolike.cn

Ruby: JSON.parse(s)
来源：http://nq.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fp.jianghongdianzi.cn

[K03] JSON 美化输出（带缩进）
来源：http://fb.lnxyls.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ii.hahajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ie.szsharing.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dx.nszjky.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://li.colortex.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://it.jianghongdianzi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fk.shxzukj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ek.nszjky.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bq.shtwfgs.cn

[K04] 读取 JSON 文件
来源：http://vv.chemitech.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ee.wgjwhj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cj.nszjky.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oy.huixiangedu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mu.jctech888.com.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uv.9csxet.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ju.jianghongdianzi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rk.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xx.521024.cn

[K05] 深拷贝对象
来源：http://fy.bookmarksfly.cn

Py:   copy.deepcopy(obj)
来源：http://po.shxzskj.cn

PHP:  unserialize(serialize($obj));
来源：http://jt.huixiangedu.cn

JS:   structuredClone(obj)
来源：http://jl.hnjuh.cn

TS:   structuredClone(obj)
来源：http://rr.newstarts.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://uw.huixiangedu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://py.jctech888.com.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://co.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ke.huanxung.cn

[K06] 解析 URL 查询串
来源：http://vg.nicolike.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://be.szsharing.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sz.asd995.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://op.huixiangedu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cm.huixiangedu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://iy.huixiangedu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fa.jianghongdianzi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fr.chemitech.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rz.9csxet.cn

[K07] 进制转换
来源：http://dr.nszjky.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ov.521024.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ok.colortex.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ee.szsharing.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pp.haigaiapp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://se.newstarts.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ou.yuexingan06.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xf.colortex.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://up.lnxyls.cn

[K08] 二进制序列化（非 JSON）
来源：http://my.szsharing.cn

Py:   pickle.dumps(obj)
来源：http://xt.panjiajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://aq.szxytkj.cn

JS:   v8.serialize(obj)        // Node
来源：http://cf.muxihuayi.cn

TS:   v8.serialize(obj)        // Node
来源：http://yg.shxzskj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xh.521024.cn

Go:   encoding/gob
来源：http://bc.szxytkj.cn

Ruby: Marshal.dump(obj)
来源：http://iy.jctech888.com.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rz.huixiangedu.cn

================================================================================
来源：http://ug.chemitech.net.cn

L. 网络请求
来源：http://bz.haigaiapp.cn

================================================================================
来源：http://lf.haigaiapp.cn

[L01] 发送 GET 请求
来源：http://wj.bjjhwx.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mx.bjjhwx.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bf.521024.cn

JS:   await fetch(url)
来源：http://ob.hahajie.cn

TS:   await fetch(url)
来源：http://ks.huanxung.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sp.chemitech.net.cn

Go:   resp, err := http.Get(url)
来源：http://xs.gzmigu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ht.colortex.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rl.huixinmuqiang.cn

[L02] 发送 POST JSON
来源：http://ak.shxzskj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rw.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dd.asd995.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iq.huixiangedu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sr.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xz.chemitech.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gs.colortex.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ed.9csxet.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pn.521024.cn

[L03] 设置自定义请求头
来源：http://uo.panjiajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vs.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nc.panjiajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lg.nicolike.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xf.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tu.521024.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mc.muxihuayi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tb.shxzskj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sf.szxytkj.cn

[L04] 设置超时
来源：http://ja.huanxung.cn

Py:   requests.get(url, timeout=5)
来源：http://hg.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vo.shxzukj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zp.newstarts.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cr.shxzukj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bs.huixiangedu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ht.newstarts.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hu.newstarts.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ns.shtwfgs.cn

[L05] 上传文件（multipart）
来源：http://hu.huixinmuqiang.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fi.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vc.asd995.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qb.huanxung.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gu.lnxyls.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ew.nszjky.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fd.colortex.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ul.yuntaijiaju.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ld.muxihuayi.cn

[L06] 解析响应为 JSON
来源：http://cp.jctech888.com.cn

Py:   resp.json()
来源：http://rs.szsharing.cn

PHP:  json_decode($body, true);
来源：http://qu.shxzskj.cn

JS:   await resp.json()
来源：http://bw.haigaiapp.cn

TS:   await resp.json()
来源：http://gv.shtwfgs.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qr.jianghongdianzi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ps.hahajie.cn

Ruby: JSON.parse(resp.body)
来源：http://wj.jianghongdianzi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ms.shxzskj.cn

[L07] 处理 HTTP 状态码
来源：http://cg.huixinmuqiang.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fy.shtwfgs.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nw.hnjuh.cn

JS:   resp.ok;  resp.status
来源：http://ey.9csxet.cn

TS:   resp.ok;  resp.status
来源：http://sm.jctech888.com.cn

Java: resp.statusCode()
来源：http://qj.521024.cn

Go:   resp.StatusCode
来源：http://xz.nicolike.cn

Ruby: resp.code.to_i
来源：http://ea.haigaiapp.cn

C#:   (int)resp.StatusCode
来源：http://es.jctech888.com.cn

[L08] 并发请求多个地址
来源：http://vg.yuntaijiaju.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yy.huixinmuqiang.cn

PHP:  curl_multi_init() 系列
来源：http://ni.gzmigu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://io.asd995.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yz.9csxet.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xg.huanxung.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ws.lnxyls.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ys.nszjky.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://li.shtwfgs.cn

================================================================================
来源：http://ah.9csxet.cn

M. 命令行 / 进程 / 环境
来源：http://vp.colortex.cn

================================================================================
来源：http://py.nszjky.cn

[M01] 读取命令行参数
来源：http://un.521024.cn

Py:   sys.argv[1:]
来源：http://if.nszjky.cn

PHP:  $argv;  $argc;
来源：http://nk.yuexingan06.cn

JS:   process.argv.slice(2)
来源：http://gm.haigaiapp.cn

TS:   process.argv.slice(2)
来源：http://sj.huanxung.cn

Java: args 数组（main 方法参数）
来源：http://ul.nszjky.cn

Go:   os.Args[1:]
来源：http://en.shxzukj.cn

Ruby: ARGV
来源：http://gk.hnjuh.cn

C#:   args 数组（Main 方法参数）
来源：http://na.bookmarksfly.cn

[M02] 读取环境变量
来源：http://ya.jianghongdianzi.cn

Py:   os.environ.get("HOME")
来源：http://dl.521024.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://aq.shtwfgs.cn

JS:   process.env.HOME
来源：http://tw.haigaiapp.cn

TS:   process.env.HOME
来源：http://gi.yuexingan06.cn

Java: System.getenv("HOME")
来源：http://lo.shtwfgs.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ha.huanxung.cn

Ruby: ENV["HOME"]
来源：http://nu.huixinmuqiang.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nu.huixiangedu.cn

[M03] 执行外部命令
来源：http://ps.bjjhwx.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vg.nicolike.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://li.huanxung.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://cu.chemitech.net.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://eq.gzmigu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qr.szxytkj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://rp.shxzukj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://lo.haigaiapp.cn

C#:   Process.Start("ls", "-l");
来源：http://lr.jctech888.com.cn

[M04] 获取当前工作目录
来源：http://ca.nicolike.cn

Py:   os.getcwd()
来源：http://ug.yuexingan06.cn

PHP:  getcwd();
来源：http://zb.szxytkj.cn

JS:   process.cwd()
来源：http://hd.hnjuh.cn


<!-- 参考信息 -->