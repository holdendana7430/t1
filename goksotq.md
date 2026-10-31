代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://le.wgjwhj.cn

[I07] 忽略大小写与多行模式
来源：http://hz.shtwfgs.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ti.huixiangedu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qt.yuntaijiaju.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xt.nszjky.cn

TS:   /error/gim
来源：http://jt.huixinmuqiang.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gq.chemitech.net.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sk.521024.cn

Ruby: s.scan(/error/i)
来源：http://qt.panjiajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jv.gzmigu.cn

[I08] 贪婪与非贪婪匹配
来源：http://gm.shxzukj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sa.hahajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wy.newstarts.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mc.gzmigu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dp.shxzskj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ui.huixinmuqiang.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pl.asd995.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://og.szxytkj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://oj.asd995.cn

================================================================================
来源：http://vc.shxzukj.cn

J. 日期与时间
来源：http://tg.lnxyls.cn

================================================================================
来源：http://ko.asd995.cn

[J01] 获取当前时间
来源：http://xb.gzmigu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://su.bjjhwx.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rq.szsharing.cn

JS:   new Date();  Date.now()
来源：http://wq.gzmigu.cn

TS:   new Date();  Date.now()
来源：http://qo.9csxet.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pg.wgjwhj.cn

Go:   time.Now()
来源：http://qv.521024.cn

Ruby: Time.now
来源：http://mm.bookmarksfly.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hv.jianghongdianzi.cn

[J02] 格式化输出
来源：http://et.chemitech.net.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://an.hahajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://df.bjjhwx.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jz.huixinmuqiang.cn

TS:   d.toISOString()
来源：http://bi.hahajie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hy.521024.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://uq.huixinmuqiang.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hu.9csxet.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://is.szsharing.cn

[J03] 字符串解析为日期
来源：http://gg.panjiajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ee.yuntaijiaju.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pl.521024.cn

JS:   new Date("2024-01-02")
来源：http://uw.nicolike.cn

TS:   new Date("2024-01-02")
来源：http://me.gzmigu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://eb.9csxet.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wx.shxzukj.cn

Ruby: Date.parse("2024-01-02")
来源：http://ey.hahajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vq.huixinmuqiang.cn

[J04] 时间戳与日期互转
来源：http://ua.haigaiapp.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uj.haigaiapp.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vq.colortex.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bw.jianghongdianzi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://el.bjjhwx.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yg.bjjhwx.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uj.shxzukj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ud.huixiangedu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vw.bjjhwx.cn

[J05] 时间加减（加 7 天）
来源：http://lq.9csxet.cn

Py:   now + timedelta(days=7)
来源：http://tr.shtwfgs.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zd.panjiajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wu.huixiangedu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qv.gzmigu.cn

Java: LocalDate.now().plusDays(7)
来源：http://ok.gzmigu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yx.muxihuayi.cn

Ruby: Time.now + 7 * 86400
来源：http://wg.shtwfgs.cn

C#:   DateTime.Now.AddDays(7)
来源：http://de.hahajie.cn

[J06] 计算两时间之差
来源：http://xm.szsharing.cn

Py:   (end - start).total_seconds()
来源：http://mo.nszjky.cn

PHP:  $end->diff($start)->days;
来源：http://bx.huixinmuqiang.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://aj.haigaiapp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://if.jianghongdianzi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zk.haigaiapp.cn

Go:   end.Sub(start).Hours()
来源：http://wh.bookmarksfly.cn

Ruby: end - start                 # 返回秒数
来源：http://jb.nszjky.cn

C#:   (end - start).TotalSeconds
来源：http://ye.wgjwhj.cn

[J07] 比较两个日期
来源：http://vq.hnjuh.cn

Py:   d1 < d2;  d1 == d2
来源：http://ou.9csxet.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kz.szxytkj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hr.hahajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://uv.panjiajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pq.jctech888.com.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://oq.shxzskj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://if.newstarts.cn

C#:   d1 < d2;  d1 == d2
来源：http://vd.shtwfgs.cn

[J08] 提取年月日与星期
来源：http://hz.asd995.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ry.shxzukj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mc.panjiajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mh.nszjky.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xa.hahajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ig.nicolike.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fs.newstarts.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://eu.521024.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bn.nszjky.cn

[J09] 时区处理
来源：http://di.haigaiapp.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nk.huixinmuqiang.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ya.haigaiapp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jn.nicolike.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://na.haigaiapp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ys.bookmarksfly.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rg.521024.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://sv.shxzskj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ml.newstarts.cn

