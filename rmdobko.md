代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://da.huixiangedu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://oy.shtwfgs.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sc.hahajie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ch.gzmigu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hk.bjjhwx.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://we.shxzukj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bq.chemitech.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ir.shxzukj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://df.9csxet.cn

[I07] 忽略大小写与多行模式
来源：http://ex.wgjwhj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mn.jctech888.com.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://oc.newstarts.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://il.bjjhwx.cn

TS:   /error/gim
来源：http://xz.szsharing.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bk.asd995.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://td.nicolike.cn

Ruby: s.scan(/error/i)
来源：http://wk.shxzukj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jd.521024.cn

[I08] 贪婪与非贪婪匹配
来源：http://pi.nszjky.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://to.jctech888.com.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yz.szsharing.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kh.bookmarksfly.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tb.colortex.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nr.haigaiapp.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ci.shtwfgs.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ax.lnxyls.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ak.hnjuh.cn

================================================================================
来源：http://ff.muxihuayi.cn

J. 日期与时间
来源：http://iw.huanxung.cn

================================================================================
来源：http://kg.haigaiapp.cn

[J01] 获取当前时间
来源：http://oq.nszjky.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ed.huixinmuqiang.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xf.yuexingan06.cn

JS:   new Date();  Date.now()
来源：http://wv.szxytkj.cn

TS:   new Date();  Date.now()
来源：http://dh.shxzskj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hx.newstarts.cn

Go:   time.Now()
来源：http://mw.huanxung.cn

Ruby: Time.now
来源：http://tb.huixinmuqiang.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kr.gzmigu.cn

[J02] 格式化输出
来源：http://it.nszjky.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://om.haigaiapp.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fq.szxytkj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qz.asd995.cn

TS:   d.toISOString()
来源：http://vh.asd995.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ee.szxytkj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lj.yuexingan06.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qr.nszjky.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qg.shxzskj.cn

[J03] 字符串解析为日期
来源：http://df.newstarts.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ok.panjiajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ht.shtwfgs.cn

JS:   new Date("2024-01-02")
来源：http://iv.9csxet.cn

TS:   new Date("2024-01-02")
来源：http://rt.szxytkj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://sw.colortex.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qx.bookmarksfly.cn

Ruby: Date.parse("2024-01-02")
来源：http://gd.nicolike.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rs.lnxyls.cn

[J04] 时间戳与日期互转
来源：http://oq.hahajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wf.yuntaijiaju.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ru.wgjwhj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://us.shxzukj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zv.muxihuayi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ri.asd995.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rw.jctech888.com.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ge.haigaiapp.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ib.chemitech.net.cn

[J05] 时间加减（加 7 天）
来源：http://rw.nszjky.cn

Py:   now + timedelta(days=7)
来源：http://ka.shtwfgs.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mi.shtwfgs.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tk.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://oy.szsharing.cn

Java: LocalDate.now().plusDays(7)
来源：http://mg.shxzskj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zs.yuexingan06.cn

Ruby: Time.now + 7 * 86400
来源：http://fo.nszjky.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jl.shtwfgs.cn

[J06] 计算两时间之差
来源：http://ll.huixinmuqiang.cn

Py:   (end - start).total_seconds()
来源：http://ff.shxzskj.cn

PHP:  $end->diff($start)->days;
来源：http://ge.bookmarksfly.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ge.nszjky.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://di.9csxet.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lm.jianghongdianzi.cn

Go:   end.Sub(start).Hours()
来源：http://kt.gzmigu.cn

Ruby: end - start                 # 返回秒数
来源：http://ee.shxzukj.cn

C#:   (end - start).TotalSeconds
来源：http://uf.yuexingan06.cn

[J07] 比较两个日期
来源：http://qj.nszjky.cn

Py:   d1 < d2;  d1 == d2
来源：http://qb.jctech888.com.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dn.huanxung.cn

JS:   d1.getTime() < d2.getTime()
来源：http://yf.newstarts.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fd.szxytkj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ij.yuexingan06.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gt.szxytkj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ov.huanxung.cn

C#:   d1 < d2;  d1 == d2
来源：http://na.521024.cn

[J08] 提取年月日与星期
来源：http://sl.jctech888.com.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ed.9csxet.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ur.lnxyls.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qe.hnjuh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mk.colortex.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://um.huixinmuqiang.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://im.asd995.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ri.haigaiapp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bl.newstarts.cn

