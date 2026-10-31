代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wn.wgjwhj.cn

TS:   /error/gim
来源：http://si.wgjwhj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ux.szsharing.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uv.shtwfgs.cn

Ruby: s.scan(/error/i)
来源：http://zs.521024.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zt.huixinmuqiang.cn

[I08] 贪婪与非贪婪匹配
来源：http://ra.hnjuh.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uq.yuexingan06.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hr.muxihuayi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lq.hnjuh.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yx.haigaiapp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://by.haigaiapp.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pl.newstarts.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tn.panjiajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://up.gzmigu.cn

================================================================================
来源：http://sf.newstarts.cn

J. 日期与时间
来源：http://nu.shxzukj.cn

================================================================================
来源：http://ld.muxihuayi.cn

[J01] 获取当前时间
来源：http://xb.shxzukj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://nq.shtwfgs.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vb.yuntaijiaju.cn

JS:   new Date();  Date.now()
来源：http://cu.9csxet.cn

TS:   new Date();  Date.now()
来源：http://ps.9csxet.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://xy.newstarts.cn

Go:   time.Now()
来源：http://an.jianghongdianzi.cn

Ruby: Time.now
来源：http://xk.bookmarksfly.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lx.panjiajie.cn

[J02] 格式化输出
来源：http://xd.bookmarksfly.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vs.jctech888.com.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jf.wgjwhj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hn.shxzskj.cn

TS:   d.toISOString()
来源：http://qu.wgjwhj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wb.wgjwhj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qo.panjiajie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kk.bookmarksfly.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gb.hnjuh.cn

[J03] 字符串解析为日期
来源：http://xr.colortex.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xa.newstarts.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://oz.shtwfgs.cn

JS:   new Date("2024-01-02")
来源：http://ft.szsharing.cn

TS:   new Date("2024-01-02")
来源：http://if.huanxung.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ha.colortex.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ga.chemitech.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://no.wgjwhj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://um.bjjhwx.cn

[J04] 时间戳与日期互转
来源：http://sv.wgjwhj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ey.jctech888.com.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nx.huixinmuqiang.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nu.panjiajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tn.shxzukj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://np.szsharing.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fc.jctech888.com.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bo.gzmigu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://oe.lnxyls.cn

[J05] 时间加减（加 7 天）
来源：http://ar.szsharing.cn

Py:   now + timedelta(days=7)
来源：http://gs.gzmigu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ej.szxytkj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fa.colortex.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ls.yuexingan06.cn

Java: LocalDate.now().plusDays(7)
来源：http://me.muxihuayi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ok.nszjky.cn

Ruby: Time.now + 7 * 86400
来源：http://iq.shxzskj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ab.newstarts.cn

[J06] 计算两时间之差
来源：http://fn.huixiangedu.cn

Py:   (end - start).total_seconds()
来源：http://ya.jctech888.com.cn

PHP:  $end->diff($start)->days;
来源：http://na.shtwfgs.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mc.shtwfgs.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wm.shxzukj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://nu.newstarts.cn

Go:   end.Sub(start).Hours()
来源：http://wn.gzmigu.cn

Ruby: end - start                 # 返回秒数
来源：http://rq.haigaiapp.cn

C#:   (end - start).TotalSeconds
来源：http://ud.shtwfgs.cn

[J07] 比较两个日期
来源：http://eg.jianghongdianzi.cn

Py:   d1 < d2;  d1 == d2
来源：http://qf.chemitech.net.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://at.hahajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://sv.shxzskj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://sc.bookmarksfly.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ae.nszjky.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lr.huixiangedu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ue.521024.cn

C#:   d1 < d2;  d1 == d2
来源：http://qj.nicolike.cn

[J08] 提取年月日与星期
来源：http://gu.huixinmuqiang.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ra.hnjuh.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xw.521024.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://od.wgjwhj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cj.panjiajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vq.haigaiapp.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dh.muxihuayi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://la.jianghongdianzi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ln.asd995.cn

[J09] 时区处理
来源：http://rd.hnjuh.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hv.shxzukj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ro.9csxet.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pd.chemitech.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fk.yuntaijiaju.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hw.nszjky.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hm.chemitech.net.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gb.haigaiapp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hl.newstarts.cn

[J10] 取今天 / 本月第一天
来源：http://dm.huixinmuqiang.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://eh.nicolike.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kq.yuntaijiaju.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dl.huixinmuqiang.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sb.bookmarksfly.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://en.shxzukj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ob.newstarts.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://es.gzmigu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cz.huixiangedu.cn

================================================================================
来源：http://ei.huixiangedu.cn

