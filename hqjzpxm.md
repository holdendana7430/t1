代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ct.jianghongdianzi.cn

[I07] 忽略大小写与多行模式
来源：http://fp.asd995.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hl.jianghongdianzi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bq.shxzskj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hf.yuntaijiaju.cn

TS:   /error/gim
来源：http://nf.asd995.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lx.szsharing.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cf.szxytkj.cn

Ruby: s.scan(/error/i)
来源：http://nq.colortex.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rl.asd995.cn

[I08] 贪婪与非贪婪匹配
来源：http://en.newstarts.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ce.521024.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ip.chemitech.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://od.jctech888.com.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://za.hahajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://pc.szsharing.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bo.nszjky.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dj.panjiajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fd.9csxet.cn

================================================================================
来源：http://eg.nicolike.cn

J. 日期与时间
来源：http://oq.huixiangedu.cn

================================================================================
来源：http://ho.521024.cn

[J01] 获取当前时间
来源：http://rf.muxihuayi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://oa.huanxung.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ef.nszjky.cn

JS:   new Date();  Date.now()
来源：http://mv.newstarts.cn

TS:   new Date();  Date.now()
来源：http://na.hahajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rf.9csxet.cn

Go:   time.Now()
来源：http://fs.shtwfgs.cn

Ruby: Time.now
来源：http://lh.asd995.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vl.colortex.cn

[J02] 格式化输出
来源：http://um.yuexingan06.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mu.asd995.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nn.newstarts.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ao.521024.cn

TS:   d.toISOString()
来源：http://jx.yuntaijiaju.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ex.szsharing.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rt.huixinmuqiang.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gy.yuntaijiaju.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://px.shxzukj.cn

[J03] 字符串解析为日期
来源：http://kn.huixiangedu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hm.shxzukj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ci.asd995.cn

JS:   new Date("2024-01-02")
来源：http://bd.gzmigu.cn

TS:   new Date("2024-01-02")
来源：http://es.shtwfgs.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rb.colortex.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zj.bookmarksfly.cn

Ruby: Date.parse("2024-01-02")
来源：http://xb.szxytkj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qm.asd995.cn

[J04] 时间戳与日期互转
来源：http://wd.yuntaijiaju.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zr.gzmigu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sw.newstarts.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ca.bookmarksfly.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ra.bjjhwx.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ez.nicolike.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bt.colortex.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rx.huixinmuqiang.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dn.wgjwhj.cn

[J05] 时间加减（加 7 天）
来源：http://oa.newstarts.cn

Py:   now + timedelta(days=7)
来源：http://bd.bjjhwx.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nt.9csxet.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qf.colortex.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dw.shtwfgs.cn

Java: LocalDate.now().plusDays(7)
来源：http://hz.huanxung.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ck.lnxyls.cn

Ruby: Time.now + 7 * 86400
来源：http://ai.huixinmuqiang.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wc.asd995.cn

[J06] 计算两时间之差
来源：http://hl.huixiangedu.cn

Py:   (end - start).total_seconds()
来源：http://zc.szsharing.cn

PHP:  $end->diff($start)->days;
来源：http://ey.szsharing.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uw.521024.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ye.chemitech.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://aw.hahajie.cn

Go:   end.Sub(start).Hours()
来源：http://xc.panjiajie.cn

Ruby: end - start                 # 返回秒数
来源：http://pu.asd995.cn

C#:   (end - start).TotalSeconds
来源：http://wk.gzmigu.cn

[J07] 比较两个日期
来源：http://vu.huixiangedu.cn

Py:   d1 < d2;  d1 == d2
来源：http://hl.shxzskj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ww.nszjky.cn

JS:   d1.getTime() < d2.getTime()
来源：http://sf.shtwfgs.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fe.huixinmuqiang.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ys.521024.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://um.asd995.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wm.huanxung.cn

C#:   d1 < d2;  d1 == d2
来源：http://em.huanxung.cn

[J08] 提取年月日与星期
来源：http://kf.bjjhwx.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xy.gzmigu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mk.szxytkj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cg.huixiangedu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vt.shxzskj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tr.huanxung.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://do.chemitech.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gv.wgjwhj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://om.szsharing.cn

[J09] 时区处理
来源：http://xg.asd995.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rx.panjiajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qg.asd995.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lh.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pp.wgjwhj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ub.haigaiapp.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ny.9csxet.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zc.jctech888.com.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ox.muxihuayi.cn

