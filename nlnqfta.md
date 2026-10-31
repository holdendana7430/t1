代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lu.haigaiapp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xz.huixiangedu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ae.panjiajie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oh.chemitech.net.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qn.wgjwhj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://in.newstarts.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://or.nszjky.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kc.asd995.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vo.panjiajie.cn

[I07] 忽略大小写与多行模式
来源：http://wl.yuexingan06.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hq.lnxyls.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ox.colortex.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sg.chemitech.net.cn

TS:   /error/gim
来源：http://gh.9csxet.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ht.muxihuayi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lz.hahajie.cn

Ruby: s.scan(/error/i)
来源：http://lp.shxzukj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ac.bjjhwx.cn

[I08] 贪婪与非贪婪匹配
来源：http://ts.wgjwhj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ek.lnxyls.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dm.hahajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jh.haigaiapp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uq.nicolike.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://up.asd995.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ip.nicolike.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ng.shtwfgs.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ip.huixiangedu.cn

================================================================================
来源：http://ye.lnxyls.cn

J. 日期与时间
来源：http://cd.521024.cn

================================================================================
来源：http://fo.asd995.cn

[J01] 获取当前时间
来源：http://vh.asd995.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qd.szsharing.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bg.nicolike.cn

JS:   new Date();  Date.now()
来源：http://jt.hnjuh.cn

TS:   new Date();  Date.now()
来源：http://qy.panjiajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://na.jctech888.com.cn

Go:   time.Now()
来源：http://hu.bookmarksfly.cn

Ruby: Time.now
来源：http://dp.huixinmuqiang.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vp.shxzukj.cn

[J02] 格式化输出
来源：http://zy.wgjwhj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ch.szxytkj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tz.shxzukj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yc.panjiajie.cn

TS:   d.toISOString()
来源：http://cn.gzmigu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ie.jctech888.com.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hj.wgjwhj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qh.9csxet.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hu.huixinmuqiang.cn

[J03] 字符串解析为日期
来源：http://bx.szsharing.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kd.asd995.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ny.asd995.cn

JS:   new Date("2024-01-02")
来源：http://uo.lnxyls.cn

TS:   new Date("2024-01-02")
来源：http://ti.shxzukj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dc.jctech888.com.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wc.huixinmuqiang.cn

Ruby: Date.parse("2024-01-02")
来源：http://cp.szsharing.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lc.huixinmuqiang.cn

[J04] 时间戳与日期互转
来源：http://sx.huixinmuqiang.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yu.panjiajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ic.huanxung.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sd.9csxet.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cn.gzmigu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ym.nszjky.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uj.yuntaijiaju.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cl.hnjuh.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mp.nicolike.cn

[J05] 时间加减（加 7 天）
来源：http://mx.yuntaijiaju.cn

Py:   now + timedelta(days=7)
来源：http://ko.hnjuh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://cu.hahajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xo.szsharing.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qd.asd995.cn

Java: LocalDate.now().plusDays(7)
来源：http://yy.shxzukj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fk.shxzukj.cn

Ruby: Time.now + 7 * 86400
来源：http://dd.9csxet.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rj.yuexingan06.cn

[J06] 计算两时间之差
来源：http://oo.hnjuh.cn

Py:   (end - start).total_seconds()
来源：http://mg.bookmarksfly.cn

PHP:  $end->diff($start)->days;
来源：http://vo.bookmarksfly.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bx.hahajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yo.colortex.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vu.newstarts.cn

Go:   end.Sub(start).Hours()
来源：http://um.shxzskj.cn

Ruby: end - start                 # 返回秒数
来源：http://xk.nicolike.cn

C#:   (end - start).TotalSeconds
来源：http://nt.bookmarksfly.cn

[J07] 比较两个日期
来源：http://gf.newstarts.cn

Py:   d1 < d2;  d1 == d2
来源：http://qe.wgjwhj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dx.nszjky.cn

JS:   d1.getTime() < d2.getTime()
来源：http://uk.nszjky.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zm.lnxyls.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fn.lnxyls.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://us.hahajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://nf.hahajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://nz.bjjhwx.cn

[J08] 提取年月日与星期
来源：http://fr.huixinmuqiang.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://at.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jd.colortex.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://of.jctech888.com.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qo.chemitech.net.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mw.bjjhwx.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rd.521024.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rx.gzmigu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tx.newstarts.cn

