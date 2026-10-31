代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rd.hnjuh.cn

TS:   /error/gim
来源：http://fi.yuexingan06.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tr.nicolike.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ne.wgjwhj.cn

Ruby: s.scan(/error/i)
来源：http://pi.bookmarksfly.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rr.panjiajie.cn

[I08] 贪婪与非贪婪匹配
来源：http://st.jctech888.com.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fc.bookmarksfly.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kp.jianghongdianzi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nz.jianghongdianzi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://it.shxzskj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vm.newstarts.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sf.gzmigu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ic.521024.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ey.shtwfgs.cn

================================================================================
来源：http://ud.shtwfgs.cn

J. 日期与时间
来源：http://ts.newstarts.cn

================================================================================
来源：http://qn.colortex.cn

[J01] 获取当前时间
来源：http://vb.gzmigu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pa.shxzukj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pu.newstarts.cn

JS:   new Date();  Date.now()
来源：http://xl.shxzukj.cn

TS:   new Date();  Date.now()
来源：http://iu.haigaiapp.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mg.nicolike.cn

Go:   time.Now()
来源：http://qf.hahajie.cn

Ruby: Time.now
来源：http://yd.colortex.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vs.521024.cn

[J02] 格式化输出
来源：http://qm.hnjuh.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uf.jctech888.com.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ks.shxzukj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bc.muxihuayi.cn

TS:   d.toISOString()
来源：http://sr.nicolike.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lp.wgjwhj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cn.huixiangedu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://to.jianghongdianzi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xj.jianghongdianzi.cn

[J03] 字符串解析为日期
来源：http://yq.yuntaijiaju.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wc.shxzskj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ys.huanxung.cn

JS:   new Date("2024-01-02")
来源：http://fa.huixinmuqiang.cn

TS:   new Date("2024-01-02")
来源：http://hj.muxihuayi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ez.jctech888.com.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vv.shtwfgs.cn

Ruby: Date.parse("2024-01-02")
来源：http://cg.nszjky.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ps.bookmarksfly.cn

[J04] 时间戳与日期互转
来源：http://ny.haigaiapp.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://eq.haigaiapp.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pb.asd995.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yq.panjiajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tf.panjiajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dl.hahajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://so.lnxyls.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kt.jianghongdianzi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zh.asd995.cn

[J05] 时间加减（加 7 天）
来源：http://no.nicolike.cn

Py:   now + timedelta(days=7)
来源：http://np.521024.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zp.shxzskj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xa.nszjky.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://on.yuexingan06.cn

Java: LocalDate.now().plusDays(7)
来源：http://ep.asd995.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dy.hnjuh.cn

Ruby: Time.now + 7 * 86400
来源：http://zn.newstarts.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jc.lnxyls.cn

[J06] 计算两时间之差
来源：http://vq.asd995.cn

Py:   (end - start).total_seconds()
来源：http://tz.wgjwhj.cn

PHP:  $end->diff($start)->days;
来源：http://ux.szsharing.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ag.chemitech.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zl.9csxet.cn

Java: Duration.between(start, end).toSeconds()
来源：http://yy.521024.cn

Go:   end.Sub(start).Hours()
来源：http://lt.yuntaijiaju.cn

Ruby: end - start                 # 返回秒数
来源：http://dv.shxzskj.cn

C#:   (end - start).TotalSeconds
来源：http://gg.hahajie.cn

[J07] 比较两个日期
来源：http://lr.huixiangedu.cn

Py:   d1 < d2;  d1 == d2
来源：http://zi.nicolike.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pj.shtwfgs.cn

JS:   d1.getTime() < d2.getTime()
来源：http://li.panjiajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fl.9csxet.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ep.shxzukj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xm.9csxet.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ce.huixinmuqiang.cn

C#:   d1 < d2;  d1 == d2
来源：http://ic.newstarts.cn

[J08] 提取年月日与星期
来源：http://js.panjiajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fc.lnxyls.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dg.asd995.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jl.newstarts.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ty.shxzskj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ui.huixiangedu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ea.muxihuayi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sk.gzmigu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uy.huixinmuqiang.cn

[J09] 时区处理
来源：http://ws.521024.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pz.szsharing.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kt.huixiangedu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qs.521024.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mo.nszjky.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nq.nicolike.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://py.colortex.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://sg.hnjuh.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dy.hahajie.cn

[J10] 取今天 / 本月第一天
来源：http://uw.bookmarksfly.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://yr.huixiangedu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wu.jianghongdianzi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uo.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pr.huixiangedu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zk.gzmigu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://am.haigaiapp.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uo.nszjky.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mj.huanxung.cn

