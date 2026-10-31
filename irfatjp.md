代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://tt.9csxet.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hj.bjjhwx.cn

JS:   s.split(/\s*,\s*/)
来源：http://qg.521024.cn

TS:   s.split(/\s*,\s*/)
来源：http://ki.colortex.cn

Java: s.split("\\s*,\\s*")
来源：http://ky.jctech888.com.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qi.gzmigu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://cx.shxzukj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://aj.bookmarksfly.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://se.gzmigu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yc.gzmigu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://iv.jctech888.com.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pl.panjiajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nj.chemitech.net.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://km.lnxyls.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zf.asd995.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jt.521024.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gw.521024.cn

[I07] 忽略大小写与多行模式
来源：http://hv.shxzskj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jl.yuntaijiaju.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ww.szsharing.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vx.yuntaijiaju.cn

TS:   /error/gim
来源：http://cm.huixiangedu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zv.shxzskj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fc.yuntaijiaju.cn

Ruby: s.scan(/error/i)
来源：http://vn.nicolike.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pk.yuexingan06.cn

[I08] 贪婪与非贪婪匹配
来源：http://tv.haigaiapp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pg.nszjky.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ke.gzmigu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://si.jctech888.com.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://eo.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xl.chemitech.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pi.yuntaijiaju.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ql.newstarts.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fo.jctech888.com.cn

================================================================================
来源：http://rx.panjiajie.cn

J. 日期与时间
来源：http://ba.9csxet.cn

================================================================================
来源：http://fm.jctech888.com.cn

[J01] 获取当前时间
来源：http://lb.asd995.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qt.nicolike.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wl.szxytkj.cn

JS:   new Date();  Date.now()
来源：http://kt.jctech888.com.cn

TS:   new Date();  Date.now()
来源：http://no.9csxet.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://us.huixiangedu.cn

Go:   time.Now()
来源：http://qg.shtwfgs.cn

Ruby: Time.now
来源：http://ty.szsharing.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hs.huanxung.cn

[J02] 格式化输出
来源：http://nb.9csxet.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ej.chemitech.net.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kn.yuntaijiaju.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pj.szsharing.cn

TS:   d.toISOString()
来源：http://si.chemitech.net.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hb.shxzukj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vm.chemitech.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://my.shtwfgs.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ky.lnxyls.cn

[J03] 字符串解析为日期
来源：http://kj.yuntaijiaju.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fb.chemitech.net.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ws.yuexingan06.cn

JS:   new Date("2024-01-02")
来源：http://nk.521024.cn

TS:   new Date("2024-01-02")
来源：http://py.shtwfgs.cn

Java: LocalDate.parse("2024-01-02")
来源：http://sm.huixiangedu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xw.nszjky.cn

Ruby: Date.parse("2024-01-02")
来源：http://zs.shxzskj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fc.shxzskj.cn

[J04] 时间戳与日期互转
来源：http://bp.yuexingan06.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vu.lnxyls.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qh.shtwfgs.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wk.nszjky.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fv.gzmigu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://be.muxihuayi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fs.nicolike.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fu.panjiajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kv.huanxung.cn

[J05] 时间加减（加 7 天）
来源：http://jg.yuntaijiaju.cn

Py:   now + timedelta(days=7)
来源：http://rw.wgjwhj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ye.yuntaijiaju.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://iz.bjjhwx.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ft.nicolike.cn

Java: LocalDate.now().plusDays(7)
来源：http://vn.nicolike.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rf.chemitech.net.cn

Ruby: Time.now + 7 * 86400
来源：http://oz.asd995.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ro.bjjhwx.cn

[J06] 计算两时间之差
来源：http://ks.huixiangedu.cn

Py:   (end - start).total_seconds()
来源：http://ll.lnxyls.cn

PHP:  $end->diff($start)->days;
来源：http://zl.shtwfgs.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ul.yuexingan06.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ua.huixiangedu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://yd.yuexingan06.cn

Go:   end.Sub(start).Hours()
来源：http://az.nicolike.cn

Ruby: end - start                 # 返回秒数
来源：http://gh.yuexingan06.cn

C#:   (end - start).TotalSeconds
来源：http://rx.yuexingan06.cn

[J07] 比较两个日期
来源：http://ch.yuntaijiaju.cn

Py:   d1 < d2;  d1 == d2
来源：http://ef.hahajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://aw.wgjwhj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jd.lnxyls.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yf.shxzukj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xf.szxytkj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vc.shxzskj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fp.chemitech.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://wb.shxzukj.cn