[J09] 时区处理
来源：http://ch.colortex.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fx.szxytkj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dq.chemitech.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jt.nszjky.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jp.hahajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wh.szsharing.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jb.yuexingan06.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://oj.huixinmuqiang.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ai.shxzskj.cn

[J10] 取今天 / 本月第一天
来源：http://uu.gzmigu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ut.hahajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bn.haigaiapp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ep.szsharing.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lw.gzmigu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wh.9csxet.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lv.gzmigu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lq.colortex.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gb.hahajie.cn

================================================================================
来源：http://tr.chemitech.net.cn

K. JSON 与序列化
来源：http://jd.nicolike.cn

================================================================================
来源：http://ss.asd995.cn

[K01] 对象转 JSON 字符串
来源：http://kg.huixiangedu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tn.huanxung.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://sb.huixiangedu.cn

JS:   JSON.stringify(obj)
来源：http://xc.shxzskj.cn

TS:   JSON.stringify(obj)
来源：http://nf.lnxyls.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sp.shxzukj.cn

Go:   json.Marshal(obj)
来源：http://vw.yuntaijiaju.cn

Ruby: obj.to_json                                     // require "json"
来源：http://sj.szxytkj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ov.shxzskj.cn

[K02] JSON 字符串转对象
来源：http://kq.jianghongdianzi.cn

Py:   json.loads(s)
来源：http://lh.szsharing.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gg.shxzskj.cn

JS:   JSON.parse(s)
来源：http://xu.huixinmuqiang.cn

TS:   JSON.parse(s)
来源：http://dp.nszjky.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://za.jianghongdianzi.cn

Go:   json.Unmarshal(data, &v)
来源：http://om.jianghongdianzi.cn

Ruby: JSON.parse(s)
来源：http://jw.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kb.bjjhwx.cn

[K03] JSON 美化输出（带缩进）
来源：http://ej.shtwfgs.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uu.newstarts.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ek.bookmarksfly.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bu.szsharing.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ks.huixinmuqiang.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ob.szsharing.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ip.gzmigu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ba.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nw.huixiangedu.cn

[K04] 读取 JSON 文件
来源：http://qe.9csxet.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kv.jianghongdianzi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ym.newstarts.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ry.521024.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dc.haigaiapp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ph.szxytkj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lh.yuntaijiaju.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://sf.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ku.shxzukj.cn

[K05] 深拷贝对象
来源：http://zp.haigaiapp.cn

Py:   copy.deepcopy(obj)
来源：http://fz.newstarts.cn

PHP:  unserialize(serialize($obj));
来源：http://qt.jctech888.com.cn

JS:   structuredClone(obj)
来源：http://ci.shxzukj.cn

TS:   structuredClone(obj)
来源：http://aq.yuntaijiaju.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://go.hahajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://at.panjiajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xn.521024.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wq.hnjuh.cn

[K06] 解析 URL 查询串
来源：http://ko.asd995.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mj.huixiangedu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qd.shxzukj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jt.hahajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pk.panjiajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://et.gzmigu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dm.nicolike.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://no.huixiangedu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ga.gzmigu.cn

[K07] 进制转换
来源：http://zj.chemitech.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mm.shxzskj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sm.hahajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wj.huixinmuqiang.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mo.panjiajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tc.muxihuayi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pb.shxzskj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://af.szxytkj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bn.haigaiapp.cn

[K08] 二进制序列化（非 JSON）
来源：http://hn.bookmarksfly.cn

Py:   pickle.dumps(obj)
来源：http://wa.bjjhwx.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lm.muxihuayi.cn

JS:   v8.serialize(obj)        // Node
来源：http://kc.haigaiapp.cn

TS:   v8.serialize(obj)        // Node
来源：http://fx.521024.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wi.shtwfgs.cn

Go:   encoding/gob
来源：http://xe.nicolike.cn

Ruby: Marshal.dump(obj)
来源：http://bs.lnxyls.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ch.nszjky.cn

================================================================================
来源：http://wa.shtwfgs.cn

L. 网络请求
来源：http://ss.yuexingan06.cn

================================================================================
来源：http://wg.jctech888.com.cn

[L01] 发送 GET 请求
来源：http://qx.gzmigu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ee.huanxung.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://eu.muxihuayi.cn

JS:   await fetch(url)
来源：http://we.szsharing.cn

TS:   await fetch(url)
来源：http://lz.hahajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lv.huanxung.cn