[J10] 取今天 / 本月第一天
来源：http://cg.shxzskj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rz.huixinmuqiang.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kz.huanxung.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mt.jctech888.com.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zg.yuexingan06.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ph.jctech888.com.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rd.lnxyls.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jr.yuexingan06.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ja.muxihuayi.cn

================================================================================
来源：http://rg.szsharing.cn

K. JSON 与序列化
来源：http://lj.szxytkj.cn

================================================================================
来源：http://hc.huixinmuqiang.cn

[K01] 对象转 JSON 字符串
来源：http://mf.gzmigu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gg.521024.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wq.lnxyls.cn

JS:   JSON.stringify(obj)
来源：http://sl.jianghongdianzi.cn

TS:   JSON.stringify(obj)
来源：http://mg.szsharing.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xl.shtwfgs.cn

Go:   json.Marshal(obj)
来源：http://ca.bookmarksfly.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wa.shxzukj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qx.yuntaijiaju.cn

[K02] JSON 字符串转对象
来源：http://hn.yuntaijiaju.cn

Py:   json.loads(s)
来源：http://ac.jianghongdianzi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dl.huixinmuqiang.cn

JS:   JSON.parse(s)
来源：http://kl.yuexingan06.cn

TS:   JSON.parse(s)
来源：http://pv.newstarts.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tm.jctech888.com.cn

Go:   json.Unmarshal(data, &v)
来源：http://pw.lnxyls.cn

Ruby: JSON.parse(s)
来源：http://td.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rl.szxytkj.cn

[K03] JSON 美化输出（带缩进）
来源：http://on.nszjky.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qi.szxytkj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://in.521024.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bh.szsharing.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bn.asd995.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ri.shxzukj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kd.lnxyls.cn

Ruby: JSON.pretty_generate(obj)
来源：http://uz.hahajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ce.hnjuh.cn

[K04] 读取 JSON 文件
来源：http://wk.nszjky.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jl.muxihuayi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://td.huixinmuqiang.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nk.szxytkj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ox.nicolike.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bt.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wo.colortex.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://np.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bv.muxihuayi.cn

[K05] 深拷贝对象
来源：http://uo.9csxet.cn

Py:   copy.deepcopy(obj)
来源：http://vb.szxytkj.cn

PHP:  unserialize(serialize($obj));
来源：http://gw.jianghongdianzi.cn

JS:   structuredClone(obj)
来源：http://wd.panjiajie.cn

TS:   structuredClone(obj)
来源：http://bc.asd995.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://iu.nszjky.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xk.chemitech.net.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sa.szsharing.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cp.asd995.cn

[K06] 解析 URL 查询串
来源：http://qt.wgjwhj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xk.jianghongdianzi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tn.jctech888.com.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ng.szsharing.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sm.jctech888.com.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qd.asd995.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bq.521024.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wa.lnxyls.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jv.nicolike.cn

[K07] 进制转换
来源：http://jm.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tr.huanxung.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ue.jctech888.com.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://by.wgjwhj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://st.haigaiapp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cd.bjjhwx.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ro.shtwfgs.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ct.bookmarksfly.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ka.shxzskj.cn

[K08] 二进制序列化（非 JSON）
来源：http://dq.jctech888.com.cn

Py:   pickle.dumps(obj)
来源：http://yb.lnxyls.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cq.muxihuayi.cn

JS:   v8.serialize(obj)        // Node
来源：http://cd.lnxyls.cn

TS:   v8.serialize(obj)        // Node
来源：http://dc.9csxet.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qx.panjiajie.cn

Go:   encoding/gob
来源：http://no.nszjky.cn

Ruby: Marshal.dump(obj)
来源：http://lr.newstarts.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wi.szsharing.cn

================================================================================
来源：http://dl.jctech888.com.cn

L. 网络请求
来源：http://af.newstarts.cn

================================================================================
来源：http://rg.shxzukj.cn

[L01] 发送 GET 请求
来源：http://fh.521024.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yh.jianghongdianzi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kn.hnjuh.cn

JS:   await fetch(url)
来源：http://fg.bjjhwx.cn

TS:   await fetch(url)
来源：http://vb.hahajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xk.newstarts.cn

Go:   resp, err := http.Get(url)
来源：http://uz.panjiajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zg.bookmarksfly.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fc.newstarts.cn

[L02] 发送 POST JSON
来源：http://yp.jctech888.com.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hj.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xe.hahajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dm.nszjky.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wv.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mb.shxzukj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cs.muxihuayi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bz.nszjky.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sc.haigaiapp.cn

[L03] 设置自定义请求头
来源：http://we.wgjwhj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qk.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://de.newstarts.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ew.shxzukj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zf.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fq.szxytkj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://eu.jctech888.com.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yr.asd995.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://oc.haigaiapp.cn