[J10] 取今天 / 本月第一天
来源：http://sh.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zc.hahajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yh.gzmigu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ug.521024.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://if.huixiangedu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://na.yuexingan06.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ul.nszjky.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jp.yuntaijiaju.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oh.shtwfgs.cn

================================================================================
来源：http://sb.yuexingan06.cn

K. JSON 与序列化
来源：http://ik.9csxet.cn

================================================================================
来源：http://bu.shxzskj.cn

[K01] 对象转 JSON 字符串
来源：http://nc.gzmigu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ns.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mw.9csxet.cn

JS:   JSON.stringify(obj)
来源：http://jj.szsharing.cn

TS:   JSON.stringify(obj)
来源：http://xa.wgjwhj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qz.bookmarksfly.cn

Go:   json.Marshal(obj)
来源：http://hj.haigaiapp.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ht.shxzskj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jj.yuntaijiaju.cn

[K02] JSON 字符串转对象
来源：http://gk.huanxung.cn

Py:   json.loads(s)
来源：http://yt.huanxung.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nn.jctech888.com.cn

JS:   JSON.parse(s)
来源：http://ar.jianghongdianzi.cn

TS:   JSON.parse(s)
来源：http://iy.521024.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mu.huanxung.cn

Go:   json.Unmarshal(data, &v)
来源：http://xv.colortex.cn

Ruby: JSON.parse(s)
来源：http://yl.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://oo.chemitech.net.cn

[K03] JSON 美化输出（带缩进）
来源：http://xw.newstarts.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qg.chemitech.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ba.bookmarksfly.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vd.huanxung.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bq.nszjky.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rb.asd995.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sr.shtwfgs.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ke.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ja.nszjky.cn

[K04] 读取 JSON 文件
来源：http://il.szxytkj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mi.asd995.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gf.nicolike.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ms.shxzukj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bh.chemitech.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nc.colortex.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sd.nszjky.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rd.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rg.shtwfgs.cn

[K05] 深拷贝对象
来源：http://yw.bjjhwx.cn

Py:   copy.deepcopy(obj)
来源：http://jq.shtwfgs.cn

PHP:  unserialize(serialize($obj));
来源：http://rf.muxihuayi.cn

JS:   structuredClone(obj)
来源：http://ol.colortex.cn

TS:   structuredClone(obj)
来源：http://ew.colortex.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wa.wgjwhj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hh.nicolike.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gr.newstarts.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zk.szsharing.cn

[K06] 解析 URL 查询串
来源：http://qr.newstarts.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ra.szsharing.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ad.muxihuayi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fl.colortex.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rq.szsharing.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yx.shxzukj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qx.hnjuh.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vt.asd995.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jf.9csxet.cn

[K07] 进制转换
来源：http://pu.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fa.newstarts.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kt.muxihuayi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zr.hnjuh.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qh.newstarts.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://np.haigaiapp.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lg.asd995.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bc.nicolike.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://co.nszjky.cn

[K08] 二进制序列化（非 JSON）
来源：http://cd.yuntaijiaju.cn

Py:   pickle.dumps(obj)
来源：http://ys.szsharing.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ut.hnjuh.cn

JS:   v8.serialize(obj)        // Node
来源：http://jb.shxzskj.cn

TS:   v8.serialize(obj)        // Node
来源：http://tn.shxzukj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://er.szxytkj.cn

Go:   encoding/gob
来源：http://cc.shxzukj.cn

Ruby: Marshal.dump(obj)
来源：http://jg.asd995.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://th.521024.cn

================================================================================
来源：http://ps.gzmigu.cn

L. 网络请求
来源：http://nq.asd995.cn

================================================================================
来源：http://ht.huixiangedu.cn

[L01] 发送 GET 请求
来源：http://wc.panjiajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mr.asd995.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://go.szxytkj.cn

JS:   await fetch(url)
来源：http://we.chemitech.net.cn

TS:   await fetch(url)
来源：http://wv.huixinmuqiang.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ac.nicolike.cn

Go:   resp, err := http.Get(url)
来源：http://jj.shxzskj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://sk.bookmarksfly.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ih.huixiangedu.cn

[L02] 发送 POST JSON
来源：http://ra.muxihuayi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hn.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ru.newstarts.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bk.szsharing.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zr.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sw.gzmigu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://es.bjjhwx.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ck.shxzukj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://se.shtwfgs.cn

[L03] 设置自定义请求头
来源：http://fc.jctech888.com.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://or.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lj.yuexingan06.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bl.bookmarksfly.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uf.colortex.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yq.nicolike.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://iy.newstarts.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bm.hahajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gp.szxytkj.cn