Go:   resp, err := http.Get(url)
来源：http://ge.wgjwhj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://te.hahajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ib.colortex.cn

[L02] 发送 POST JSON
来源：http://wq.yuntaijiaju.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ur.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dt.bjjhwx.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lo.hahajie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rs.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ou.jianghongdianzi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qn.szsharing.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ka.hahajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wb.muxihuayi.cn

[L03] 设置自定义请求头
来源：http://fa.panjiajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mu.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fo.bjjhwx.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mg.szsharing.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bu.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ff.muxihuayi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://et.colortex.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zj.szxytkj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fk.yuntaijiaju.cn

[L04] 设置超时
来源：http://aw.szsharing.cn

Py:   requests.get(url, timeout=5)
来源：http://wh.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ay.hnjuh.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zx.asd995.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://we.asd995.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sy.shxzskj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://si.colortex.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ic.shxzskj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ay.huixiangedu.cn

[L05] 上传文件（multipart）
来源：http://am.9csxet.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cy.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yh.bookmarksfly.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ro.colortex.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mu.szxytkj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://po.shxzukj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pi.hnjuh.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ig.huixiangedu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rc.muxihuayi.cn

[L06] 解析响应为 JSON
来源：http://ws.bjjhwx.cn

Py:   resp.json()
来源：http://dd.haigaiapp.cn

PHP:  json_decode($body, true);
来源：http://xp.shxzukj.cn

JS:   await resp.json()
来源：http://ur.shxzukj.cn

TS:   await resp.json()
来源：http://vi.521024.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mo.panjiajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://si.shxzskj.cn

Ruby: JSON.parse(resp.body)
来源：http://kp.lnxyls.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://er.nszjky.cn

[L07] 处理 HTTP 状态码
来源：http://hw.jianghongdianzi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ao.yuntaijiaju.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cb.szsharing.cn

JS:   resp.ok;  resp.status
来源：http://fd.bjjhwx.cn

TS:   resp.ok;  resp.status
来源：http://je.szsharing.cn

Java: resp.statusCode()
来源：http://np.gzmigu.cn

Go:   resp.StatusCode
来源：http://rm.hahajie.cn

Ruby: resp.code.to_i
来源：http://qq.haigaiapp.cn

C#:   (int)resp.StatusCode
来源：http://dw.yuntaijiaju.cn

[L08] 并发请求多个地址
来源：http://ar.newstarts.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tg.yuntaijiaju.cn

PHP:  curl_multi_init() 系列
来源：http://so.shtwfgs.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wj.newstarts.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pk.panjiajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sy.panjiajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://js.nszjky.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ye.muxihuayi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zz.haigaiapp.cn

================================================================================
来源：http://as.shxzukj.cn

M. 命令行 / 进程 / 环境
来源：http://nd.wgjwhj.cn

================================================================================
来源：http://ie.jctech888.com.cn

[M01] 读取命令行参数
来源：http://tg.hnjuh.cn

Py:   sys.argv[1:]
来源：http://gy.gzmigu.cn

PHP:  $argv;  $argc;
来源：http://bh.bjjhwx.cn

JS:   process.argv.slice(2)
来源：http://er.muxihuayi.cn

TS:   process.argv.slice(2)
来源：http://xd.nszjky.cn

Java: args 数组（main 方法参数）
来源：http://zb.shtwfgs.cn

Go:   os.Args[1:]
来源：http://gs.muxihuayi.cn

Ruby: ARGV
来源：http://nk.huixiangedu.cn

C#:   args 数组（Main 方法参数）
来源：http://hc.shxzukj.cn

[M02] 读取环境变量
来源：http://py.chemitech.net.cn

Py:   os.environ.get("HOME")
来源：http://cr.chemitech.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ez.bookmarksfly.cn

JS:   process.env.HOME
来源：http://xf.gzmigu.cn

TS:   process.env.HOME
来源：http://hv.newstarts.cn

Java: System.getenv("HOME")
来源：http://vc.colortex.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bh.szxytkj.cn

Ruby: ENV["HOME"]
来源：http://mx.521024.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tx.yuexingan06.cn

[M03] 执行外部命令
来源：http://nt.shxzukj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dj.shxzskj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://by.huixiangedu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gr.nszjky.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vr.gzmigu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cj.jctech888.com.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zl.muxihuayi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pf.szsharing.cn

C#:   Process.Start("ls", "-l");
来源：http://cu.yuntaijiaju.cn


<!-- 参考信息 -->