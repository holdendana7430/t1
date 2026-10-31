代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nf.hahajie.cn

[I07] 忽略大小写与多行模式
来源：http://xu.shtwfgs.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xj.chemitech.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dn.bjjhwx.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ld.shxzskj.cn

TS:   /error/gim
来源：http://jx.huixiangedu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mn.szsharing.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://du.gzmigu.cn

Ruby: s.scan(/error/i)
来源：http://oh.9csxet.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://iz.asd995.cn

[I08] 贪婪与非贪婪匹配
来源：http://ti.asd995.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xn.wgjwhj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gd.haigaiapp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rk.huixinmuqiang.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jl.yuntaijiaju.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ez.huanxung.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jy.hnjuh.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pq.9csxet.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jm.huixinmuqiang.cn

================================================================================
来源：http://xl.chemitech.net.cn

J. 日期与时间
来源：http://bk.bookmarksfly.cn

================================================================================
来源：http://zu.newstarts.cn

[J01] 获取当前时间
来源：http://ne.shtwfgs.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://jq.asd995.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tu.asd995.cn

JS:   new Date();  Date.now()
来源：http://xb.lnxyls.cn

TS:   new Date();  Date.now()
来源：http://wy.shxzskj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wc.newstarts.cn

Go:   time.Now()
来源：http://mm.shxzskj.cn

Ruby: Time.now
来源：http://as.9csxet.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zo.bjjhwx.cn

[J02] 格式化输出
来源：http://cr.shtwfgs.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oo.szxytkj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://of.gzmigu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yc.chemitech.net.cn

TS:   d.toISOString()
来源：http://vl.haigaiapp.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mz.chemitech.net.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pp.hahajie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xq.szxytkj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://aq.bookmarksfly.cn

[J03] 字符串解析为日期
来源：http://fm.szsharing.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ho.521024.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bj.shxzukj.cn

JS:   new Date("2024-01-02")
来源：http://wq.newstarts.cn

TS:   new Date("2024-01-02")
来源：http://yu.jianghongdianzi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jx.jianghongdianzi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jh.nicolike.cn

Ruby: Date.parse("2024-01-02")
来源：http://ki.asd995.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bj.yuntaijiaju.cn

[J04] 时间戳与日期互转
来源：http://ex.jctech888.com.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://oc.muxihuayi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ol.hnjuh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zs.chemitech.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://sq.haigaiapp.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dd.huixinmuqiang.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ph.hahajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cv.gzmigu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nk.huixinmuqiang.cn

[J05] 时间加减（加 7 天）
来源：http://pq.newstarts.cn

Py:   now + timedelta(days=7)
来源：http://du.asd995.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wg.muxihuayi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://do.nszjky.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gu.yuexingan06.cn

Java: LocalDate.now().plusDays(7)
来源：http://lj.gzmigu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sf.521024.cn

Ruby: Time.now + 7 * 86400
来源：http://sb.szxytkj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://oz.huixinmuqiang.cn

[J06] 计算两时间之差
来源：http://nm.bookmarksfly.cn

Py:   (end - start).total_seconds()
来源：http://eg.jctech888.com.cn

PHP:  $end->diff($start)->days;
来源：http://kv.newstarts.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sq.colortex.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wb.shtwfgs.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ks.huixinmuqiang.cn

Go:   end.Sub(start).Hours()
来源：http://nn.lnxyls.cn

Ruby: end - start                 # 返回秒数
来源：http://kn.wgjwhj.cn

C#:   (end - start).TotalSeconds
来源：http://jh.panjiajie.cn

[J07] 比较两个日期
来源：http://kb.yuexingan06.cn

Py:   d1 < d2;  d1 == d2
来源：http://lt.shxzskj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kl.9csxet.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gh.panjiajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ue.asd995.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ia.huanxung.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pj.szsharing.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wo.9csxet.cn

C#:   d1 < d2;  d1 == d2
来源：http://ps.chemitech.net.cn

[J08] 提取年月日与星期
来源：http://vb.shxzukj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://et.bookmarksfly.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gy.huixiangedu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wb.521024.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kt.wgjwhj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pm.muxihuayi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ap.hnjuh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://iz.wgjwhj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vz.huanxung.cn

[J09] 时区处理
来源：http://rs.asd995.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jz.szsharing.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ar.asd995.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://st.huixiangedu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ma.szsharing.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kk.hahajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://je.szxytkj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jr.shtwfgs.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ou.bookmarksfly.cn