[J09] 时区处理
来源：http://qr.yuexingan06.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fu.bookmarksfly.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ba.hnjuh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://go.huanxung.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ix.shxzskj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kv.yuntaijiaju.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://aa.colortex.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vy.hahajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zs.wgjwhj.cn

[J10] 取今天 / 本月第一天
来源：http://wr.szxytkj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wm.muxihuayi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ul.szxytkj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ln.521024.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wk.wgjwhj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mo.hahajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wh.asd995.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ir.haigaiapp.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lp.shxzukj.cn

================================================================================
来源：http://md.shxzskj.cn

K. JSON 与序列化
来源：http://nv.shxzskj.cn

================================================================================
来源：http://hj.9csxet.cn

[K01] 对象转 JSON 字符串
来源：http://nv.521024.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yo.szsharing.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fj.shxzukj.cn

JS:   JSON.stringify(obj)
来源：http://fw.shtwfgs.cn

TS:   JSON.stringify(obj)
来源：http://rb.shtwfgs.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mc.szsharing.cn

Go:   json.Marshal(obj)
来源：http://rq.jianghongdianzi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rj.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lz.bookmarksfly.cn

[K02] JSON 字符串转对象
来源：http://ce.hahajie.cn

Py:   json.loads(s)
来源：http://gm.newstarts.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bh.huanxung.cn

JS:   JSON.parse(s)
来源：http://pt.chemitech.net.cn

TS:   JSON.parse(s)
来源：http://lk.lnxyls.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fv.huixiangedu.cn

Go:   json.Unmarshal(data, &v)
来源：http://mt.521024.cn

Ruby: JSON.parse(s)
来源：http://pf.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tp.yuntaijiaju.cn

[K03] JSON 美化输出（带缩进）
来源：http://ij.huixinmuqiang.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cn.huixiangedu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ua.521024.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pu.bjjhwx.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://jz.huixiangedu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://iu.shxzukj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zl.szsharing.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pi.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sf.huanxung.cn

[K04] 读取 JSON 文件
来源：http://fx.yuexingan06.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ba.haigaiapp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wr.yuntaijiaju.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wl.huixiangedu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lx.9csxet.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dc.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zk.bjjhwx.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ic.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wr.jianghongdianzi.cn

[K05] 深拷贝对象
来源：http://ks.asd995.cn

Py:   copy.deepcopy(obj)
来源：http://di.haigaiapp.cn

PHP:  unserialize(serialize($obj));
来源：http://em.jctech888.com.cn

JS:   structuredClone(obj)
来源：http://ws.hnjuh.cn

TS:   structuredClone(obj)
来源：http://ja.newstarts.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://cf.hahajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://de.wgjwhj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ig.hnjuh.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://on.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://et.hahajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ma.asd995.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ya.hnjuh.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fz.shtwfgs.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wg.hahajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://me.bookmarksfly.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://az.hahajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vy.yuexingan06.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://co.muxihuayi.cn

[K07] 进制转换
来源：http://sg.jctech888.com.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qu.jianghongdianzi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fd.yuexingan06.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mx.shxzskj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ih.lnxyls.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rt.shxzskj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kd.huixiangedu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mb.hahajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sr.szxytkj.cn

[K08] 二进制序列化（非 JSON）
来源：http://pj.shxzukj.cn

Py:   pickle.dumps(obj)
来源：http://nu.huanxung.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://on.lnxyls.cn

JS:   v8.serialize(obj)        // Node
来源：http://ol.nicolike.cn

TS:   v8.serialize(obj)        // Node
来源：http://io.jianghongdianzi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://az.jctech888.com.cn

Go:   encoding/gob
来源：http://mh.huixinmuqiang.cn

Ruby: Marshal.dump(obj)
来源：http://of.huixiangedu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://om.panjiajie.cn

================================================================================
来源：http://st.hahajie.cn

L. 网络请求
来源：http://qt.colortex.cn

================================================================================
来源：http://yb.shxzskj.cn

[L01] 发送 GET 请求
来源：http://qg.nicolike.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mr.colortex.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hi.shxzukj.cn

JS:   await fetch(url)
来源：http://hi.jianghongdianzi.cn

TS:   await fetch(url)
来源：http://ok.asd995.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zv.gzmigu.cn

Go:   resp, err := http.Get(url)
来源：http://nb.shtwfgs.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zd.colortex.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tg.521024.cn

[L02] 发送 POST JSON
来源：http://zf.newstarts.cn

