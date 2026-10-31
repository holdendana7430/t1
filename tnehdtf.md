代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nl.bookmarksfly.cn

[I07] 忽略大小写与多行模式
来源：http://ml.bookmarksfly.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ym.9csxet.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://id.yuntaijiaju.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kf.bookmarksfly.cn

TS:   /error/gim
来源：http://tq.nicolike.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rj.newstarts.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tw.shtwfgs.cn

Ruby: s.scan(/error/i)
来源：http://vl.gzmigu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://px.gzmigu.cn

[I08] 贪婪与非贪婪匹配
来源：http://zd.521024.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xi.huixinmuqiang.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hv.gzmigu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dh.9csxet.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sb.colortex.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xl.gzmigu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kd.hnjuh.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nk.yuexingan06.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sw.huanxung.cn

================================================================================
来源：http://xz.jianghongdianzi.cn

J. 日期与时间
来源：http://lx.asd995.cn

================================================================================
来源：http://es.szsharing.cn

[J01] 获取当前时间
来源：http://ps.yuntaijiaju.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ng.nszjky.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gh.yuntaijiaju.cn

JS:   new Date();  Date.now()
来源：http://vw.shtwfgs.cn

TS:   new Date();  Date.now()
来源：http://cx.hahajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fx.hnjuh.cn

Go:   time.Now()
来源：http://tb.wgjwhj.cn

Ruby: Time.now
来源：http://jv.muxihuayi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lt.gzmigu.cn

[J02] 格式化输出
来源：http://xa.nicolike.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kq.yuexingan06.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gr.huixiangedu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yt.wgjwhj.cn

TS:   d.toISOString()
来源：http://ll.muxihuayi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nz.bookmarksfly.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ez.huixiangedu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pk.bjjhwx.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xf.hahajie.cn

[J03] 字符串解析为日期
来源：http://mq.shtwfgs.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kj.wgjwhj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yy.521024.cn

JS:   new Date("2024-01-02")
来源：http://qz.panjiajie.cn

TS:   new Date("2024-01-02")
来源：http://gt.nicolike.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ng.bookmarksfly.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://st.hahajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://lz.jianghongdianzi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xt.shxzukj.cn

[J04] 时间戳与日期互转
来源：http://jj.hnjuh.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://op.yuexingan06.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yk.chemitech.net.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.haigaiapp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wq.panjiajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fj.muxihuayi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ve.huanxung.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://un.gzmigu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ma.asd995.cn

[J05] 时间加减（加 7 天）
来源：http://hh.wgjwhj.cn

Py:   now + timedelta(days=7)
来源：http://up.nszjky.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sv.jianghongdianzi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://be.muxihuayi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zr.shtwfgs.cn

Java: LocalDate.now().plusDays(7)
来源：http://um.muxihuayi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ow.haigaiapp.cn

Ruby: Time.now + 7 * 86400
来源：http://fq.wgjwhj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ud.huanxung.cn

[J06] 计算两时间之差
来源：http://ef.chemitech.net.cn

Py:   (end - start).total_seconds()
来源：http://wq.newstarts.cn

PHP:  $end->diff($start)->days;
来源：http://yb.jctech888.com.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kx.newstarts.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jy.gzmigu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gp.bookmarksfly.cn

Go:   end.Sub(start).Hours()
来源：http://iq.asd995.cn

Ruby: end - start                 # 返回秒数
来源：http://oo.shxzukj.cn

C#:   (end - start).TotalSeconds
来源：http://eq.yuexingan06.cn

[J07] 比较两个日期
来源：http://vp.asd995.cn

Py:   d1 < d2;  d1 == d2
来源：http://pt.szxytkj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sx.szsharing.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jx.gzmigu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xw.panjiajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://aw.yuexingan06.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://el.gzmigu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://he.newstarts.cn

C#:   d1 < d2;  d1 == d2
来源：http://if.colortex.cn

[J08] 提取年月日与星期
来源：http://ld.wgjwhj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fu.chemitech.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ti.asd995.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vp.chemitech.net.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wj.nicolike.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hh.bjjhwx.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://go.nszjky.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ql.shxzukj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://oa.shtwfgs.cn

[J09] 时区处理
来源：http://aj.colortex.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yj.521024.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nw.bjjhwx.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rq.shxzukj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://al.jctech888.com.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fb.yuntaijiaju.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hs.yuexingan06.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://la.yuntaijiaju.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vt.szsharing.cn