[L04] 设置超时
来源：http://ih.wgjwhj.cn

Py:   requests.get(url, timeout=5)
来源：http://qt.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dt.lnxyls.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bm.hahajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ek.yuntaijiaju.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ps.szsharing.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qh.yuntaijiaju.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wg.panjiajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ro.hnjuh.cn

[L05] 上传文件（multipart）
来源：http://ab.shxzukj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ur.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ke.huanxung.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jh.shxzukj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ch.huixiangedu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vv.shxzskj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zc.nicolike.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cs.gzmigu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xr.nszjky.cn

[L06] 解析响应为 JSON
来源：http://di.9csxet.cn

Py:   resp.json()
来源：http://sl.521024.cn

PHP:  json_decode($body, true);
来源：http://fa.huixinmuqiang.cn

JS:   await resp.json()
来源：http://za.bookmarksfly.cn

TS:   await resp.json()
来源：http://mk.szsharing.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rp.yuntaijiaju.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://el.newstarts.cn

Ruby: JSON.parse(resp.body)
来源：http://nc.gzmigu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://eg.haigaiapp.cn

[L07] 处理 HTTP 状态码
来源：http://to.hnjuh.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xn.yuntaijiaju.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pt.shxzskj.cn

JS:   resp.ok;  resp.status
来源：http://gp.newstarts.cn

TS:   resp.ok;  resp.status
来源：http://lx.jctech888.com.cn

Java: resp.statusCode()
来源：http://he.hahajie.cn

Go:   resp.StatusCode
来源：http://rj.wgjwhj.cn

Ruby: resp.code.to_i
来源：http://ol.521024.cn

C#:   (int)resp.StatusCode
来源：http://fi.huixinmuqiang.cn

[L08] 并发请求多个地址
来源：http://me.newstarts.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ur.colortex.cn

PHP:  curl_multi_init() 系列
来源：http://jt.shxzskj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pb.shxzukj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nc.hnjuh.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wf.asd995.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rl.nszjky.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bd.bookmarksfly.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yx.shxzukj.cn

================================================================================
来源：http://ak.9csxet.cn

M. 命令行 / 进程 / 环境
来源：http://gx.newstarts.cn

================================================================================
来源：http://yn.yuntaijiaju.cn

[M01] 读取命令行参数
来源：http://kw.nicolike.cn

Py:   sys.argv[1:]
来源：http://vj.shxzukj.cn

PHP:  $argv;  $argc;
来源：http://nu.nicolike.cn

JS:   process.argv.slice(2)
来源：http://ke.huanxung.cn

TS:   process.argv.slice(2)
来源：http://xv.shtwfgs.cn

Java: args 数组（main 方法参数）
来源：http://xi.huixiangedu.cn

Go:   os.Args[1:]
来源：http://zt.shtwfgs.cn

Ruby: ARGV
来源：http://jt.asd995.cn

C#:   args 数组（Main 方法参数）
来源：http://xx.muxihuayi.cn

[M02] 读取环境变量
来源：http://mq.wgjwhj.cn

Py:   os.environ.get("HOME")
来源：http://jf.yuexingan06.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://um.wgjwhj.cn

JS:   process.env.HOME
来源：http://wv.newstarts.cn

TS:   process.env.HOME
来源：http://yq.shxzskj.cn

Java: System.getenv("HOME")
来源：http://bz.huixinmuqiang.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qf.yuntaijiaju.cn

Ruby: ENV["HOME"]
来源：http://wa.newstarts.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fx.jianghongdianzi.cn

[M03] 执行外部命令
来源：http://zo.nszjky.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://oq.lnxyls.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jn.wgjwhj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://iw.panjiajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yg.9csxet.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mq.nicolike.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://te.muxihuayi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ft.yuexingan06.cn

C#:   Process.Start("ls", "-l");
来源：http://ds.huixiangedu.cn

[M04] 获取当前工作目录
来源：http://ai.nszjky.cn

Py:   os.getcwd()
来源：http://tc.hnjuh.cn

PHP:  getcwd();
来源：http://bo.chemitech.net.cn

JS:   process.cwd()
来源：http://op.jctech888.com.cn

TS:   process.cwd()
来源：http://qt.shxzskj.cn

Java: Path.of("").toAbsolutePath()
来源：http://fu.bookmarksfly.cn

Go:   os.Getwd()
来源：http://vi.newstarts.cn

Ruby: Dir.pwd
来源：http://jv.9csxet.cn


<!-- 参考信息 -->