================================================================================
来源：http://mt.muxihuayi.cn

K. JSON 与序列化
来源：http://gr.szxytkj.cn

================================================================================
来源：http://cn.yuexingan06.cn

[K01] 对象转 JSON 字符串
来源：http://ly.bjjhwx.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pm.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fu.chemitech.net.cn

JS:   JSON.stringify(obj)
来源：http://dz.bjjhwx.cn

TS:   JSON.stringify(obj)
来源：http://le.huixinmuqiang.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xt.yuntaijiaju.cn

Go:   json.Marshal(obj)
来源：http://nk.colortex.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fe.hahajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://df.jctech888.com.cn

[K02] JSON 字符串转对象
来源：http://uh.muxihuayi.cn

Py:   json.loads(s)
来源：http://pj.jctech888.com.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://be.szsharing.cn

JS:   JSON.parse(s)
来源：http://bk.gzmigu.cn

TS:   JSON.parse(s)
来源：http://hn.szsharing.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rp.chemitech.net.cn

Go:   json.Unmarshal(data, &v)
来源：http://mt.huixiangedu.cn

Ruby: JSON.parse(s)
来源：http://uk.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xn.asd995.cn

[K03] JSON 美化输出（带缩进）
来源：http://ra.szsharing.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://di.shxzskj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gy.chemitech.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://cv.yuntaijiaju.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ub.wgjwhj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dl.muxihuayi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xi.asd995.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ju.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cc.szxytkj.cn

[K04] 读取 JSON 文件
来源：http://lz.hahajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lm.huixiangedu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ab.muxihuayi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tj.lnxyls.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://se.jctech888.com.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://oh.hahajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gz.szsharing.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ei.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tm.chemitech.net.cn

[K05] 深拷贝对象
来源：http://up.colortex.cn

Py:   copy.deepcopy(obj)
来源：http://mr.nszjky.cn

PHP:  unserialize(serialize($obj));
来源：http://sy.muxihuayi.cn

JS:   structuredClone(obj)
来源：http://fi.haigaiapp.cn

TS:   structuredClone(obj)
来源：http://kr.szsharing.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://so.lnxyls.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gt.yuexingan06.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vw.haigaiapp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xg.szsharing.cn

[K06] 解析 URL 查询串
来源：http://qe.jctech888.com.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jr.yuntaijiaju.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fg.bookmarksfly.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gt.gzmigu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pl.nszjky.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dd.huanxung.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ot.9csxet.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cu.jctech888.com.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yn.hahajie.cn

[K07] 进制转换
来源：http://yh.jianghongdianzi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gq.szsharing.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nc.szxytkj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qa.muxihuayi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://he.jianghongdianzi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pu.haigaiapp.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://im.shxzskj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ht.huixinmuqiang.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sf.szsharing.cn

[K08] 二进制序列化（非 JSON）
来源：http://pq.gzmigu.cn

Py:   pickle.dumps(obj)
来源：http://al.gzmigu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ub.bjjhwx.cn

JS:   v8.serialize(obj)        // Node
来源：http://aw.nicolike.cn

TS:   v8.serialize(obj)        // Node
来源：http://jd.bjjhwx.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cz.lnxyls.cn

Go:   encoding/gob
来源：http://wa.huixinmuqiang.cn

Ruby: Marshal.dump(obj)
来源：http://mr.muxihuayi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rg.9csxet.cn

================================================================================
来源：http://hx.hahajie.cn

L. 网络请求
来源：http://ls.nszjky.cn

================================================================================
来源：http://fs.gzmigu.cn

[L01] 发送 GET 请求
来源：http://ga.szsharing.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pp.lnxyls.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kc.shxzukj.cn

JS:   await fetch(url)
来源：http://ek.hahajie.cn

TS:   await fetch(url)
来源：http://db.shxzukj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hk.bookmarksfly.cn

Go:   resp, err := http.Get(url)
来源：http://re.yuexingan06.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://kz.nszjky.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ht.521024.cn

[L02] 发送 POST JSON
来源：http://ea.muxihuayi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wk.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mf.chemitech.net.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uv.wgjwhj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://id.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tm.bookmarksfly.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ou.yuexingan06.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fe.hahajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qb.hahajie.cn

[L03] 设置自定义请求头
来源：http://ej.wgjwhj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ya.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://in.shtwfgs.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ev.521024.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ac.asd995.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ce.9csxet.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ex.yuexingan06.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pk.yuexingan06.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://iv.asd995.cn

[L04] 设置超时
来源：http://xe.yuexingan06.cn

