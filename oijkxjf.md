代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lm.nszjky.cn

TS:   /error/gim
来源：http://ck.521024.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tl.jianghongdianzi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yc.huanxung.cn

Ruby: s.scan(/error/i)
来源：http://ln.huixiangedu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wp.jctech888.com.cn

[I08] 贪婪与非贪婪匹配
来源：http://sa.9csxet.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vx.newstarts.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://or.hahajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bm.szsharing.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fv.asd995.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ee.yuntaijiaju.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ep.chemitech.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ha.colortex.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ja.panjiajie.cn

================================================================================
来源：http://js.shxzskj.cn

J. 日期与时间
来源：http://fx.gzmigu.cn

================================================================================
来源：http://tn.bookmarksfly.cn

[J01] 获取当前时间
来源：http://lb.yuntaijiaju.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://gc.newstarts.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ow.szxytkj.cn

JS:   new Date();  Date.now()
来源：http://bt.shxzskj.cn

TS:   new Date();  Date.now()
来源：http://jr.huixinmuqiang.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jt.szsharing.cn

Go:   time.Now()
来源：http://fn.nicolike.cn

Ruby: Time.now
来源：http://kw.haigaiapp.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mv.hahajie.cn

[J02] 格式化输出
来源：http://ft.yuntaijiaju.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iq.hahajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kq.shxzukj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zk.huanxung.cn

TS:   d.toISOString()
来源：http://ox.haigaiapp.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ei.yuexingan06.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://av.yuntaijiaju.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yg.shxzskj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sl.shtwfgs.cn

[J03] 字符串解析为日期
来源：http://tg.haigaiapp.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nh.szxytkj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pb.huixinmuqiang.cn

JS:   new Date("2024-01-02")
来源：http://di.nszjky.cn

TS:   new Date("2024-01-02")
来源：http://qp.jianghongdianzi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zn.shxzukj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lv.muxihuayi.cn

Ruby: Date.parse("2024-01-02")
来源：http://wb.muxihuayi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xe.huixiangedu.cn

[J04] 时间戳与日期互转
来源：http://xq.newstarts.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mq.huixinmuqiang.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pv.shtwfgs.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rs.chemitech.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ng.nszjky.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fd.asd995.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uu.asd995.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rf.shxzskj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tr.lnxyls.cn

[J05] 时间加减（加 7 天）
来源：http://bp.huixinmuqiang.cn

Py:   now + timedelta(days=7)
来源：http://hz.bookmarksfly.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://dy.chemitech.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gv.newstarts.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fm.nszjky.cn

Java: LocalDate.now().plusDays(7)
来源：http://dz.huixiangedu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tq.szxytkj.cn

Ruby: Time.now + 7 * 86400
来源：http://kr.521024.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xh.haigaiapp.cn

[J06] 计算两时间之差
来源：http://dj.colortex.cn

Py:   (end - start).total_seconds()
来源：http://kc.nicolike.cn

PHP:  $end->diff($start)->days;
来源：http://yk.shxzukj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ls.hahajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ce.muxihuayi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zi.lnxyls.cn

Go:   end.Sub(start).Hours()
来源：http://ov.newstarts.cn

Ruby: end - start                 # 返回秒数
来源：http://pn.nicolike.cn

C#:   (end - start).TotalSeconds
来源：http://dx.haigaiapp.cn

[J07] 比较两个日期
来源：http://cv.jianghongdianzi.cn

Py:   d1 < d2;  d1 == d2
来源：http://zt.shtwfgs.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xh.shxzukj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xv.panjiajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qo.wgjwhj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vd.hahajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://eq.wgjwhj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ez.muxihuayi.cn

C#:   d1 < d2;  d1 == d2
来源：http://jf.haigaiapp.cn

[J08] 提取年月日与星期
来源：http://aj.lnxyls.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qn.shtwfgs.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mg.huanxung.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xq.muxihuayi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gx.haigaiapp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cp.chemitech.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pw.huixinmuqiang.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lr.haigaiapp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ee.9csxet.cn

[J09] 时区处理
来源：http://eu.szxytkj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ns.wgjwhj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://uh.yuntaijiaju.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://og.jianghongdianzi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vh.haigaiapp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kc.asd995.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qq.hahajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vr.bjjhwx.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kf.yuntaijiaju.cn

[J10] 取今天 / 本月第一天
来源：http://hq.shxzskj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bp.huixinmuqiang.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pc.szsharing.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sl.shxzskj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wa.9csxet.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dz.nicolike.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://la.szxytkj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jh.hahajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lp.muxihuayi.cn

