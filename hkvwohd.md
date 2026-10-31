代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uh.jianghongdianzi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kl.panjiajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nt.lnxyls.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://is.yuexingan06.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ag.nszjky.cn

[I07] 忽略大小写与多行模式
来源：http://yp.panjiajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bq.huanxung.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://an.bookmarksfly.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jp.asd995.cn

TS:   /error/gim
来源：http://zx.yuntaijiaju.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uv.yuntaijiaju.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qd.nszjky.cn

Ruby: s.scan(/error/i)
来源：http://ca.521024.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vz.huanxung.cn

[I08] 贪婪与非贪婪匹配
来源：http://ln.wgjwhj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zk.nszjky.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qo.yuexingan06.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dt.asd995.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kg.haigaiapp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://yy.lnxyls.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gx.huixiangedu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cd.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://te.gzmigu.cn

================================================================================
来源：http://wm.shxzskj.cn

J. 日期与时间
来源：http://ze.haigaiapp.cn

================================================================================
来源：http://qw.jianghongdianzi.cn

[J01] 获取当前时间
来源：http://nr.9csxet.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://gw.shxzukj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.shtwfgs.cn

JS:   new Date();  Date.now()
来源：http://on.bookmarksfly.cn

TS:   new Date();  Date.now()
来源：http://wb.hnjuh.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tg.shtwfgs.cn

Go:   time.Now()
来源：http://am.panjiajie.cn

Ruby: Time.now
来源：http://jz.jianghongdianzi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tg.hahajie.cn

[J02] 格式化输出
来源：http://gj.jctech888.com.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ne.szxytkj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ag.asd995.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wd.shxzskj.cn

TS:   d.toISOString()
来源：http://ws.bookmarksfly.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mb.hnjuh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cu.wgjwhj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nt.nszjky.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ty.9csxet.cn

[J03] 字符串解析为日期
来源：http://ju.9csxet.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://er.bookmarksfly.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kq.shxzukj.cn

JS:   new Date("2024-01-02")
来源：http://fk.hnjuh.cn

TS:   new Date("2024-01-02")
来源：http://yt.szxytkj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://nj.colortex.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mn.shtwfgs.cn

Ruby: Date.parse("2024-01-02")
来源：http://zc.jctech888.com.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://oe.bookmarksfly.cn

[J04] 时间戳与日期互转
来源：http://ok.jianghongdianzi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.asd995.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tb.jianghongdianzi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rf.shtwfgs.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wm.colortex.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ff.jctech888.com.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://br.shtwfgs.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nj.colortex.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nj.bookmarksfly.cn

[J05] 时间加减（加 7 天）
来源：http://kf.bjjhwx.cn

Py:   now + timedelta(days=7)
来源：http://pl.panjiajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nt.hahajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yy.lnxyls.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://en.colortex.cn

Java: LocalDate.now().plusDays(7)
来源：http://qi.chemitech.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sn.asd995.cn

Ruby: Time.now + 7 * 86400
来源：http://qa.521024.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jy.yuntaijiaju.cn

[J06] 计算两时间之差
来源：http://ep.nicolike.cn

Py:   (end - start).total_seconds()
来源：http://en.shxzskj.cn

PHP:  $end->diff($start)->days;
来源：http://wp.yuexingan06.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://no.wgjwhj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qz.szsharing.cn

Java: Duration.between(start, end).toSeconds()
来源：http://cl.hnjuh.cn

Go:   end.Sub(start).Hours()
来源：http://kq.szsharing.cn

Ruby: end - start                 # 返回秒数
来源：http://xx.szxytkj.cn

C#:   (end - start).TotalSeconds
来源：http://wg.bjjhwx.cn

[J07] 比较两个日期
来源：http://qr.gzmigu.cn

Py:   d1 < d2;  d1 == d2
来源：http://ae.9csxet.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xk.yuexingan06.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bl.muxihuayi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ai.nicolike.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xj.lnxyls.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xb.muxihuayi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://sf.shxzukj.cn

C#:   d1 < d2;  d1 == d2
来源：http://cw.521024.cn

[J08] 提取年月日与星期
来源：http://yv.gzmigu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kl.haigaiapp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vz.gzmigu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bf.colortex.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hf.hnjuh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://va.szsharing.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://le.muxihuayi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ip.huixiangedu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lg.huixiangedu.cn

[J09] 时区处理
来源：http://ur.szxytkj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rx.yuexingan06.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://io.yuntaijiaju.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fj.huixiangedu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nc.chemitech.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://je.9csxet.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rr.yuexingan06.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gq.bjjhwx.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cd.newstarts.cn

