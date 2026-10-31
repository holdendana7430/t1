代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ig.nicolike.cn

[I07] 忽略大小写与多行模式
来源：http://zp.yuntaijiaju.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://os.muxihuayi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wp.muxihuayi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://et.hnjuh.cn

TS:   /error/gim
来源：http://dx.huixinmuqiang.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tx.bookmarksfly.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vq.szxytkj.cn

Ruby: s.scan(/error/i)
来源：http://fa.chemitech.net.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vv.9csxet.cn

[I08] 贪婪与非贪婪匹配
来源：http://pz.lnxyls.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wk.9csxet.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xf.chemitech.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hq.shxzskj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wa.hnjuh.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bl.9csxet.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uz.nicolike.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uf.huixinmuqiang.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ji.521024.cn

================================================================================
来源：http://dr.huixiangedu.cn

J. 日期与时间
来源：http://mi.asd995.cn

================================================================================
来源：http://ki.yuntaijiaju.cn

[J01] 获取当前时间
来源：http://ne.asd995.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://an.nicolike.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ce.jctech888.com.cn

JS:   new Date();  Date.now()
来源：http://bd.shxzukj.cn

TS:   new Date();  Date.now()
来源：http://ij.hahajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://js.gzmigu.cn

Go:   time.Now()
来源：http://wg.hahajie.cn

Ruby: Time.now
来源：http://mf.yuexingan06.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://si.yuntaijiaju.cn

[J02] 格式化输出
来源：http://xi.muxihuayi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://da.jianghongdianzi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hi.huixinmuqiang.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nt.lnxyls.cn

TS:   d.toISOString()
来源：http://us.chemitech.net.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ga.shtwfgs.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://th.shxzskj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wm.hahajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zn.gzmigu.cn

[J03] 字符串解析为日期
来源：http://kj.shxzukj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bg.nicolike.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lz.nicolike.cn

JS:   new Date("2024-01-02")
来源：http://cj.9csxet.cn

TS:   new Date("2024-01-02")
来源：http://lf.huanxung.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pr.huixiangedu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hb.gzmigu.cn

Ruby: Date.parse("2024-01-02")
来源：http://pb.nszjky.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vd.hahajie.cn

[J04] 时间戳与日期互转
来源：http://wm.haigaiapp.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://aj.muxihuayi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nz.chemitech.net.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://up.chemitech.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wn.shtwfgs.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ve.lnxyls.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pn.panjiajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tu.gzmigu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://go.9csxet.cn

[J05] 时间加减（加 7 天）
来源：http://mb.nicolike.cn

Py:   now + timedelta(days=7)
来源：http://js.gzmigu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ed.panjiajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wb.haigaiapp.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://io.hnjuh.cn

Java: LocalDate.now().plusDays(7)
来源：http://gm.chemitech.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nv.asd995.cn

Ruby: Time.now + 7 * 86400
来源：http://xj.9csxet.cn

C#:   DateTime.Now.AddDays(7)
来源：http://py.jianghongdianzi.cn

[J06] 计算两时间之差
来源：http://nw.yuntaijiaju.cn

Py:   (end - start).total_seconds()
来源：http://fq.bookmarksfly.cn

PHP:  $end->diff($start)->days;
来源：http://te.hahajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fj.yuexingan06.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://en.jctech888.com.cn

Java: Duration.between(start, end).toSeconds()
来源：http://iy.yuntaijiaju.cn

Go:   end.Sub(start).Hours()
来源：http://zf.bookmarksfly.cn

Ruby: end - start                 # 返回秒数
来源：http://pr.asd995.cn

C#:   (end - start).TotalSeconds
来源：http://ff.panjiajie.cn

[J07] 比较两个日期
来源：http://xp.lnxyls.cn

Py:   d1 < d2;  d1 == d2
来源：http://gg.521024.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tz.shxzukj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zw.9csxet.cn

TS:   d1.getTime() < d2.getTime()
来源：http://dy.asd995.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://no.wgjwhj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pc.jianghongdianzi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vj.gzmigu.cn

C#:   d1 < d2;  d1 == d2
来源：http://ul.muxihuayi.cn

[J08] 提取年月日与星期
来源：http://dl.huixiangedu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ri.yuexingan06.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ol.lnxyls.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mh.lnxyls.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jc.colortex.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fu.lnxyls.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yo.huixiangedu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gh.chemitech.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xn.shxzukj.cn

[J09] 时区处理
来源：http://zz.shtwfgs.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ss.szsharing.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xb.szsharing.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zh.gzmigu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kc.newstarts.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hk.asd995.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zl.yuntaijiaju.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://kn.nszjky.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fp.szsharing.cn