[J10] 取今天 / 本月第一天
来源：http://my.shxzskj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bg.lnxyls.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hb.szxytkj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wp.shxzskj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ep.bookmarksfly.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ic.nicolike.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zw.521024.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ta.shxzskj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ou.shxzukj.cn

================================================================================
来源：http://an.hahajie.cn

K. JSON 与序列化
来源：http://dc.haigaiapp.cn

================================================================================
来源：http://xs.huixiangedu.cn

[K01] 对象转 JSON 字符串
来源：http://eq.yuntaijiaju.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pg.newstarts.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oy.huixiangedu.cn

JS:   JSON.stringify(obj)
来源：http://te.chemitech.net.cn

TS:   JSON.stringify(obj)
来源：http://oq.asd995.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ux.huixinmuqiang.cn

Go:   json.Marshal(obj)
来源：http://fu.asd995.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jw.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ta.huixiangedu.cn

[K02] JSON 字符串转对象
来源：http://vq.jianghongdianzi.cn

Py:   json.loads(s)
来源：http://nf.jctech888.com.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://py.colortex.cn

JS:   JSON.parse(s)
来源：http://qq.9csxet.cn

TS:   JSON.parse(s)
来源：http://jx.muxihuayi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ij.jctech888.com.cn

Go:   json.Unmarshal(data, &v)
来源：http://wj.yuntaijiaju.cn

Ruby: JSON.parse(s)
来源：http://yp.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yc.jianghongdianzi.cn

[K03] JSON 美化输出（带缩进）
来源：http://en.nszjky.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qh.9csxet.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://su.panjiajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://oj.shtwfgs.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sf.jianghongdianzi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ep.yuntaijiaju.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://al.huanxung.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fz.hahajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lh.newstarts.cn

[K04] 读取 JSON 文件
来源：http://jo.haigaiapp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pt.yuexingan06.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vi.bookmarksfly.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bb.shxzskj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ev.lnxyls.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://iv.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cy.huanxung.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://pw.521024.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ku.yuexingan06.cn

[K05] 深拷贝对象
来源：http://tj.lnxyls.cn

Py:   copy.deepcopy(obj)
来源：http://sa.panjiajie.cn

PHP:  unserialize(serialize($obj));
来源：http://px.wgjwhj.cn

JS:   structuredClone(obj)
来源：http://km.nszjky.cn

TS:   structuredClone(obj)
来源：http://ym.yuntaijiaju.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://oj.colortex.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ux.huixiangedu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tm.hnjuh.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://al.huixiangedu.cn

[K06] 解析 URL 查询串
来源：http://zn.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ob.lnxyls.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rt.gzmigu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ih.colortex.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ml.jianghongdianzi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hd.gzmigu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://oy.nicolike.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://su.colortex.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mh.wgjwhj.cn

[K07] 进制转换
来源：http://ix.jianghongdianzi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qs.521024.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ei.huixiangedu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ku.9csxet.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xo.hahajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://oh.asd995.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rz.panjiajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://eh.asd995.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ll.muxihuayi.cn

[K08] 二进制序列化（非 JSON）
来源：http://xr.szsharing.cn

Py:   pickle.dumps(obj)
来源：http://ld.bookmarksfly.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ib.asd995.cn

JS:   v8.serialize(obj)        // Node
来源：http://rk.muxihuayi.cn

TS:   v8.serialize(obj)        // Node
来源：http://rr.muxihuayi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vn.yuntaijiaju.cn

Go:   encoding/gob
来源：http://ve.newstarts.cn

Ruby: Marshal.dump(obj)
来源：http://wt.gzmigu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ba.szxytkj.cn

================================================================================
来源：http://kr.szsharing.cn

L. 网络请求
来源：http://rq.szsharing.cn

================================================================================
来源：http://lb.nicolike.cn

[L01] 发送 GET 请求
来源：http://pe.yuntaijiaju.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://po.hahajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ty.haigaiapp.cn

JS:   await fetch(url)
来源：http://fg.chemitech.net.cn

TS:   await fetch(url)
来源：http://dg.hnjuh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lb.szsharing.cn

Go:   resp, err := http.Get(url)
来源：http://yr.huixinmuqiang.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://lu.bjjhwx.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ri.9csxet.cn

[L02] 发送 POST JSON
来源：http://lp.nicolike.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ex.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dy.shxzukj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bc.jianghongdianzi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dl.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://oh.huixiangedu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lj.yuntaijiaju.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ei.lnxyls.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://oz.yuntaijiaju.cn

[L03] 设置自定义请求头
来源：http://af.gzmigu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bi.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ll.jctech888.com.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fp.nszjky.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://av.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bv.bjjhwx.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rq.521024.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vp.jctech888.com.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sh.nszjky.cn