Py:   requests.post(url, json={"a": 1})
来源：http://jh.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vb.muxihuayi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fr.bookmarksfly.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fj.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hx.asd995.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qw.szxytkj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fa.muxihuayi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gd.gzmigu.cn

[L03] 设置自定义请求头
来源：http://ap.jctech888.com.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jj.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xe.9csxet.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hm.muxihuayi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ow.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ln.hahajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fs.chemitech.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pf.panjiajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pt.muxihuayi.cn

[L04] 设置超时
来源：http://ds.huixinmuqiang.cn

Py:   requests.get(url, timeout=5)
来源：http://an.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qn.yuntaijiaju.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ii.hnjuh.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fg.shxzskj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nr.lnxyls.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kw.bookmarksfly.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ie.bjjhwx.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tm.muxihuayi.cn

[L05] 上传文件（multipart）
来源：http://bk.shtwfgs.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jj.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gh.huixiangedu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hc.szsharing.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ve.bookmarksfly.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ms.shxzskj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xx.newstarts.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tp.nszjky.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mi.shxzskj.cn

[L06] 解析响应为 JSON
来源：http://vn.yuntaijiaju.cn

Py:   resp.json()
来源：http://zw.huanxung.cn

PHP:  json_decode($body, true);
来源：http://ih.huixiangedu.cn

JS:   await resp.json()
来源：http://gg.bjjhwx.cn

TS:   await resp.json()
来源：http://wh.haigaiapp.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ky.nszjky.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jm.nszjky.cn

Ruby: JSON.parse(resp.body)
来源：http://yp.yuexingan06.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fa.haigaiapp.cn

[L07] 处理 HTTP 状态码
来源：http://ik.shxzskj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ux.jctech888.com.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cc.shtwfgs.cn

JS:   resp.ok;  resp.status
来源：http://vq.bookmarksfly.cn

TS:   resp.ok;  resp.status
来源：http://mk.colortex.cn

Java: resp.statusCode()
来源：http://mt.shxzskj.cn

Go:   resp.StatusCode
来源：http://rk.yuntaijiaju.cn

Ruby: resp.code.to_i
来源：http://rr.yuntaijiaju.cn

C#:   (int)resp.StatusCode
来源：http://nk.yuexingan06.cn

[L08] 并发请求多个地址
来源：http://uj.9csxet.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://af.muxihuayi.cn

PHP:  curl_multi_init() 系列
来源：http://yd.panjiajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yv.bookmarksfly.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xa.yuexingan06.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yb.wgjwhj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wc.521024.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ao.jctech888.com.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mn.huixiangedu.cn

================================================================================
来源：http://eq.szsharing.cn

M. 命令行 / 进程 / 环境
来源：http://el.wgjwhj.cn

================================================================================
来源：http://lj.yuntaijiaju.cn

[M01] 读取命令行参数
来源：http://gq.panjiajie.cn

Py:   sys.argv[1:]
来源：http://jc.haigaiapp.cn

PHP:  $argv;  $argc;
来源：http://ys.newstarts.cn

JS:   process.argv.slice(2)
来源：http://yg.asd995.cn

TS:   process.argv.slice(2)
来源：http://bx.nicolike.cn

Java: args 数组（main 方法参数）
来源：http://fj.chemitech.net.cn

Go:   os.Args[1:]
来源：http://gu.asd995.cn

Ruby: ARGV
来源：http://ot.nicolike.cn

C#:   args 数组（Main 方法参数）
来源：http://jz.shxzukj.cn

[M02] 读取环境变量
来源：http://fl.huanxung.cn

Py:   os.environ.get("HOME")
来源：http://og.lnxyls.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vr.nicolike.cn

JS:   process.env.HOME
来源：http://wk.jianghongdianzi.cn

TS:   process.env.HOME
来源：http://cj.huixinmuqiang.cn

Java: System.getenv("HOME")
来源：http://og.gzmigu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qe.shxzskj.cn

Ruby: ENV["HOME"]
来源：http://va.hnjuh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fj.nszjky.cn

[M03] 执行外部命令
来源：http://sg.bjjhwx.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mq.huixinmuqiang.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kw.chemitech.net.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://du.colortex.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wq.colortex.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pi.muxihuayi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vs.yuntaijiaju.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xy.lnxyls.cn

C#:   Process.Start("ls", "-l");
来源：http://py.jctech888.com.cn


<!-- 参考信息 -->