[J10] 取今天 / 本月第一天
来源：http://ew.jctech888.com.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kd.hnjuh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gc.huixinmuqiang.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://la.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://el.hnjuh.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bb.huixiangedu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://md.bookmarksfly.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tj.wgjwhj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fz.shxzskj.cn

================================================================================
来源：http://ox.haigaiapp.cn

K. JSON 与序列化
来源：http://jp.huixinmuqiang.cn

================================================================================
来源：http://sg.shxzskj.cn

[K01] 对象转 JSON 字符串
来源：http://od.huanxung.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bv.huanxung.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://az.asd995.cn

JS:   JSON.stringify(obj)
来源：http://wp.colortex.cn

TS:   JSON.stringify(obj)
来源：http://ae.panjiajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yt.huanxung.cn

Go:   json.Marshal(obj)
来源：http://xs.shxzskj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ik.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://oc.huixiangedu.cn

[K02] JSON 字符串转对象
来源：http://tm.wgjwhj.cn

Py:   json.loads(s)
来源：http://st.jianghongdianzi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dz.shtwfgs.cn

JS:   JSON.parse(s)
来源：http://wk.asd995.cn

TS:   JSON.parse(s)
来源：http://ju.szsharing.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gf.haigaiapp.cn

Go:   json.Unmarshal(data, &v)
来源：http://uz.muxihuayi.cn

Ruby: JSON.parse(s)
来源：http://xv.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pc.nicolike.cn

[K03] JSON 美化输出（带缩进）
来源：http://zi.shxzskj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kl.muxihuayi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sq.shxzskj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vl.lnxyls.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qe.bjjhwx.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://er.colortex.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://be.huixiangedu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vf.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://id.haigaiapp.cn

[K04] 读取 JSON 文件
来源：http://kk.chemitech.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pf.haigaiapp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uw.bjjhwx.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pt.szxytkj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://as.yuntaijiaju.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ce.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://di.asd995.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://tr.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dh.newstarts.cn

[K05] 深拷贝对象
来源：http://pi.panjiajie.cn

Py:   copy.deepcopy(obj)
来源：http://er.bookmarksfly.cn

PHP:  unserialize(serialize($obj));
来源：http://kf.panjiajie.cn

JS:   structuredClone(obj)
来源：http://op.huixiangedu.cn

TS:   structuredClone(obj)
来源：http://oc.gzmigu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ub.jctech888.com.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pz.huixiangedu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ax.jctech888.com.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yo.nszjky.cn

[K06] 解析 URL 查询串
来源：http://by.huanxung.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fz.wgjwhj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xx.yuntaijiaju.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://br.jctech888.com.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ed.nszjky.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://st.szxytkj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xd.shxzskj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ee.huixiangedu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fd.nicolike.cn

[K07] 进制转换
来源：http://wt.huanxung.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gm.muxihuayi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dd.huixinmuqiang.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xy.hahajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zz.gzmigu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rd.gzmigu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oj.521024.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nv.muxihuayi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xn.9csxet.cn

[K08] 二进制序列化（非 JSON）
来源：http://bu.bjjhwx.cn

Py:   pickle.dumps(obj)
来源：http://kp.muxihuayi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://da.newstarts.cn

JS:   v8.serialize(obj)        // Node
来源：http://fi.yuntaijiaju.cn

TS:   v8.serialize(obj)        // Node
来源：http://jy.szsharing.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wg.szxytkj.cn

Go:   encoding/gob
来源：http://yz.asd995.cn

Ruby: Marshal.dump(obj)
来源：http://oe.nicolike.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mr.bookmarksfly.cn

================================================================================
来源：http://vl.bjjhwx.cn

L. 网络请求
来源：http://ki.huanxung.cn

================================================================================
来源：http://xx.newstarts.cn

[L01] 发送 GET 请求
来源：http://zz.panjiajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ik.shxzskj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dz.521024.cn

JS:   await fetch(url)
来源：http://lp.wgjwhj.cn

TS:   await fetch(url)
来源：http://yb.bookmarksfly.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zk.hnjuh.cn

Go:   resp, err := http.Get(url)
来源：http://kw.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ck.521024.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oo.gzmigu.cn

[L02] 发送 POST JSON
来源：http://pn.shtwfgs.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gb.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ch.shtwfgs.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tt.shxzukj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yn.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rh.huanxung.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gp.chemitech.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nd.panjiajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zn.9csxet.cn