================================================================================
来源：http://ca.wgjwhj.cn

K. JSON 与序列化
来源：http://ex.9csxet.cn

================================================================================
来源：http://tk.jianghongdianzi.cn

[K01] 对象转 JSON 字符串
来源：http://zg.jianghongdianzi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bt.bookmarksfly.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rl.shtwfgs.cn

JS:   JSON.stringify(obj)
来源：http://sq.szsharing.cn

TS:   JSON.stringify(obj)
来源：http://oi.gzmigu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yz.hnjuh.cn

Go:   json.Marshal(obj)
来源：http://ag.muxihuayi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://my.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rm.colortex.cn

[K02] JSON 字符串转对象
来源：http://wg.521024.cn

Py:   json.loads(s)
来源：http://cb.bjjhwx.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ga.nicolike.cn

JS:   JSON.parse(s)
来源：http://ct.muxihuayi.cn

TS:   JSON.parse(s)
来源：http://il.9csxet.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jd.shxzskj.cn

Go:   json.Unmarshal(data, &v)
来源：http://xs.huixinmuqiang.cn

Ruby: JSON.parse(s)
来源：http://bc.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uq.shxzukj.cn

[K03] JSON 美化输出（带缩进）
来源：http://dz.szsharing.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fl.shxzukj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kx.nszjky.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hd.bookmarksfly.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gt.nicolike.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zg.colortex.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wx.yuexingan06.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ex.nicolike.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fo.bookmarksfly.cn

[K04] 读取 JSON 文件
来源：http://iw.521024.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fd.hahajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ef.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hs.jctech888.com.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dh.newstarts.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kp.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bd.wgjwhj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ft.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://oe.nicolike.cn

[K05] 深拷贝对象
来源：http://pb.jctech888.com.cn

Py:   copy.deepcopy(obj)
来源：http://do.shtwfgs.cn

PHP:  unserialize(serialize($obj));
来源：http://te.chemitech.net.cn

JS:   structuredClone(obj)
来源：http://ot.yuntaijiaju.cn

TS:   structuredClone(obj)
来源：http://sl.chemitech.net.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fb.chemitech.net.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pe.huanxung.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dd.shxzukj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ky.jianghongdianzi.cn

[K06] 解析 URL 查询串
来源：http://xg.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cc.bjjhwx.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ud.shtwfgs.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yb.haigaiapp.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ye.hnjuh.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pq.hnjuh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cw.huixinmuqiang.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qf.bjjhwx.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://md.shtwfgs.cn

[K07] 进制转换
来源：http://ht.bjjhwx.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sd.panjiajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://le.shxzukj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ms.wgjwhj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ua.hahajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vn.shtwfgs.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qk.nicolike.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yv.shtwfgs.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ij.jianghongdianzi.cn

[K08] 二进制序列化（非 JSON）
来源：http://bg.shtwfgs.cn

Py:   pickle.dumps(obj)
来源：http://mv.lnxyls.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fx.newstarts.cn

JS:   v8.serialize(obj)        // Node
来源：http://rq.521024.cn

TS:   v8.serialize(obj)        // Node
来源：http://vz.szxytkj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sj.9csxet.cn

Go:   encoding/gob
来源：http://pq.asd995.cn

Ruby: Marshal.dump(obj)
来源：http://mv.shxzskj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jk.shtwfgs.cn

================================================================================
来源：http://mj.jctech888.com.cn

L. 网络请求
来源：http://mz.shxzskj.cn

================================================================================
来源：http://oc.shxzskj.cn

[L01] 发送 GET 请求
来源：http://qc.gzmigu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ik.9csxet.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xt.asd995.cn

JS:   await fetch(url)
来源：http://ov.shxzukj.cn

TS:   await fetch(url)
来源：http://bd.huixiangedu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ri.chemitech.net.cn

Go:   resp, err := http.Get(url)
来源：http://gg.yuntaijiaju.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://es.lnxyls.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bj.yuexingan06.cn

[L02] 发送 POST JSON
来源：http://ut.nszjky.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wh.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xt.shxzukj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gm.shxzukj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ku.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ff.szxytkj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mf.bookmarksfly.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://on.gzmigu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ve.jctech888.com.cn

[L03] 设置自定义请求头
来源：http://rx.haigaiapp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sd.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xq.hahajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lu.wgjwhj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eb.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lh.huanxung.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lp.huixinmuqiang.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ke.hahajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://iz.yuntaijiaju.cn

[L04] 设置超时
来源：http://uz.colortex.cn