[J10] 取今天 / 本月第一天
来源：http://ys.bjjhwx.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://qm.muxihuayi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fx.chemitech.net.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sl.muxihuayi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jw.hnjuh.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yx.521024.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qa.panjiajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sp.huanxung.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ck.muxihuayi.cn

================================================================================
来源：http://xx.lnxyls.cn

K. JSON 与序列化
来源：http://nj.lnxyls.cn

================================================================================
来源：http://kt.shtwfgs.cn

[K01] 对象转 JSON 字符串
来源：http://mp.huanxung.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wx.521024.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tw.huixiangedu.cn

JS:   JSON.stringify(obj)
来源：http://kc.huanxung.cn

TS:   JSON.stringify(obj)
来源：http://aw.bookmarksfly.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bj.colortex.cn

Go:   json.Marshal(obj)
来源：http://ai.nszjky.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ou.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://tl.shtwfgs.cn

[K02] JSON 字符串转对象
来源：http://ms.gzmigu.cn

Py:   json.loads(s)
来源：http://lq.lnxyls.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ej.lnxyls.cn

JS:   JSON.parse(s)
来源：http://yf.bookmarksfly.cn

TS:   JSON.parse(s)
来源：http://kq.9csxet.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jc.jctech888.com.cn

Go:   json.Unmarshal(data, &v)
来源：http://oz.huixiangedu.cn

Ruby: JSON.parse(s)
来源：http://pi.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gm.huixinmuqiang.cn

[K03] JSON 美化输出（带缩进）
来源：http://vz.shtwfgs.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uq.haigaiapp.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wh.wgjwhj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ly.asd995.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xa.shxzukj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hr.hnjuh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jg.yuexingan06.cn

Ruby: JSON.pretty_generate(obj)
来源：http://di.hnjuh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yu.chemitech.net.cn

[K04] 读取 JSON 文件
来源：http://br.521024.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jz.szsharing.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ma.lnxyls.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qj.nszjky.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vv.bookmarksfly.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uh.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ze.newstarts.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jr.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wk.huixinmuqiang.cn

[K05] 深拷贝对象
来源：http://cn.hnjuh.cn

Py:   copy.deepcopy(obj)
来源：http://fy.yuexingan06.cn

PHP:  unserialize(serialize($obj));
来源：http://ww.huixinmuqiang.cn

JS:   structuredClone(obj)
来源：http://gj.jianghongdianzi.cn

TS:   structuredClone(obj)
来源：http://gl.9csxet.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fk.yuexingan06.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://of.haigaiapp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://br.bookmarksfly.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lx.9csxet.cn

[K06] 解析 URL 查询串
来源：http://ik.asd995.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ph.hnjuh.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tz.asd995.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sp.chemitech.net.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rv.shxzskj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://co.newstarts.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ny.jianghongdianzi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xj.muxihuayi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://im.muxihuayi.cn

[K07] 进制转换
来源：http://pz.yuntaijiaju.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rl.asd995.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qi.lnxyls.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yi.huixiangedu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pw.huanxung.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gr.shtwfgs.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://my.bjjhwx.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://iq.newstarts.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cu.nszjky.cn

[K08] 二进制序列化（非 JSON）
来源：http://qe.lnxyls.cn

Py:   pickle.dumps(obj)
来源：http://xw.huixiangedu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://eb.huanxung.cn

JS:   v8.serialize(obj)        // Node
来源：http://uq.jctech888.com.cn

TS:   v8.serialize(obj)        // Node
来源：http://uj.shxzukj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qb.newstarts.cn

Go:   encoding/gob
来源：http://as.szsharing.cn

Ruby: Marshal.dump(obj)
来源：http://ge.521024.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ml.shxzukj.cn

================================================================================
来源：http://nl.9csxet.cn

L. 网络请求
来源：http://gy.bjjhwx.cn

================================================================================
来源：http://tn.chemitech.net.cn

[L01] 发送 GET 请求
来源：http://oz.haigaiapp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://me.chemitech.net.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vx.haigaiapp.cn

JS:   await fetch(url)
来源：http://yt.shxzukj.cn

TS:   await fetch(url)
来源：http://bj.521024.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hi.hahajie.cn

Go:   resp, err := http.Get(url)
来源：http://lh.gzmigu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://oi.bookmarksfly.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zu.shtwfgs.cn

