代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://oq.nicolike.cn

TS:   /error/gim
来源：http://rh.panjiajie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bi.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vo.szsharing.cn

Ruby: s.scan(/error/i)
来源：http://wh.huixinmuqiang.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hm.521024.cn

[I08] 贪婪与非贪婪匹配
来源：http://bn.asd995.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lo.nicolike.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ts.muxihuayi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ad.muxihuayi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zq.yuexingan06.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://jp.gzmigu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://to.muxihuayi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dz.szxytkj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dj.muxihuayi.cn

================================================================================
来源：http://bm.huanxung.cn

J. 日期与时间
来源：http://kf.gzmigu.cn

================================================================================
来源：http://mq.huixiangedu.cn

[J01] 获取当前时间
来源：http://pg.shxzskj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lf.asd995.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dl.jianghongdianzi.cn

JS:   new Date();  Date.now()
来源：http://ln.gzmigu.cn

TS:   new Date();  Date.now()
来源：http://iq.521024.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mc.newstarts.cn

Go:   time.Now()
来源：http://mg.shxzskj.cn

Ruby: Time.now
来源：http://mo.huanxung.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rb.nszjky.cn

[J02] 格式化输出
来源：http://ta.newstarts.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gz.lnxyls.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://th.wgjwhj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xc.jianghongdianzi.cn

TS:   d.toISOString()
来源：http://ao.muxihuayi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dy.lnxyls.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vk.newstarts.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rt.bjjhwx.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jq.9csxet.cn

[J03] 字符串解析为日期
来源：http://ix.hnjuh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lg.nszjky.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qu.lnxyls.cn

JS:   new Date("2024-01-02")
来源：http://yw.haigaiapp.cn

TS:   new Date("2024-01-02")
来源：http://wb.gzmigu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fy.hnjuh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dj.wgjwhj.cn

Ruby: Date.parse("2024-01-02")
来源：http://ys.yuexingan06.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ah.szxytkj.cn

[J04] 时间戳与日期互转
来源：http://gb.panjiajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bx.muxihuayi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://re.muxihuayi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ka.huixinmuqiang.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dh.shxzukj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ie.shxzskj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vx.hnjuh.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cc.jianghongdianzi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nr.shxzukj.cn

[J05] 时间加减（加 7 天）
来源：http://qs.hahajie.cn

Py:   now + timedelta(days=7)
来源：http://ul.huixinmuqiang.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://hk.muxihuayi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ns.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ea.shxzukj.cn

Java: LocalDate.now().plusDays(7)
来源：http://df.yuntaijiaju.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bn.newstarts.cn

Ruby: Time.now + 7 * 86400
来源：http://yw.wgjwhj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hp.nicolike.cn

[J06] 计算两时间之差
来源：http://io.shxzukj.cn

Py:   (end - start).total_seconds()
来源：http://nr.szxytkj.cn

PHP:  $end->diff($start)->days;
来源：http://ux.hahajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vn.haigaiapp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wz.szsharing.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vj.gzmigu.cn

Go:   end.Sub(start).Hours()
来源：http://zr.jctech888.com.cn

Ruby: end - start                 # 返回秒数
来源：http://pm.yuntaijiaju.cn

C#:   (end - start).TotalSeconds
来源：http://pm.shxzskj.cn

[J07] 比较两个日期
来源：http://me.wgjwhj.cn

Py:   d1 < d2;  d1 == d2
来源：http://xk.nicolike.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://en.asd995.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jq.szsharing.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bj.nszjky.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hh.bookmarksfly.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hs.521024.cn

Ruby: d1 < d2;  d1 == d2
来源：http://sh.shtwfgs.cn

C#:   d1 < d2;  d1 == d2
来源：http://vb.gzmigu.cn

[J08] 提取年月日与星期
来源：http://zx.asd995.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gj.wgjwhj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nu.szsharing.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vt.yuexingan06.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://od.nicolike.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ha.szsharing.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://or.yuntaijiaju.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cx.huixinmuqiang.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lh.szsharing.cn

[J09] 时区处理
来源：http://db.hahajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dx.huanxung.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xu.bookmarksfly.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://do.9csxet.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wi.shxzskj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jf.bjjhwx.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dm.huixiangedu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://sj.huixiangedu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uw.panjiajie.cn

[J10] 取今天 / 本月第一天
来源：http://oe.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vx.shxzskj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yn.wgjwhj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xj.hnjuh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cr.bookmarksfly.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dk.chemitech.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dr.yuexingan06.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ve.huixiangedu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lz.szxytkj.cn

================================================================================
来源：http://pr.huanxung.cn