[L04] 设置超时
来源：http://kx.hahajie.cn

Py:   requests.get(url, timeout=5)
来源：http://li.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ez.chemitech.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wq.huanxung.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://up.colortex.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kj.bookmarksfly.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lo.huixiangedu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lm.haigaiapp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qd.huixiangedu.cn

[L05] 上传文件（multipart）
来源：http://gi.huixinmuqiang.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://oj.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fi.chemitech.net.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://im.gzmigu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fm.yuntaijiaju.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://te.yuexingan06.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rj.huanxung.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fx.shtwfgs.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lt.hahajie.cn

[L06] 解析响应为 JSON
来源：http://hz.521024.cn

Py:   resp.json()
来源：http://hc.haigaiapp.cn

PHP:  json_decode($body, true);
来源：http://el.jctech888.com.cn

JS:   await resp.json()
来源：http://ud.haigaiapp.cn

TS:   await resp.json()
来源：http://em.nszjky.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sq.bjjhwx.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jh.gzmigu.cn

Ruby: JSON.parse(resp.body)
来源：http://sx.bjjhwx.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jd.szxytkj.cn

[L07] 处理 HTTP 状态码
来源：http://zy.wgjwhj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fq.yuexingan06.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yr.shxzskj.cn

JS:   resp.ok;  resp.status
来源：http://yy.bjjhwx.cn

TS:   resp.ok;  resp.status
来源：http://ht.shtwfgs.cn

Java: resp.statusCode()
来源：http://uz.huixiangedu.cn

Go:   resp.StatusCode
来源：http://tv.wgjwhj.cn

Ruby: resp.code.to_i
来源：http://fg.szxytkj.cn

C#:   (int)resp.StatusCode
来源：http://vk.wgjwhj.cn

[L08] 并发请求多个地址
来源：http://fw.yuntaijiaju.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ju.muxihuayi.cn

PHP:  curl_multi_init() 系列
来源：http://ci.gzmigu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pl.huixinmuqiang.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dc.jctech888.com.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xm.huixiangedu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xi.shtwfgs.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ek.szsharing.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lp.wgjwhj.cn

================================================================================
来源：http://au.nicolike.cn

M. 命令行 / 进程 / 环境
来源：http://pe.szxytkj.cn

================================================================================
来源：http://kh.haigaiapp.cn

[M01] 读取命令行参数
来源：http://gq.nicolike.cn

Py:   sys.argv[1:]
来源：http://um.wgjwhj.cn

PHP:  $argv;  $argc;
来源：http://ep.shtwfgs.cn

JS:   process.argv.slice(2)
来源：http://am.szxytkj.cn

TS:   process.argv.slice(2)
来源：http://ah.bookmarksfly.cn

Java: args 数组（main 方法参数）
来源：http://zq.nszjky.cn

Go:   os.Args[1:]
来源：http://gh.szsharing.cn

Ruby: ARGV
来源：http://gb.huixiangedu.cn

C#:   args 数组（Main 方法参数）
来源：http://kg.bjjhwx.cn

[M02] 读取环境变量
来源：http://np.shxzskj.cn

Py:   os.environ.get("HOME")
来源：http://ru.shxzukj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lt.521024.cn

JS:   process.env.HOME
来源：http://lt.hahajie.cn

TS:   process.env.HOME
来源：http://zy.bjjhwx.cn

Java: System.getenv("HOME")
来源：http://mc.yuexingan06.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bs.szxytkj.cn

Ruby: ENV["HOME"]
来源：http://dn.szxytkj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hv.yuntaijiaju.cn

[M03] 执行外部命令
来源：http://ga.asd995.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bv.521024.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pf.asd995.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vr.bjjhwx.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ni.hahajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lk.yuntaijiaju.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nz.gzmigu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://nr.jianghongdianzi.cn

C#:   Process.Start("ls", "-l");
来源：http://uv.shxzskj.cn

[M04] 获取当前工作目录
来源：http://mx.szxytkj.cn

Py:   os.getcwd()
来源：http://bi.shxzukj.cn

PHP:  getcwd();
来源：http://wo.chemitech.net.cn

JS:   process.cwd()
来源：http://tq.wgjwhj.cn

TS:   process.cwd()
来源：http://fv.9csxet.cn

Java: Path.of("").toAbsolutePath()
来源：http://zp.521024.cn

Go:   os.Getwd()
来源：http://ay.bookmarksfly.cn

Ruby: Dir.pwd
来源：http://mb.panjiajie.cn


<!-- 参考信息 -->