[L02] 发送 POST JSON
来源：http://lq.huixinmuqiang.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bk.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://io.nicolike.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fh.muxihuayi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ei.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zp.bookmarksfly.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pa.szxytkj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yl.chemitech.net.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ka.muxihuayi.cn

[L03] 设置自定义请求头
来源：http://ft.colortex.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fv.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kh.nicolike.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xv.9csxet.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gg.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jp.asd995.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nw.huanxung.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pc.wgjwhj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://il.szsharing.cn

[L04] 设置超时
来源：http://we.wgjwhj.cn

Py:   requests.get(url, timeout=5)
来源：http://rh.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xx.shxzukj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dm.9csxet.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qt.shxzskj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dk.huanxung.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://oc.yuexingan06.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hr.yuexingan06.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pq.hahajie.cn

[L05] 上传文件（multipart）
来源：http://xe.gzmigu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cc.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ax.szsharing.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dn.huanxung.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ct.jctech888.com.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://io.jianghongdianzi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fk.muxihuayi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sh.hnjuh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hk.huixiangedu.cn

[L06] 解析响应为 JSON
来源：http://kz.szsharing.cn

Py:   resp.json()
来源：http://uk.szxytkj.cn

PHP:  json_decode($body, true);
来源：http://oz.wgjwhj.cn

JS:   await resp.json()
来源：http://yy.haigaiapp.cn

TS:   await resp.json()
来源：http://uw.huixiangedu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://of.lnxyls.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zh.bjjhwx.cn

Ruby: JSON.parse(resp.body)
来源：http://kh.gzmigu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yr.asd995.cn

[L07] 处理 HTTP 状态码
来源：http://pt.jianghongdianzi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ri.shxzukj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dn.huixiangedu.cn

JS:   resp.ok;  resp.status
来源：http://xh.szsharing.cn

TS:   resp.ok;  resp.status
来源：http://ow.wgjwhj.cn

Java: resp.statusCode()
来源：http://la.newstarts.cn

Go:   resp.StatusCode
来源：http://kz.shxzskj.cn

Ruby: resp.code.to_i
来源：http://fy.hnjuh.cn

C#:   (int)resp.StatusCode
来源：http://ao.yuntaijiaju.cn

[L08] 并发请求多个地址
来源：http://ye.chemitech.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hq.asd995.cn

PHP:  curl_multi_init() 系列
来源：http://nh.lnxyls.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ik.hahajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jy.nicolike.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://is.panjiajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://me.shtwfgs.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fa.huixinmuqiang.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lm.newstarts.cn

================================================================================
来源：http://zx.hnjuh.cn

M. 命令行 / 进程 / 环境
来源：http://te.9csxet.cn

================================================================================
来源：http://ps.huixiangedu.cn

[M01] 读取命令行参数
来源：http://el.nszjky.cn

Py:   sys.argv[1:]
来源：http://kn.huanxung.cn

PHP:  $argv;  $argc;
来源：http://dl.jianghongdianzi.cn

JS:   process.argv.slice(2)
来源：http://bh.yuexingan06.cn

TS:   process.argv.slice(2)
来源：http://rk.yuexingan06.cn

Java: args 数组（main 方法参数）
来源：http://qa.jctech888.com.cn

Go:   os.Args[1:]
来源：http://xw.nicolike.cn

Ruby: ARGV
来源：http://vt.chemitech.net.cn

C#:   args 数组（Main 方法参数）
来源：http://cm.nszjky.cn

[M02] 读取环境变量
来源：http://kx.wgjwhj.cn

Py:   os.environ.get("HOME")
来源：http://av.wgjwhj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yx.panjiajie.cn

JS:   process.env.HOME
来源：http://db.huixiangedu.cn

TS:   process.env.HOME
来源：http://ff.shxzskj.cn

Java: System.getenv("HOME")
来源：http://io.panjiajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sq.colortex.cn

Ruby: ENV["HOME"]
来源：http://my.yuntaijiaju.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tg.wgjwhj.cn

[M03] 执行外部命令
来源：http://jo.yuntaijiaju.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dh.asd995.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lj.hnjuh.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hl.muxihuayi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wm.jctech888.com.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qm.szxytkj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://iw.bookmarksfly.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zw.szsharing.cn

C#:   Process.Start("ls", "-l");
来源：http://vz.newstarts.cn

[M04] 获取当前工作目录
来源：http://dv.hahajie.cn

Py:   os.getcwd()
来源：http://dj.yuexingan06.cn

PHP:  getcwd();
来源：http://lq.521024.cn

JS:   process.cwd()
来源：http://zo.jianghongdianzi.cn


<!-- 参考信息 -->