Py:   requests.get(url, timeout=5)
来源：http://ma.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hq.huanxung.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gk.haigaiapp.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fp.yuntaijiaju.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gv.jctech888.com.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dc.muxihuayi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cm.hnjuh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cv.jctech888.com.cn

[L05] 上传文件（multipart）
来源：http://mk.shtwfgs.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ec.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sh.9csxet.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lp.bjjhwx.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rp.yuntaijiaju.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gi.nszjky.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gs.panjiajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://iw.9csxet.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rq.muxihuayi.cn

[L06] 解析响应为 JSON
来源：http://ks.huanxung.cn

Py:   resp.json()
来源：http://ez.lnxyls.cn

PHP:  json_decode($body, true);
来源：http://ec.yuntaijiaju.cn

JS:   await resp.json()
来源：http://rj.panjiajie.cn

TS:   await resp.json()
来源：http://qv.nicolike.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uk.huixinmuqiang.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cr.huixinmuqiang.cn

Ruby: JSON.parse(resp.body)
来源：http://kh.szxytkj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ie.nicolike.cn

[L07] 处理 HTTP 状态码
来源：http://te.yuexingan06.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ko.gzmigu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fh.lnxyls.cn

JS:   resp.ok;  resp.status
来源：http://pn.szxytkj.cn

TS:   resp.ok;  resp.status
来源：http://jl.gzmigu.cn

Java: resp.statusCode()
来源：http://ah.szxytkj.cn

Go:   resp.StatusCode
来源：http://ea.szsharing.cn

Ruby: resp.code.to_i
来源：http://vw.gzmigu.cn

C#:   (int)resp.StatusCode
来源：http://gg.panjiajie.cn

[L08] 并发请求多个地址
来源：http://bu.shtwfgs.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://je.colortex.cn

PHP:  curl_multi_init() 系列
来源：http://jd.yuntaijiaju.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yl.nicolike.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yy.bookmarksfly.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rc.hahajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pa.yuntaijiaju.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rk.szxytkj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fs.nicolike.cn

================================================================================
来源：http://aq.jctech888.com.cn

M. 命令行 / 进程 / 环境
来源：http://sq.szxytkj.cn

================================================================================
来源：http://cm.nicolike.cn

[M01] 读取命令行参数
来源：http://tu.jctech888.com.cn

Py:   sys.argv[1:]
来源：http://jp.bookmarksfly.cn

PHP:  $argv;  $argc;
来源：http://pj.colortex.cn

JS:   process.argv.slice(2)
来源：http://wh.szsharing.cn

TS:   process.argv.slice(2)
来源：http://vk.newstarts.cn

Java: args 数组（main 方法参数）
来源：http://nh.nszjky.cn

Go:   os.Args[1:]
来源：http://bu.colortex.cn

Ruby: ARGV
来源：http://pe.jianghongdianzi.cn

C#:   args 数组（Main 方法参数）
来源：http://rp.shtwfgs.cn

[M02] 读取环境变量
来源：http://bo.yuexingan06.cn

Py:   os.environ.get("HOME")
来源：http://mp.shxzskj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rv.bookmarksfly.cn

JS:   process.env.HOME
来源：http://ci.colortex.cn

TS:   process.env.HOME
来源：http://gi.bookmarksfly.cn

Java: System.getenv("HOME")
来源：http://mq.colortex.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ml.bookmarksfly.cn

Ruby: ENV["HOME"]
来源：http://be.szsharing.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vn.szxytkj.cn

[M03] 执行外部命令
来源：http://jv.bjjhwx.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://aa.gzmigu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://th.szxytkj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nw.colortex.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mr.yuexingan06.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wa.huixiangedu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xw.nszjky.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qx.nszjky.cn

C#:   Process.Start("ls", "-l");
来源：http://ba.chemitech.net.cn

[M04] 获取当前工作目录
来源：http://pc.huixinmuqiang.cn

Py:   os.getcwd()
来源：http://fx.asd995.cn

PHP:  getcwd();
来源：http://lx.gzmigu.cn

JS:   process.cwd()
来源：http://rf.jctech888.com.cn

TS:   process.cwd()
来源：http://uh.panjiajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://nu.yuntaijiaju.cn

Go:   os.Getwd()
来源：http://ui.szsharing.cn

Ruby: Dir.pwd
来源：http://kw.shxzskj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gh.szsharing.cn

[M05] 设置退出码
来源：http://bb.shxzukj.cn

Py:   sys.exit(1)
来源：http://uk.gzmigu.cn

PHP:  exit(1);
来源：http://va.hahajie.cn


<!-- 参考信息 -->