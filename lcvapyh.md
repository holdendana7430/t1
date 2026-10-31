代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kg.huixiangedu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nm.szxytkj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ou.wgjwhj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ad.yuexingan06.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nx.colortex.cn

[I07] 忽略大小写与多行模式
来源：http://ks.hahajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fs.muxihuayi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xl.jianghongdianzi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qo.chemitech.net.cn

TS:   /error/gim
来源：http://ba.szsharing.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://by.bjjhwx.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://oy.shxzskj.cn

Ruby: s.scan(/error/i)
来源：http://oj.shtwfgs.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://km.colortex.cn

[I08] 贪婪与非贪婪匹配
来源：http://gw.gzmigu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jr.asd995.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ay.shtwfgs.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cp.yuexingan06.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tr.szxytkj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fg.shxzskj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lk.newstarts.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rn.hnjuh.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zm.yuntaijiaju.cn

================================================================================
来源：http://di.hahajie.cn

J. 日期与时间
来源：http://xo.yuntaijiaju.cn

================================================================================
来源：http://zx.haigaiapp.cn

[J01] 获取当前时间
来源：http://uw.hnjuh.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://of.panjiajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ho.9csxet.cn

JS:   new Date();  Date.now()
来源：http://td.huanxung.cn

TS:   new Date();  Date.now()
来源：http://yc.newstarts.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mi.shxzskj.cn

Go:   time.Now()
来源：http://zt.chemitech.net.cn

Ruby: Time.now
来源：http://hb.yuexingan06.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jo.9csxet.cn

[J02] 格式化输出
来源：http://ug.nicolike.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://se.lnxyls.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gf.shxzskj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ob.521024.cn

TS:   d.toISOString()
来源：http://sm.nicolike.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fp.bjjhwx.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vt.9csxet.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uy.wgjwhj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gw.muxihuayi.cn

[J03] 字符串解析为日期
来源：http://ly.asd995.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xa.yuntaijiaju.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ys.muxihuayi.cn

JS:   new Date("2024-01-02")
来源：http://ui.yuexingan06.cn

TS:   new Date("2024-01-02")
来源：http://ef.bjjhwx.cn

Java: LocalDate.parse("2024-01-02")
来源：http://af.asd995.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tp.chemitech.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://tg.szsharing.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uz.jctech888.com.cn

[J04] 时间戳与日期互转
来源：http://xh.nszjky.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dc.shxzskj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pe.bjjhwx.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pg.szsharing.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://no.nicolike.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lz.chemitech.net.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ly.hahajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tv.szxytkj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dt.bookmarksfly.cn

[J05] 时间加减（加 7 天）
来源：http://xf.szsharing.cn

Py:   now + timedelta(days=7)
来源：http://ft.bookmarksfly.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zr.bookmarksfly.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://de.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wr.bjjhwx.cn

Java: LocalDate.now().plusDays(7)
来源：http://rb.szxytkj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ac.shxzukj.cn

Ruby: Time.now + 7 * 86400
来源：http://uo.szxytkj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://dj.muxihuayi.cn

[J06] 计算两时间之差
来源：http://cf.muxihuayi.cn

Py:   (end - start).total_seconds()
来源：http://mm.nicolike.cn

PHP:  $end->diff($start)->days;
来源：http://wa.panjiajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fu.muxihuayi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lu.hnjuh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://iy.szxytkj.cn

Go:   end.Sub(start).Hours()
来源：http://ym.lnxyls.cn

Ruby: end - start                 # 返回秒数
来源：http://sl.haigaiapp.cn

C#:   (end - start).TotalSeconds
来源：http://tb.huixiangedu.cn

[J07] 比较两个日期
来源：http://tp.huixinmuqiang.cn

Py:   d1 < d2;  d1 == d2
来源：http://ws.colortex.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://er.muxihuayi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tk.gzmigu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://pn.9csxet.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xq.hahajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cm.lnxyls.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cr.9csxet.cn

C#:   d1 < d2;  d1 == d2
来源：http://qn.gzmigu.cn

[J08] 提取年月日与星期
来源：http://ux.shtwfgs.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lr.huixinmuqiang.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fs.hahajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://im.hahajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ka.shxzukj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qp.lnxyls.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://or.bookmarksfly.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ah.chemitech.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mt.wgjwhj.cn

[J09] 时区处理
来源：http://xo.huanxung.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wu.bookmarksfly.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://la.shxzukj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jr.jctech888.com.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ri.newstarts.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rj.colortex.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xc.9csxet.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://oc.panjiajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gz.szxytkj.cn