[L03] 设置自定义请求头
来源：http://xc.szsharing.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zq.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gi.nszjky.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hp.hahajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kw.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hx.szxytkj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ar.szxytkj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jk.shxzskj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dp.9csxet.cn

[L04] 设置超时
来源：http://wc.wgjwhj.cn

Py:   requests.get(url, timeout=5)
来源：http://sy.521024.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fl.szxytkj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lu.newstarts.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lw.panjiajie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gb.bjjhwx.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dw.shtwfgs.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kr.huixiangedu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qi.asd995.cn

[L05] 上传文件（multipart）
来源：http://hd.hahajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uv.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://at.gzmigu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://oz.colortex.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tx.huixiangedu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tc.9csxet.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ff.nicolike.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://er.nszjky.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yh.hnjuh.cn

[L06] 解析响应为 JSON
来源：http://sm.shtwfgs.cn

Py:   resp.json()
来源：http://vc.9csxet.cn

PHP:  json_decode($body, true);
来源：http://ix.jianghongdianzi.cn

JS:   await resp.json()
来源：http://ct.hahajie.cn

TS:   await resp.json()
来源：http://gx.colortex.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lq.muxihuayi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lj.gzmigu.cn

Ruby: JSON.parse(resp.body)
来源：http://zy.jctech888.com.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ps.szsharing.cn

[L07] 处理 HTTP 状态码
来源：http://je.jianghongdianzi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ea.shxzukj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zh.szsharing.cn

JS:   resp.ok;  resp.status
来源：http://jd.nicolike.cn

TS:   resp.ok;  resp.status
来源：http://el.jctech888.com.cn

Java: resp.statusCode()
来源：http://ij.haigaiapp.cn

Go:   resp.StatusCode
来源：http://va.newstarts.cn

Ruby: resp.code.to_i
来源：http://zs.jctech888.com.cn

C#:   (int)resp.StatusCode
来源：http://ma.asd995.cn

[L08] 并发请求多个地址
来源：http://gx.hahajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xr.shxzskj.cn

PHP:  curl_multi_init() 系列
来源：http://pr.bjjhwx.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fv.shtwfgs.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zm.newstarts.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gz.jianghongdianzi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jv.asd995.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ul.hahajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fa.huixinmuqiang.cn

================================================================================
来源：http://tt.hahajie.cn

M. 命令行 / 进程 / 环境
来源：http://qg.hnjuh.cn

================================================================================
来源：http://bo.jctech888.com.cn

[M01] 读取命令行参数
来源：http://xr.521024.cn

Py:   sys.argv[1:]
来源：http://iv.newstarts.cn

PHP:  $argv;  $argc;
来源：http://nl.bjjhwx.cn

JS:   process.argv.slice(2)
来源：http://gk.shxzskj.cn

TS:   process.argv.slice(2)
来源：http://tx.muxihuayi.cn

Java: args 数组（main 方法参数）
来源：http://nf.colortex.cn

Go:   os.Args[1:]
来源：http://mg.hahajie.cn

Ruby: ARGV
来源：http://le.hahajie.cn

C#:   args 数组（Main 方法参数）
来源：http://aw.9csxet.cn

[M02] 读取环境变量
来源：http://xj.jianghongdianzi.cn

Py:   os.environ.get("HOME")
来源：http://yb.521024.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zk.jianghongdianzi.cn

JS:   process.env.HOME
来源：http://mv.huixinmuqiang.cn

TS:   process.env.HOME
来源：http://ee.yuntaijiaju.cn

Java: System.getenv("HOME")
来源：http://qc.jctech888.com.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ch.huixinmuqiang.cn

Ruby: ENV["HOME"]
来源：http://ne.huixinmuqiang.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tf.9csxet.cn

[M03] 执行外部命令
来源：http://ul.9csxet.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fv.szsharing.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ve.shtwfgs.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nd.bookmarksfly.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fx.newstarts.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yk.szxytkj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gy.huixinmuqiang.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ks.nicolike.cn

C#:   Process.Start("ls", "-l");
来源：http://ib.asd995.cn

[M04] 获取当前工作目录
来源：http://ys.szsharing.cn

Py:   os.getcwd()
来源：http://iy.9csxet.cn

PHP:  getcwd();
来源：http://hh.bjjhwx.cn

JS:   process.cwd()
来源：http://wk.bjjhwx.cn

TS:   process.cwd()
来源：http://rq.bookmarksfly.cn

Java: Path.of("").toAbsolutePath()
来源：http://xw.bookmarksfly.cn

Go:   os.Getwd()
来源：http://nk.bookmarksfly.cn

Ruby: Dir.pwd
来源：http://hk.huanxung.cn


<!-- 参考信息 -->