K. JSON 与序列化
来源：http://id.yuntaijiaju.cn

================================================================================
来源：http://ft.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://uk.bjjhwx.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vb.huixiangedu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bj.bookmarksfly.cn

JS:   JSON.stringify(obj)
来源：http://ib.wgjwhj.cn

TS:   JSON.stringify(obj)
来源：http://fq.lnxyls.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://aa.huanxung.cn

Go:   json.Marshal(obj)
来源：http://mt.bjjhwx.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vx.nszjky.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jp.bjjhwx.cn

[K02] JSON 字符串转对象
来源：http://hn.wgjwhj.cn

Py:   json.loads(s)
来源：http://qz.yuntaijiaju.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://la.lnxyls.cn

JS:   JSON.parse(s)
来源：http://ne.jctech888.com.cn

TS:   JSON.parse(s)
来源：http://ev.panjiajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nl.9csxet.cn

Go:   json.Unmarshal(data, &v)
来源：http://yq.colortex.cn

Ruby: JSON.parse(s)
来源：http://pw.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ui.gzmigu.cn

[K03] JSON 美化输出（带缩进）
来源：http://re.asd995.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zq.asd995.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nc.chemitech.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ve.shtwfgs.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yz.shtwfgs.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ed.lnxyls.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://au.nszjky.cn

Ruby: JSON.pretty_generate(obj)
来源：http://os.asd995.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dx.szxytkj.cn

[K04] 读取 JSON 文件
来源：http://uy.shtwfgs.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kj.lnxyls.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dt.muxihuayi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ie.newstarts.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uz.bjjhwx.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rs.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sr.nszjky.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://pk.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dm.shxzskj.cn

[K05] 深拷贝对象
来源：http://vf.wgjwhj.cn

Py:   copy.deepcopy(obj)
来源：http://pg.huixiangedu.cn

PHP:  unserialize(serialize($obj));
来源：http://hf.szxytkj.cn

JS:   structuredClone(obj)
来源：http://pw.jctech888.com.cn

TS:   structuredClone(obj)
来源：http://sn.hahajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://cp.huixinmuqiang.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zw.bjjhwx.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fs.haigaiapp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wb.panjiajie.cn

[K06] 解析 URL 查询串
来源：http://ye.chemitech.net.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uu.chemitech.net.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pc.bjjhwx.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uy.jianghongdianzi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wu.chemitech.net.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lt.huixinmuqiang.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ut.colortex.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pw.szsharing.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fb.hahajie.cn

[K07] 进制转换
来源：http://lx.nicolike.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ch.521024.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bc.yuexingan06.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zj.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://oc.huixinmuqiang.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://oc.9csxet.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ug.shxzukj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gp.yuexingan06.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kt.huixiangedu.cn

[K08] 二进制序列化（非 JSON）
来源：http://jg.yuntaijiaju.cn

Py:   pickle.dumps(obj)
来源：http://mh.colortex.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ih.newstarts.cn

JS:   v8.serialize(obj)        // Node
来源：http://zb.szsharing.cn

TS:   v8.serialize(obj)        // Node
来源：http://yq.newstarts.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vm.jianghongdianzi.cn

Go:   encoding/gob
来源：http://em.bjjhwx.cn

Ruby: Marshal.dump(obj)
来源：http://vg.jianghongdianzi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ui.chemitech.net.cn

================================================================================
来源：http://iw.bookmarksfly.cn

L. 网络请求
来源：http://vj.asd995.cn

================================================================================
来源：http://gc.lnxyls.cn

[L01] 发送 GET 请求
来源：http://pm.huixiangedu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://de.lnxyls.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://eo.hahajie.cn

JS:   await fetch(url)
来源：http://rf.9csxet.cn

TS:   await fetch(url)
来源：http://pi.yuntaijiaju.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bs.bookmarksfly.cn

Go:   resp, err := http.Get(url)
来源：http://is.yuexingan06.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://su.huixinmuqiang.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gq.haigaiapp.cn

[L02] 发送 POST JSON
来源：http://wb.muxihuayi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ql.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://np.haigaiapp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uz.huixinmuqiang.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sz.521024.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fl.hnjuh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://da.bookmarksfly.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dc.bookmarksfly.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lo.nszjky.cn

[L03] 设置自定义请求头
来源：http://fr.shxzukj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sy.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vj.hnjuh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://so.yuntaijiaju.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lj.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hl.gzmigu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://eb.huanxung.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yo.asd995.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ey.shxzukj.cn

[L04] 设置超时
来源：http://cf.wgjwhj.cn