[J08] 提取年月日与星期
来源：http://yn.wgjwhj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ce.gzmigu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sq.bookmarksfly.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xh.szsharing.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gv.chemitech.net.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://eq.panjiajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://us.jctech888.com.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hd.newstarts.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yx.hahajie.cn

[J09] 时区处理
来源：http://hj.haigaiapp.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://oc.colortex.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gd.yuntaijiaju.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dv.wgjwhj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fp.bjjhwx.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lr.colortex.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vz.jctech888.com.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gn.jianghongdianzi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://um.lnxyls.cn

[J10] 取今天 / 本月第一天
来源：http://rj.szxytkj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ee.haigaiapp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wy.bookmarksfly.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wd.haigaiapp.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yg.asd995.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xg.colortex.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xc.nszjky.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zq.huanxung.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hm.bjjhwx.cn

================================================================================
来源：http://tb.nszjky.cn

K. JSON 与序列化
来源：http://yt.asd995.cn

================================================================================
来源：http://wy.nicolike.cn

[K01] 对象转 JSON 字符串
来源：http://gk.yuntaijiaju.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ys.hahajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rr.huanxung.cn

JS:   JSON.stringify(obj)
来源：http://vy.nszjky.cn

TS:   JSON.stringify(obj)
来源：http://sm.shxzskj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kz.shtwfgs.cn

Go:   json.Marshal(obj)
来源：http://mz.gzmigu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gp.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://sj.hnjuh.cn

[K02] JSON 字符串转对象
来源：http://en.shxzukj.cn

Py:   json.loads(s)
来源：http://nc.yuntaijiaju.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://om.huixinmuqiang.cn

JS:   JSON.parse(s)
来源：http://pl.asd995.cn

TS:   JSON.parse(s)
来源：http://ai.521024.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jb.chemitech.net.cn

Go:   json.Unmarshal(data, &v)
来源：http://hp.newstarts.cn

Ruby: JSON.parse(s)
来源：http://uu.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dq.huanxung.cn

[K03] JSON 美化输出（带缩进）
来源：http://xz.lnxyls.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ut.yuexingan06.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wb.asd995.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fh.shxzukj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ke.shxzukj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ye.chemitech.net.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ta.9csxet.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xe.gzmigu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fv.huixiangedu.cn

[K04] 读取 JSON 文件
来源：http://qo.nicolike.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fp.muxihuayi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://du.nszjky.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gz.szxytkj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nr.jctech888.com.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xp.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uw.bookmarksfly.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dl.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jg.shtwfgs.cn

[K05] 深拷贝对象
来源：http://ai.haigaiapp.cn

Py:   copy.deepcopy(obj)
来源：http://ji.huixinmuqiang.cn

PHP:  unserialize(serialize($obj));
来源：http://zj.huanxung.cn

JS:   structuredClone(obj)
来源：http://xe.asd995.cn

TS:   structuredClone(obj)
来源：http://ym.shtwfgs.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ts.szxytkj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ba.szsharing.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pw.nicolike.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ns.nszjky.cn

[K06] 解析 URL 查询串
来源：http://qi.huixinmuqiang.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://in.szsharing.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yn.nicolike.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lh.wgjwhj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://em.chemitech.net.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hm.szsharing.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vc.shxzukj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qp.haigaiapp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://td.chemitech.net.cn

[K07] 进制转换
来源：http://ih.shxzskj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ml.shtwfgs.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ji.nszjky.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uq.nicolike.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jn.panjiajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yn.huixinmuqiang.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qj.shxzskj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pk.yuntaijiaju.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ci.muxihuayi.cn

[K08] 二进制序列化（非 JSON）
来源：http://tv.colortex.cn

Py:   pickle.dumps(obj)
来源：http://oa.gzmigu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nd.muxihuayi.cn

JS:   v8.serialize(obj)        // Node
来源：http://ye.huixiangedu.cn

TS:   v8.serialize(obj)        // Node
来源：http://ov.yuntaijiaju.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ww.bookmarksfly.cn

Go:   encoding/gob
来源：http://we.bookmarksfly.cn

Ruby: Marshal.dump(obj)
来源：http://jd.yuntaijiaju.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://za.jctech888.com.cn

================================================================================
来源：http://ck.newstarts.cn

L. 网络请求
来源：http://ve.lnxyls.cn

================================================================================
来源：http://nn.newstarts.cn