[L04] 设置超时
来源：http://hl.gzmigu.cn

Py:   requests.get(url, timeout=5)
来源：http://xv.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ii.huixiangedu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kn.huixiangedu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sz.shxzskj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fp.huanxung.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bo.9csxet.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ns.lnxyls.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gn.szsharing.cn

[L05] 上传文件（multipart）
来源：http://ao.huanxung.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uc.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nb.lnxyls.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kl.bookmarksfly.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tg.shxzukj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pq.panjiajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qo.szsharing.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tw.huixiangedu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uf.huixiangedu.cn

[L06] 解析响应为 JSON
来源：http://ds.nszjky.cn

Py:   resp.json()
来源：http://xd.wgjwhj.cn

PHP:  json_decode($body, true);
来源：http://yx.hahajie.cn

JS:   await resp.json()
来源：http://cg.gzmigu.cn

TS:   await resp.json()
来源：http://ln.colortex.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qd.yuexingan06.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wm.huanxung.cn

Ruby: JSON.parse(resp.body)
来源：http://zy.shtwfgs.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gr.asd995.cn

[L07] 处理 HTTP 状态码
来源：http://vl.szsharing.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xf.nszjky.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ir.huixiangedu.cn

JS:   resp.ok;  resp.status
来源：http://jw.newstarts.cn

TS:   resp.ok;  resp.status
来源：http://gl.chemitech.net.cn

Java: resp.statusCode()
来源：http://xp.chemitech.net.cn

Go:   resp.StatusCode
来源：http://di.huanxung.cn

Ruby: resp.code.to_i
来源：http://qk.huanxung.cn

C#:   (int)resp.StatusCode
来源：http://rw.gzmigu.cn

[L08] 并发请求多个地址
来源：http://bg.haigaiapp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://te.shxzskj.cn

PHP:  curl_multi_init() 系列
来源：http://jk.521024.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oq.wgjwhj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lh.shxzukj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cl.huanxung.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kv.hnjuh.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cx.9csxet.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qj.asd995.cn

================================================================================
来源：http://cf.nszjky.cn

M. 命令行 / 进程 / 环境
来源：http://be.shxzskj.cn

================================================================================
来源：http://ql.newstarts.cn

[M01] 读取命令行参数
来源：http://pd.wgjwhj.cn

Py:   sys.argv[1:]
来源：http://sf.szxytkj.cn

PHP:  $argv;  $argc;
来源：http://ur.bookmarksfly.cn

JS:   process.argv.slice(2)
来源：http://ff.hahajie.cn

TS:   process.argv.slice(2)
来源：http://ww.shxzukj.cn

Java: args 数组（main 方法参数）
来源：http://vt.jctech888.com.cn

Go:   os.Args[1:]
来源：http://bp.huixinmuqiang.cn

Ruby: ARGV
来源：http://mv.bjjhwx.cn

C#:   args 数组（Main 方法参数）
来源：http://om.521024.cn

[M02] 读取环境变量
来源：http://fj.bookmarksfly.cn

Py:   os.environ.get("HOME")
来源：http://hd.szsharing.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ks.jianghongdianzi.cn

JS:   process.env.HOME
来源：http://du.shtwfgs.cn

TS:   process.env.HOME
来源：http://ru.huixinmuqiang.cn

Java: System.getenv("HOME")
来源：http://hy.hahajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mk.yuexingan06.cn

Ruby: ENV["HOME"]
来源：http://mh.nicolike.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ee.szsharing.cn

[M03] 执行外部命令
来源：http://ia.nszjky.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qd.szsharing.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://la.hahajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ma.hnjuh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gw.colortex.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lq.huixinmuqiang.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://aj.nszjky.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zf.shtwfgs.cn

C#:   Process.Start("ls", "-l");
来源：http://oz.9csxet.cn

[M04] 获取当前工作目录
来源：http://xl.521024.cn

Py:   os.getcwd()
来源：http://ml.hnjuh.cn

PHP:  getcwd();
来源：http://iq.9csxet.cn

JS:   process.cwd()
来源：http://xd.hnjuh.cn

TS:   process.cwd()
来源：http://xr.jctech888.com.cn

Java: Path.of("").toAbsolutePath()
来源：http://mk.huixinmuqiang.cn

Go:   os.Getwd()
来源：http://uu.bjjhwx.cn

Ruby: Dir.pwd
来源：http://ki.huixinmuqiang.cn


<!-- 参考信息 -->