[J10] 取今天 / 本月第一天
来源：http://qk.jianghongdianzi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://uo.gzmigu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ze.chemitech.net.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rk.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gb.jianghongdianzi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sg.nicolike.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jf.yuexingan06.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bq.szxytkj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lx.chemitech.net.cn

================================================================================
来源：http://yp.chemitech.net.cn

K. JSON 与序列化
来源：http://mc.jianghongdianzi.cn

================================================================================
来源：http://fc.jctech888.com.cn

[K01] 对象转 JSON 字符串
来源：http://ap.shtwfgs.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gq.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://id.huixiangedu.cn

JS:   JSON.stringify(obj)
来源：http://tm.shtwfgs.cn

TS:   JSON.stringify(obj)
来源：http://dx.nicolike.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wt.asd995.cn

Go:   json.Marshal(obj)
来源：http://vg.bjjhwx.cn

Ruby: obj.to_json                                     // require "json"
来源：http://do.gzmigu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zj.hahajie.cn

[K02] JSON 字符串转对象
来源：http://ko.szxytkj.cn

Py:   json.loads(s)
来源：http://yp.muxihuayi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jl.muxihuayi.cn

JS:   JSON.parse(s)
来源：http://yo.yuexingan06.cn

TS:   JSON.parse(s)
来源：http://vn.colortex.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dg.newstarts.cn

Go:   json.Unmarshal(data, &v)
来源：http://en.hnjuh.cn

Ruby: JSON.parse(s)
来源：http://no.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uz.shxzskj.cn

[K03] JSON 美化输出（带缩进）
来源：http://re.wgjwhj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ti.szsharing.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hi.huixiangedu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dy.yuexingan06.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://dc.9csxet.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zp.gzmigu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qd.bookmarksfly.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qz.shxzskj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bh.chemitech.net.cn

[K04] 读取 JSON 文件
来源：http://fj.nszjky.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fn.shtwfgs.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tr.huanxung.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gg.hahajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ql.szsharing.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ir.nicolike.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hq.jctech888.com.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hv.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://js.szxytkj.cn

[K05] 深拷贝对象
来源：http://al.newstarts.cn

Py:   copy.deepcopy(obj)
来源：http://oi.huixiangedu.cn

PHP:  unserialize(serialize($obj));
来源：http://pe.wgjwhj.cn

JS:   structuredClone(obj)
来源：http://qa.bookmarksfly.cn

TS:   structuredClone(obj)
来源：http://kz.newstarts.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bq.muxihuayi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rr.shxzskj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ox.lnxyls.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://kp.asd995.cn

[K06] 解析 URL 查询串
来源：http://xm.bookmarksfly.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ri.muxihuayi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ga.bookmarksfly.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bz.panjiajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ow.huanxung.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vs.szxytkj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://kr.wgjwhj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ln.521024.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pz.wgjwhj.cn

[K07] 进制转换
来源：http://zz.newstarts.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yy.lnxyls.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ze.newstarts.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qa.szsharing.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lg.shtwfgs.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fj.lnxyls.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zf.chemitech.net.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oa.jianghongdianzi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dt.huanxung.cn

[K08] 二进制序列化（非 JSON）
来源：http://by.hahajie.cn

Py:   pickle.dumps(obj)
来源：http://cp.yuntaijiaju.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://da.bjjhwx.cn

JS:   v8.serialize(obj)        // Node
来源：http://cb.9csxet.cn

TS:   v8.serialize(obj)        // Node
来源：http://si.521024.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://il.hnjuh.cn

Go:   encoding/gob
来源：http://af.panjiajie.cn

Ruby: Marshal.dump(obj)
来源：http://zh.yuexingan06.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://si.nicolike.cn

================================================================================
来源：http://lm.hnjuh.cn

L. 网络请求
来源：http://xh.shtwfgs.cn

================================================================================
来源：http://dg.jianghongdianzi.cn

[L01] 发送 GET 请求
来源：http://aq.nicolike.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yw.jianghongdianzi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://am.haigaiapp.cn

JS:   await fetch(url)
来源：http://dv.yuntaijiaju.cn

TS:   await fetch(url)
来源：http://ca.9csxet.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ga.asd995.cn

Go:   resp, err := http.Get(url)
来源：http://su.asd995.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://eo.lnxyls.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kq.newstarts.cn

[L02] 发送 POST JSON
来源：http://ko.chemitech.net.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gq.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jl.wgjwhj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://to.newstarts.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gq.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uo.colortex.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qb.szxytkj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vu.szxytkj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mg.wgjwhj.cn