Py:   requests.get(url, timeout=5)
来源：http://wq.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xz.lnxyls.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cp.haigaiapp.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sb.colortex.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fr.chemitech.net.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ld.bookmarksfly.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ja.jctech888.com.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dk.521024.cn

[L05] 上传文件（multipart）
来源：http://qm.lnxyls.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dq.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qx.hnjuh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dt.panjiajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vg.asd995.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gn.newstarts.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pm.bjjhwx.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vc.9csxet.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://re.muxihuayi.cn

[L06] 解析响应为 JSON
来源：http://op.nszjky.cn

Py:   resp.json()
来源：http://dg.huixinmuqiang.cn

PHP:  json_decode($body, true);
来源：http://wq.gzmigu.cn

JS:   await resp.json()
来源：http://gz.bookmarksfly.cn

TS:   await resp.json()
来源：http://fx.shxzukj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yb.haigaiapp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.haigaiapp.cn

Ruby: JSON.parse(resp.body)
来源：http://mz.bookmarksfly.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mg.yuntaijiaju.cn

[L07] 处理 HTTP 状态码
来源：http://xg.hnjuh.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://my.huixiangedu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fa.newstarts.cn

JS:   resp.ok;  resp.status
来源：http://nr.bookmarksfly.cn

TS:   resp.ok;  resp.status
来源：http://cl.haigaiapp.cn

Java: resp.statusCode()
来源：http://zl.haigaiapp.cn

Go:   resp.StatusCode
来源：http://mo.huixiangedu.cn

Ruby: resp.code.to_i
来源：http://eq.yuexingan06.cn

C#:   (int)resp.StatusCode
来源：http://wc.huixinmuqiang.cn

[L08] 并发请求多个地址
来源：http://tq.hnjuh.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gq.szxytkj.cn

PHP:  curl_multi_init() 系列
来源：http://rn.hahajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://je.nszjky.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zv.jianghongdianzi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wj.chemitech.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://to.yuexingan06.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yu.hnjuh.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://na.9csxet.cn

================================================================================
来源：http://hj.asd995.cn

M. 命令行 / 进程 / 环境
来源：http://ef.szsharing.cn

================================================================================
来源：http://jt.bjjhwx.cn

[M01] 读取命令行参数
来源：http://zx.521024.cn

Py:   sys.argv[1:]
来源：http://kv.shxzskj.cn

PHP:  $argv;  $argc;
来源：http://th.asd995.cn

JS:   process.argv.slice(2)
来源：http://kg.muxihuayi.cn

TS:   process.argv.slice(2)
来源：http://vs.bookmarksfly.cn

Java: args 数组（main 方法参数）
来源：http://ku.lnxyls.cn

Go:   os.Args[1:]
来源：http://eb.9csxet.cn

Ruby: ARGV
来源：http://rl.huixinmuqiang.cn

C#:   args 数组（Main 方法参数）
来源：http://ik.bookmarksfly.cn

[M02] 读取环境变量
来源：http://oc.jctech888.com.cn

Py:   os.environ.get("HOME")
来源：http://vu.panjiajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://la.chemitech.net.cn

JS:   process.env.HOME
来源：http://uy.chemitech.net.cn

TS:   process.env.HOME
来源：http://ex.panjiajie.cn

Java: System.getenv("HOME")
来源：http://db.shxzukj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qr.bookmarksfly.cn

Ruby: ENV["HOME"]
来源：http://hb.521024.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://av.szsharing.cn

[M03] 执行外部命令
来源：http://ti.bookmarksfly.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ws.huixinmuqiang.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ne.shxzukj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://tm.wgjwhj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ud.yuexingan06.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nk.panjiajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qc.szsharing.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ym.haigaiapp.cn

C#:   Process.Start("ls", "-l");
来源：http://qh.chemitech.net.cn

[M04] 获取当前工作目录
来源：http://tj.newstarts.cn

Py:   os.getcwd()
来源：http://di.chemitech.net.cn

PHP:  getcwd();
来源：http://uc.wgjwhj.cn

JS:   process.cwd()
来源：http://dt.shtwfgs.cn

TS:   process.cwd()
来源：http://gq.huanxung.cn

Java: Path.of("").toAbsolutePath()
来源：http://nu.hnjuh.cn

Go:   os.Getwd()
来源：http://md.szsharing.cn

Ruby: Dir.pwd
来源：http://sn.asd995.cn

C#:   Directory.GetCurrentDirectory()
来源：http://lo.hahajie.cn

[M05] 设置退出码
来源：http://cs.huixinmuqiang.cn

Py:   sys.exit(1)
来源：http://ef.muxihuayi.cn

PHP:  exit(1);
来源：http://rp.newstarts.cn


<!-- 参考信息 -->