[J10] 取今天 / 本月第一天
来源：http://rx.jianghongdianzi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://mv.szxytkj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qs.9csxet.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ca.jctech888.com.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yv.bookmarksfly.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gv.huanxung.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dj.lnxyls.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tv.shxzukj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://io.newstarts.cn

================================================================================
来源：http://uk.hahajie.cn

K. JSON 与序列化
来源：http://wc.wgjwhj.cn

================================================================================
来源：http://ry.hahajie.cn

[K01] 对象转 JSON 字符串
来源：http://xc.bookmarksfly.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xz.9csxet.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ba.newstarts.cn

JS:   JSON.stringify(obj)
来源：http://gn.huixiangedu.cn

TS:   JSON.stringify(obj)
来源：http://ob.szxytkj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nq.521024.cn

Go:   json.Marshal(obj)
来源：http://hp.newstarts.cn

Ruby: obj.to_json                                     // require "json"
来源：http://za.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://re.lnxyls.cn

[K02] JSON 字符串转对象
来源：http://cl.haigaiapp.cn

Py:   json.loads(s)
来源：http://hg.newstarts.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://an.nszjky.cn

JS:   JSON.parse(s)
来源：http://pu.hnjuh.cn

TS:   JSON.parse(s)
来源：http://wy.haigaiapp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sd.newstarts.cn

Go:   json.Unmarshal(data, &v)
来源：http://mu.haigaiapp.cn

Ruby: JSON.parse(s)
来源：http://ua.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tz.huixinmuqiang.cn

[K03] JSON 美化输出（带缩进）
来源：http://wn.bookmarksfly.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ae.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jk.yuntaijiaju.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jb.huanxung.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bs.jctech888.com.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zb.muxihuayi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ue.nicolike.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gl.szsharing.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ms.huanxung.cn

[K04] 读取 JSON 文件
来源：http://fu.newstarts.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://co.szxytkj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fw.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://np.yuexingan06.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zf.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sg.shxzukj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dm.szsharing.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xr.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pv.gzmigu.cn

[K05] 深拷贝对象
来源：http://bi.muxihuayi.cn

Py:   copy.deepcopy(obj)
来源：http://lt.nicolike.cn

PHP:  unserialize(serialize($obj));
来源：http://fc.nszjky.cn

JS:   structuredClone(obj)
来源：http://xg.colortex.cn

TS:   structuredClone(obj)
来源：http://ki.hahajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://lk.nszjky.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://uc.hnjuh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dv.hahajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://on.yuntaijiaju.cn

[K06] 解析 URL 查询串
来源：http://nk.nicolike.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qo.muxihuayi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://em.hnjuh.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bn.nicolike.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ek.hahajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://oi.gzmigu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fr.huixinmuqiang.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://na.colortex.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sh.haigaiapp.cn

[K07] 进制转换
来源：http://qv.hahajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fb.szxytkj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yh.yuntaijiaju.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nc.szxytkj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yz.huixinmuqiang.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yi.jctech888.com.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dr.jianghongdianzi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sz.chemitech.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hp.nicolike.cn

[K08] 二进制序列化（非 JSON）
来源：http://xg.szsharing.cn

Py:   pickle.dumps(obj)
来源：http://ke.hahajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ku.muxihuayi.cn

JS:   v8.serialize(obj)        // Node
来源：http://mi.szsharing.cn

TS:   v8.serialize(obj)        // Node
来源：http://el.hnjuh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ay.shxzukj.cn

Go:   encoding/gob
来源：http://aj.shtwfgs.cn

Ruby: Marshal.dump(obj)
来源：http://bp.szsharing.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zz.huixinmuqiang.cn

================================================================================
来源：http://vf.shtwfgs.cn

L. 网络请求
来源：http://zx.hahajie.cn

================================================================================
来源：http://tl.huixiangedu.cn

[L01] 发送 GET 请求
来源：http://ih.muxihuayi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://px.shxzukj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gv.wgjwhj.cn

JS:   await fetch(url)
来源：http://zx.shxzukj.cn

TS:   await fetch(url)
来源：http://gz.jianghongdianzi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qk.nszjky.cn

Go:   resp, err := http.Get(url)
来源：http://yu.521024.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hp.hnjuh.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://je.chemitech.net.cn

[L02] 发送 POST JSON
来源：http://nr.nicolike.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mp.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kn.9csxet.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ne.huanxung.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ln.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gn.bjjhwx.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://iy.yuexingan06.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://st.nicolike.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ue.huixinmuqiang.cn

[L03] 设置自定义请求头
来源：http://dr.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yy.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://va.colortex.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jt.shtwfgs.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ex.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xb.hnjuh.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yq.hahajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bd.shtwfgs.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ua.muxihuayi.cn