Py:   requests.get(url, timeout=5)
来源：http://ph.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gi.shxzskj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vl.panjiajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dv.bookmarksfly.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yx.huanxung.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uy.chemitech.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://iq.asd995.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xk.wgjwhj.cn

[L05] 上传文件（multipart）
来源：http://eg.wgjwhj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ug.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sm.521024.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qs.huixinmuqiang.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hl.yuexingan06.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fw.9csxet.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://er.panjiajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qv.huixinmuqiang.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zn.nicolike.cn

[L06] 解析响应为 JSON
来源：http://dg.nicolike.cn

Py:   resp.json()
来源：http://mq.colortex.cn

PHP:  json_decode($body, true);
来源：http://xx.haigaiapp.cn

JS:   await resp.json()
来源：http://ew.colortex.cn

TS:   await resp.json()
来源：http://lq.jctech888.com.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sd.nszjky.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cs.yuntaijiaju.cn

Ruby: JSON.parse(resp.body)
来源：http://xn.huanxung.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bo.nszjky.cn

[L07] 处理 HTTP 状态码
来源：http://mk.panjiajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wa.hnjuh.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vd.huixinmuqiang.cn

JS:   resp.ok;  resp.status
来源：http://it.yuexingan06.cn

TS:   resp.ok;  resp.status
来源：http://di.nicolike.cn

Java: resp.statusCode()
来源：http://zw.muxihuayi.cn

Go:   resp.StatusCode
来源：http://ts.hnjuh.cn

Ruby: resp.code.to_i
来源：http://rd.asd995.cn

C#:   (int)resp.StatusCode
来源：http://se.9csxet.cn

[L08] 并发请求多个地址
来源：http://vh.asd995.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bv.shtwfgs.cn

PHP:  curl_multi_init() 系列
来源：http://gx.panjiajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://me.bjjhwx.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bw.huixiangedu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zu.nicolike.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://di.szxytkj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gd.panjiajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://au.huanxung.cn

================================================================================
来源：http://zm.gzmigu.cn

M. 命令行 / 进程 / 环境
来源：http://ki.shxzskj.cn

================================================================================
来源：http://bv.nszjky.cn

[M01] 读取命令行参数
来源：http://pk.hahajie.cn

Py:   sys.argv[1:]
来源：http://dw.muxihuayi.cn

PHP:  $argv;  $argc;
来源：http://yr.szxytkj.cn

JS:   process.argv.slice(2)
来源：http://rs.asd995.cn

TS:   process.argv.slice(2)
来源：http://jo.jctech888.com.cn

Java: args 数组（main 方法参数）
来源：http://ps.bookmarksfly.cn

Go:   os.Args[1:]
来源：http://it.shtwfgs.cn

Ruby: ARGV
来源：http://or.panjiajie.cn

C#:   args 数组（Main 方法参数）
来源：http://hw.lnxyls.cn

[M02] 读取环境变量
来源：http://ll.hahajie.cn

Py:   os.environ.get("HOME")
来源：http://ck.yuntaijiaju.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ir.yuexingan06.cn

JS:   process.env.HOME
来源：http://cl.panjiajie.cn

TS:   process.env.HOME
来源：http://ns.huanxung.cn

Java: System.getenv("HOME")
来源：http://zd.521024.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qv.newstarts.cn

Ruby: ENV["HOME"]
来源：http://vz.nszjky.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xo.asd995.cn

[M03] 执行外部命令
来源：http://lq.shxzukj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bb.newstarts.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ed.shxzskj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://eu.colortex.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://hb.yuntaijiaju.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yv.nicolike.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zw.huanxung.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ap.bookmarksfly.cn

C#:   Process.Start("ls", "-l");
来源：http://ul.szxytkj.cn

[M04] 获取当前工作目录
来源：http://fd.muxihuayi.cn

Py:   os.getcwd()
来源：http://fe.colortex.cn

PHP:  getcwd();
来源：http://xn.newstarts.cn

JS:   process.cwd()
来源：http://zq.shxzskj.cn

TS:   process.cwd()
来源：http://un.lnxyls.cn

Java: Path.of("").toAbsolutePath()
来源：http://cx.huixinmuqiang.cn

Go:   os.Getwd()
来源：http://xn.szsharing.cn

Ruby: Dir.pwd
来源：http://xy.muxihuayi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://pv.shxzskj.cn

[M05] 设置退出码
来源：http://pg.szxytkj.cn

Py:   sys.exit(1)
来源：http://ng.jianghongdianzi.cn

PHP:  exit(1);
来源：http://nb.hnjuh.cn


<!-- 参考信息 -->