[L03] 设置自定义请求头
来源：http://md.9csxet.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ku.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ro.shxzukj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://im.gzmigu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xc.asd995.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ot.nszjky.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jb.muxihuayi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://km.panjiajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hs.huixiangedu.cn

[L04] 设置超时
来源：http://wo.newstarts.cn

Py:   requests.get(url, timeout=5)
来源：http://ol.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://oh.huixiangedu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kc.muxihuayi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jk.panjiajie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://od.wgjwhj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yd.gzmigu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://di.lnxyls.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rl.muxihuayi.cn

[L05] 上传文件（multipart）
来源：http://kl.shtwfgs.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dl.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://iz.wgjwhj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cu.shtwfgs.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lt.shtwfgs.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nv.shxzukj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xx.yuexingan06.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ek.shxzskj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rn.chemitech.net.cn

[L06] 解析响应为 JSON
来源：http://dk.hahajie.cn

Py:   resp.json()
来源：http://jq.shxzskj.cn

PHP:  json_decode($body, true);
来源：http://lj.huixinmuqiang.cn

JS:   await resp.json()
来源：http://vq.hahajie.cn

TS:   await resp.json()
来源：http://ia.huixiangedu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://aw.gzmigu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pk.lnxyls.cn

Ruby: JSON.parse(resp.body)
来源：http://ti.asd995.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wp.huixinmuqiang.cn

[L07] 处理 HTTP 状态码
来源：http://gt.hnjuh.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qz.huanxung.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sb.panjiajie.cn

JS:   resp.ok;  resp.status
来源：http://mt.nicolike.cn

TS:   resp.ok;  resp.status
来源：http://ly.huixinmuqiang.cn

Java: resp.statusCode()
来源：http://bu.521024.cn

Go:   resp.StatusCode
来源：http://zi.shxzukj.cn

Ruby: resp.code.to_i
来源：http://dw.panjiajie.cn

C#:   (int)resp.StatusCode
来源：http://ph.nicolike.cn

[L08] 并发请求多个地址
来源：http://aw.9csxet.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gl.shxzskj.cn

PHP:  curl_multi_init() 系列
来源：http://cu.shxzukj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rm.shtwfgs.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nn.haigaiapp.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://au.jctech888.com.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.bjjhwx.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zk.gzmigu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://to.lnxyls.cn

================================================================================
来源：http://lx.huixiangedu.cn

M. 命令行 / 进程 / 环境
来源：http://ep.shtwfgs.cn

================================================================================
来源：http://ji.521024.cn

[M01] 读取命令行参数
来源：http://wr.shtwfgs.cn

Py:   sys.argv[1:]
来源：http://ox.panjiajie.cn

PHP:  $argv;  $argc;
来源：http://mv.hnjuh.cn

JS:   process.argv.slice(2)
来源：http://yl.huixiangedu.cn

TS:   process.argv.slice(2)
来源：http://st.asd995.cn

Java: args 数组（main 方法参数）
来源：http://ih.521024.cn

Go:   os.Args[1:]
来源：http://zn.chemitech.net.cn

Ruby: ARGV
来源：http://pm.newstarts.cn

C#:   args 数组（Main 方法参数）
来源：http://mi.yuntaijiaju.cn

[M02] 读取环境变量
来源：http://nw.521024.cn

Py:   os.environ.get("HOME")
来源：http://gz.szxytkj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://be.yuntaijiaju.cn

JS:   process.env.HOME
来源：http://uf.wgjwhj.cn

TS:   process.env.HOME
来源：http://xk.asd995.cn

Java: System.getenv("HOME")
来源：http://jc.huixinmuqiang.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sr.nszjky.cn

Ruby: ENV["HOME"]
来源：http://ra.muxihuayi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oa.nicolike.cn

[M03] 执行外部命令
来源：http://og.asd995.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kb.haigaiapp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jm.shxzskj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ig.colortex.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://bq.newstarts.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://to.newstarts.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fz.shtwfgs.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gr.shtwfgs.cn

C#:   Process.Start("ls", "-l");
来源：http://ui.shxzskj.cn

[M04] 获取当前工作目录
来源：http://lw.shtwfgs.cn

Py:   os.getcwd()
来源：http://ep.nszjky.cn

PHP:  getcwd();
来源：http://wl.chemitech.net.cn

JS:   process.cwd()
来源：http://gc.asd995.cn


<!-- 参考信息 -->