[L01] 发送 GET 请求
来源：http://tf.haigaiapp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dj.shxzskj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ml.asd995.cn

JS:   await fetch(url)
来源：http://jx.huixinmuqiang.cn

TS:   await fetch(url)
来源：http://vv.shxzskj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kw.hahajie.cn

Go:   resp, err := http.Get(url)
来源：http://wc.521024.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://sj.nicolike.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ib.bjjhwx.cn

[L02] 发送 POST JSON
来源：http://op.bookmarksfly.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ur.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cg.shtwfgs.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ea.huixiangedu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sg.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://oe.huanxung.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wn.shxzukj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nk.hahajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lb.lnxyls.cn

[L03] 设置自定义请求头
来源：http://cu.panjiajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ix.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zv.bookmarksfly.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tp.shtwfgs.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ju.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yk.huanxung.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yk.hnjuh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ry.panjiajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ci.yuexingan06.cn

[L04] 设置超时
来源：http://gf.chemitech.net.cn

Py:   requests.get(url, timeout=5)
来源：http://af.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fb.jianghongdianzi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://el.521024.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ci.colortex.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bi.jctech888.com.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jy.shtwfgs.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ty.newstarts.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mk.asd995.cn

[L05] 上传文件（multipart）
来源：http://hf.colortex.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ss.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mw.newstarts.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qf.bookmarksfly.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lt.gzmigu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://to.yuexingan06.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://to.szsharing.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dn.asd995.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gt.hnjuh.cn

[L06] 解析响应为 JSON
来源：http://vg.nicolike.cn

Py:   resp.json()
来源：http://op.gzmigu.cn

PHP:  json_decode($body, true);
来源：http://vq.szxytkj.cn

JS:   await resp.json()
来源：http://nd.nszjky.cn

TS:   await resp.json()
来源：http://oo.panjiajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nf.huixinmuqiang.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gm.szsharing.cn

Ruby: JSON.parse(resp.body)
来源：http://by.huanxung.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zy.bookmarksfly.cn

[L07] 处理 HTTP 状态码
来源：http://qc.jctech888.com.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mj.newstarts.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://te.bjjhwx.cn

JS:   resp.ok;  resp.status
来源：http://bs.nszjky.cn

TS:   resp.ok;  resp.status
来源：http://bq.szsharing.cn

Java: resp.statusCode()
来源：http://yc.szxytkj.cn

Go:   resp.StatusCode
来源：http://zj.huixinmuqiang.cn

Ruby: resp.code.to_i
来源：http://de.szxytkj.cn

C#:   (int)resp.StatusCode
来源：http://fx.huanxung.cn

[L08] 并发请求多个地址
来源：http://io.jianghongdianzi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zi.hahajie.cn

PHP:  curl_multi_init() 系列
来源：http://rn.asd995.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://se.huanxung.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vj.muxihuayi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ci.bookmarksfly.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gk.lnxyls.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qa.huixinmuqiang.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bi.panjiajie.cn

================================================================================
来源：http://oe.chemitech.net.cn

M. 命令行 / 进程 / 环境
来源：http://tw.huixiangedu.cn

================================================================================
来源：http://nu.hnjuh.cn

[M01] 读取命令行参数
来源：http://ru.wgjwhj.cn

Py:   sys.argv[1:]
来源：http://oj.wgjwhj.cn

PHP:  $argv;  $argc;
来源：http://ly.colortex.cn

JS:   process.argv.slice(2)
来源：http://jf.521024.cn

TS:   process.argv.slice(2)
来源：http://yd.chemitech.net.cn

Java: args 数组（main 方法参数）
来源：http://ln.huanxung.cn

Go:   os.Args[1:]
来源：http://od.9csxet.cn

Ruby: ARGV
来源：http://xu.jianghongdianzi.cn

C#:   args 数组（Main 方法参数）
来源：http://xh.colortex.cn

[M02] 读取环境变量
来源：http://rf.haigaiapp.cn

Py:   os.environ.get("HOME")
来源：http://kx.szsharing.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fm.521024.cn

JS:   process.env.HOME
来源：http://pw.9csxet.cn

TS:   process.env.HOME
来源：http://yt.gzmigu.cn

Java: System.getenv("HOME")
来源：http://jz.bjjhwx.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gd.haigaiapp.cn

Ruby: ENV["HOME"]
来源：http://jn.bookmarksfly.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yw.colortex.cn

[M03] 执行外部命令
来源：http://qn.shtwfgs.cn


<!-- 参考信息 -->