[L04] 设置超时
来源：http://zj.huixinmuqiang.cn

Py:   requests.get(url, timeout=5)
来源：http://nv.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ap.gzmigu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://id.shtwfgs.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vx.shxzskj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jk.nszjky.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mx.muxihuayi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ra.szxytkj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vc.haigaiapp.cn

[L05] 上传文件（multipart）
来源：http://ra.jianghongdianzi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gy.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cv.hnjuh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rm.szsharing.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xy.szxytkj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jg.wgjwhj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pd.shtwfgs.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zr.huixiangedu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bi.szsharing.cn

[L06] 解析响应为 JSON
来源：http://ck.yuexingan06.cn

Py:   resp.json()
来源：http://fu.wgjwhj.cn

PHP:  json_decode($body, true);
来源：http://me.chemitech.net.cn

JS:   await resp.json()
来源：http://vx.wgjwhj.cn

TS:   await resp.json()
来源：http://vm.shtwfgs.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://eu.huanxung.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ya.nszjky.cn

Ruby: JSON.parse(resp.body)
来源：http://fp.yuexingan06.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ox.shtwfgs.cn

[L07] 处理 HTTP 状态码
来源：http://at.muxihuayi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ly.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dx.nicolike.cn

JS:   resp.ok;  resp.status
来源：http://mp.huanxung.cn

TS:   resp.ok;  resp.status
来源：http://kw.shxzskj.cn

Java: resp.statusCode()
来源：http://zx.521024.cn

Go:   resp.StatusCode
来源：http://yc.shxzskj.cn

Ruby: resp.code.to_i
来源：http://hq.panjiajie.cn

C#:   (int)resp.StatusCode
来源：http://qw.muxihuayi.cn

[L08] 并发请求多个地址
来源：http://ee.panjiajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wp.lnxyls.cn

PHP:  curl_multi_init() 系列
来源：http://nm.chemitech.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lj.asd995.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://af.szsharing.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zd.colortex.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kt.bookmarksfly.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hf.jianghongdianzi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://es.huixinmuqiang.cn

================================================================================
来源：http://iz.asd995.cn

M. 命令行 / 进程 / 环境
来源：http://yg.muxihuayi.cn

================================================================================
来源：http://jz.yuexingan06.cn

[M01] 读取命令行参数
来源：http://dl.panjiajie.cn

Py:   sys.argv[1:]
来源：http://gf.shxzskj.cn

PHP:  $argv;  $argc;
来源：http://vg.nszjky.cn

JS:   process.argv.slice(2)
来源：http://td.bjjhwx.cn

TS:   process.argv.slice(2)
来源：http://zv.jctech888.com.cn

Java: args 数组（main 方法参数）
来源：http://kh.huixinmuqiang.cn

Go:   os.Args[1:]
来源：http://bf.shtwfgs.cn

Ruby: ARGV
来源：http://ua.asd995.cn

C#:   args 数组（Main 方法参数）
来源：http://jc.huixinmuqiang.cn

[M02] 读取环境变量
来源：http://xq.shxzskj.cn

Py:   os.environ.get("HOME")
来源：http://zq.asd995.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mb.asd995.cn

JS:   process.env.HOME
来源：http://pa.asd995.cn

TS:   process.env.HOME
来源：http://rv.asd995.cn

Java: System.getenv("HOME")
来源：http://ff.newstarts.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kr.shxzskj.cn

Ruby: ENV["HOME"]
来源：http://mp.szxytkj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ri.jianghongdianzi.cn

[M03] 执行外部命令
来源：http://zk.nszjky.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://sc.huixiangedu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jj.lnxyls.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ke.szxytkj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mx.lnxyls.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hc.chemitech.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dw.panjiajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://mc.jctech888.com.cn

C#:   Process.Start("ls", "-l");
来源：http://kb.gzmigu.cn

[M04] 获取当前工作目录
来源：http://ph.hnjuh.cn

Py:   os.getcwd()
来源：http://zw.muxihuayi.cn

PHP:  getcwd();
来源：http://cj.lnxyls.cn

JS:   process.cwd()
来源：http://ij.huixiangedu.cn

TS:   process.cwd()
来源：http://xe.muxihuayi.cn

Java: Path.of("").toAbsolutePath()
来源：http://ya.nicolike.cn

Go:   os.Getwd()
来源：http://bt.colortex.cn

Ruby: Dir.pwd
来源：http://tg.huixiangedu.cn


<!-- 参考信息 -->