K. JSON 与序列化
来源：http://xn.9csxet.cn

================================================================================
来源：http://ws.asd995.cn

[K01] 对象转 JSON 字符串
来源：http://om.huixiangedu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://je.haigaiapp.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gl.newstarts.cn

JS:   JSON.stringify(obj)
来源：http://ed.huixinmuqiang.cn

TS:   JSON.stringify(obj)
来源：http://xo.jianghongdianzi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zb.nicolike.cn

Go:   json.Marshal(obj)
来源：http://sh.wgjwhj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qz.huanxung.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jl.shxzukj.cn

[K02] JSON 字符串转对象
来源：http://lc.colortex.cn

Py:   json.loads(s)
来源：http://si.nszjky.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fp.haigaiapp.cn

JS:   JSON.parse(s)
来源：http://ih.yuexingan06.cn

TS:   JSON.parse(s)
来源：http://ey.521024.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ic.newstarts.cn

Go:   json.Unmarshal(data, &v)
来源：http://ip.szxytkj.cn

Ruby: JSON.parse(s)
来源：http://rz.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ky.9csxet.cn

[K03] JSON 美化输出（带缩进）
来源：http://su.yuexingan06.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mt.shxzskj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dv.nicolike.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bu.jianghongdianzi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ta.bookmarksfly.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pc.hahajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nm.shtwfgs.cn

Ruby: JSON.pretty_generate(obj)
来源：http://oc.lnxyls.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nw.521024.cn

[K04] 读取 JSON 文件
来源：http://gl.newstarts.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rb.9csxet.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gr.huanxung.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gg.lnxyls.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pq.yuexingan06.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://df.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xh.chemitech.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://uf.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rq.bookmarksfly.cn

[K05] 深拷贝对象
来源：http://qw.lnxyls.cn

Py:   copy.deepcopy(obj)
来源：http://xi.wgjwhj.cn

PHP:  unserialize(serialize($obj));
来源：http://wh.chemitech.net.cn

JS:   structuredClone(obj)
来源：http://fw.lnxyls.cn

TS:   structuredClone(obj)
来源：http://zz.hahajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ob.chemitech.net.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qk.lnxyls.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jl.haigaiapp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://iu.szxytkj.cn

[K06] 解析 URL 查询串
来源：http://nc.shtwfgs.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ci.haigaiapp.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pz.lnxyls.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iq.bjjhwx.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eb.shxzukj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://un.wgjwhj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://co.huanxung.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mj.panjiajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zv.lnxyls.cn

[K07] 进制转换
来源：http://ri.gzmigu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ak.nicolike.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vp.haigaiapp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://po.9csxet.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gg.huixiangedu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ic.nszjky.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ef.colortex.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cj.wgjwhj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xd.chemitech.net.cn

[K08] 二进制序列化（非 JSON）
来源：http://at.hahajie.cn

Py:   pickle.dumps(obj)
来源：http://hc.szsharing.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zn.hahajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://px.huixinmuqiang.cn

TS:   v8.serialize(obj)        // Node
来源：http://lb.shxzukj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ar.shxzukj.cn

Go:   encoding/gob
来源：http://er.lnxyls.cn

Ruby: Marshal.dump(obj)
来源：http://eg.huanxung.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cu.szxytkj.cn

================================================================================
来源：http://gd.huanxung.cn

L. 网络请求
来源：http://aw.huixiangedu.cn

================================================================================
来源：http://kf.jianghongdianzi.cn

[L01] 发送 GET 请求
来源：http://mt.newstarts.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tl.jctech888.com.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zg.huixiangedu.cn

JS:   await fetch(url)
来源：http://lk.bjjhwx.cn

TS:   await fetch(url)
来源：http://ys.panjiajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ck.hnjuh.cn

Go:   resp, err := http.Get(url)
来源：http://kw.bjjhwx.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pv.bjjhwx.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mx.muxihuayi.cn

[L02] 发送 POST JSON
来源：http://uq.hahajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hg.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vb.colortex.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ej.szxytkj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fv.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ro.asd995.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xh.asd995.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://un.huixinmuqiang.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cq.huixinmuqiang.cn

[L03] 设置自定义请求头
来源：http://zy.lnxyls.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rk.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qj.gzmigu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nz.hnjuh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://on.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yw.wgjwhj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vw.haigaiapp.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ij.bjjhwx.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wh.gzmigu.cn

[L04] 设置超时
来源：http://uh.bjjhwx.cn

Py:   requests.get(url, timeout=5)
来源：http://za.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sj.lnxyls.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lj.jctech888.com.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wo.lnxyls.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sp.bookmarksfly.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gm.bookmarksfly.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sm.huixinmuqiang.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hk.huixinmuqiang.cn

[L05] 上传文件（multipart）
来源：http://an.muxihuayi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sg.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cf.newstarts.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ez.lnxyls.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ir.bookmarksfly.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xd.yuexingan06.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uo.hahajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dp.huixiangedu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://to.huixiangedu.cn

[L06] 解析响应为 JSON
来源：http://ym.gzmigu.cn

Py:   resp.json()
来源：http://lc.bookmarksfly.cn

PHP:  json_decode($body, true);
来源：http://dy.panjiajie.cn

JS:   await resp.json()
来源：http://zr.huixinmuqiang.cn

TS:   await resp.json()
来源：http://ua.shxzskj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://li.panjiajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ma.newstarts.cn

Ruby: JSON.parse(resp.body)
来源：http://bm.yuexingan06.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nx.haigaiapp.cn

[L07] 处理 HTTP 状态码
来源：http://in.bjjhwx.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://di.gzmigu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://np.lnxyls.cn

JS:   resp.ok;  resp.status
来源：http://sj.asd995.cn

TS:   resp.ok;  resp.status
来源：http://ll.lnxyls.cn

Java: resp.statusCode()
来源：http://dx.yuexingan06.cn

Go:   resp.StatusCode
来源：http://km.lnxyls.cn

Ruby: resp.code.to_i
来源：http://pc.lnxyls.cn

C#:   (int)resp.StatusCode
来源：http://lu.shxzskj.cn

[L08] 并发请求多个地址
来源：http://pr.shxzskj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://iz.yuntaijiaju.cn

PHP:  curl_multi_init() 系列
来源：http://jm.shtwfgs.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rk.9csxet.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ix.szsharing.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dq.szxytkj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vf.yuntaijiaju.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ol.huanxung.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ft.9csxet.cn

================================================================================
来源：http://dq.haigaiapp.cn

M. 命令行 / 进程 / 环境
来源：http://hd.9csxet.cn

================================================================================
来源：http://lg.huixiangedu.cn

[M01] 读取命令行参数
来源：http://be.shxzskj.cn

Py:   sys.argv[1:]
来源：http://ke.shxzskj.cn

PHP:  $argv;  $argc;
来源：http://pv.haigaiapp.cn

JS:   process.argv.slice(2)
来源：http://nz.wgjwhj.cn

TS:   process.argv.slice(2)
来源：http://xj.yuntaijiaju.cn

Java: args 数组（main 方法参数）
来源：http://fh.yuntaijiaju.cn

Go:   os.Args[1:]
来源：http://wp.huanxung.cn

Ruby: ARGV
来源：http://wd.shtwfgs.cn

C#:   args 数组（Main 方法参数）
来源：http://lc.muxihuayi.cn

[M02] 读取环境变量
来源：http://ou.panjiajie.cn

Py:   os.environ.get("HOME")
来源：http://up.gzmigu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qj.haigaiapp.cn

JS:   process.env.HOME
来源：http://em.bjjhwx.cn

TS:   process.env.HOME
来源：http://ju.huanxung.cn

Java: System.getenv("HOME")
来源：http://zl.asd995.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rf.bookmarksfly.cn

Ruby: ENV["HOME"]
来源：http://cn.bjjhwx.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xw.newstarts.cn

[M03] 执行外部命令
来源：http://oc.bjjhwx.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ea.lnxyls.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ja.huixinmuqiang.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://uh.szsharing.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ln.newstarts.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cu.nszjky.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fj.wgjwhj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://aa.huanxung.cn

C#:   Process.Start("ls", "-l");
来源：http://as.huanxung.cn

[M04] 获取当前工作目录
来源：http://ky.colortex.cn

Py:   os.getcwd()
来源：http://am.yuexingan06.cn

PHP:  getcwd();
来源：http://dl.shxzukj.cn

JS:   process.cwd()
来源：http://xv.hnjuh.cn

TS:   process.cwd()
来源：http://yj.nszjky.cn

Java: Path.of("").toAbsolutePath()
来源：http://wi.asd995.cn

Go:   os.Getwd()
来源：http://ti.huanxung.cn

Ruby: Dir.pwd
来源：http://yo.yuexingan06.cn

C#:   Directory.GetCurrentDirectory()
来源：http://su.521024.cn

[M05] 设置退出码
来源：http://fc.huixinmuqiang.cn

Py:   sys.exit(1)
来源：http://hx.wgjwhj.cn

PHP:  exit(1);
来源：http://ae.hahajie.cn


<!-- 参考信息 -->