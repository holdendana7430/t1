代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ae.shxzskj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hv.bjjhwx.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jv.shxzskj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nx.521024.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fc.shtwfgs.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pz.muxihuayi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rr.panjiajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cx.szsharing.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ng.yuexingan06.cn

[I07] 忽略大小写与多行模式
来源：http://gj.yuexingan06.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qf.chemitech.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yq.huixinmuqiang.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nk.asd995.cn

TS:   /error/gim
来源：http://kk.huanxung.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ff.szxytkj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ux.colortex.cn

Ruby: s.scan(/error/i)
来源：http://dv.szsharing.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hp.jctech888.com.cn

[I08] 贪婪与非贪婪匹配
来源：http://ov.wgjwhj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ct.nszjky.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tr.muxihuayi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bc.haigaiapp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nb.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zn.huixinmuqiang.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xb.nicolike.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://px.lnxyls.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mh.nszjky.cn

================================================================================
来源：http://ga.shxzukj.cn

J. 日期与时间
来源：http://ic.szxytkj.cn

================================================================================
来源：http://vn.newstarts.cn

[J01] 获取当前时间
来源：http://cj.muxihuayi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fl.521024.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://si.huixinmuqiang.cn

JS:   new Date();  Date.now()
来源：http://xt.panjiajie.cn

TS:   new Date();  Date.now()
来源：http://nb.panjiajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://xp.yuexingan06.cn

Go:   time.Now()
来源：http://lq.shxzukj.cn

Ruby: Time.now
来源：http://jl.szxytkj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pk.asd995.cn

[J02] 格式化输出
来源：http://ni.yuntaijiaju.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xz.shxzukj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qv.nicolike.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ln.jctech888.com.cn

TS:   d.toISOString()
来源：http://rr.muxihuayi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qb.haigaiapp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ti.lnxyls.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jf.lnxyls.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wt.newstarts.cn

[J03] 字符串解析为日期
来源：http://lx.jianghongdianzi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ik.521024.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tr.nszjky.cn

JS:   new Date("2024-01-02")
来源：http://zj.9csxet.cn

TS:   new Date("2024-01-02")
来源：http://jo.jianghongdianzi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://en.jctech888.com.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ln.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://tl.wgjwhj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hv.jianghongdianzi.cn

[J04] 时间戳与日期互转
来源：http://en.gzmigu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://oh.chemitech.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kw.521024.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://it.nicolike.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tt.521024.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hu.nicolike.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nh.asd995.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ps.jctech888.com.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pk.hnjuh.cn

[J05] 时间加减（加 7 天）
来源：http://de.nszjky.cn

Py:   now + timedelta(days=7)
来源：http://cp.huanxung.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sc.yuexingan06.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ql.yuntaijiaju.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qu.9csxet.cn

Java: LocalDate.now().plusDays(7)
来源：http://ec.yuntaijiaju.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ka.wgjwhj.cn

Ruby: Time.now + 7 * 86400
来源：http://yt.panjiajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ks.bjjhwx.cn

[J06] 计算两时间之差
来源：http://wq.jianghongdianzi.cn

Py:   (end - start).total_seconds()
来源：http://rj.hahajie.cn

PHP:  $end->diff($start)->days;
来源：http://au.huanxung.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uh.jctech888.com.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uq.huixiangedu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://in.szsharing.cn

Go:   end.Sub(start).Hours()
来源：http://gg.hnjuh.cn

Ruby: end - start                 # 返回秒数
来源：http://mb.hahajie.cn

C#:   (end - start).TotalSeconds
来源：http://bg.huanxung.cn

[J07] 比较两个日期
来源：http://hd.521024.cn

Py:   d1 < d2;  d1 == d2
来源：http://ue.bookmarksfly.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mp.szsharing.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ar.9csxet.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xh.hahajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ms.muxihuayi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qk.bjjhwx.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xy.bjjhwx.cn

C#:   d1 < d2;  d1 == d2
来源：http://ak.muxihuayi.cn

[J08] 提取年月日与星期
来源：http://jp.9csxet.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zf.gzmigu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tb.huixiangedu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tx.huixiangedu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oe.hahajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cl.newstarts.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pm.nicolike.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://eq.shxzukj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mn.shtwfgs.cn

[J09] 时区处理
来源：http://sm.yuntaijiaju.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lo.muxihuayi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fg.huanxung.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vo.wgjwhj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bm.hnjuh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ue.huanxung.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lj.nszjky.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://oz.haigaiapp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zp.szsharing.cn

[J10] 取今天 / 本月第一天
来源：http://qq.panjiajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wb.szsharing.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xw.gzmigu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fj.hnjuh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rt.haigaiapp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xu.lnxyls.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bv.yuntaijiaju.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kl.haigaiapp.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wu.gzmigu.cn

================================================================================
来源：http://wk.shxzskj.cn

K. JSON 与序列化
来源：http://gx.haigaiapp.cn

================================================================================
来源：http://fz.gzmigu.cn

[K01] 对象转 JSON 字符串
来源：http://ya.shxzukj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ev.521024.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://sz.hahajie.cn

JS:   JSON.stringify(obj)
来源：http://ac.yuexingan06.cn

TS:   JSON.stringify(obj)
来源：http://dd.huixiangedu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://oo.colortex.cn

Go:   json.Marshal(obj)
来源：http://dq.wgjwhj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://yy.hnjuh.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://uc.shxzskj.cn

[K02] JSON 字符串转对象
来源：http://di.szxytkj.cn

Py:   json.loads(s)
来源：http://wy.shxzskj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hu.muxihuayi.cn

JS:   JSON.parse(s)
来源：http://yl.hahajie.cn

TS:   JSON.parse(s)
来源：http://bx.bookmarksfly.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fo.9csxet.cn

Go:   json.Unmarshal(data, &v)
来源：http://kr.shtwfgs.cn

Ruby: JSON.parse(s)
来源：http://rp.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vz.yuexingan06.cn

[K03] JSON 美化输出（带缩进）
来源：http://dl.bjjhwx.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vo.jctech888.com.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lr.hahajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ba.nicolike.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ns.shtwfgs.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yz.hnjuh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mn.yuntaijiaju.cn

Ruby: JSON.pretty_generate(obj)
来源：http://uy.szxytkj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fy.jctech888.com.cn

[K04] 读取 JSON 文件
来源：http://pg.szsharing.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kw.hnjuh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tt.shxzukj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ao.asd995.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cn.yuexingan06.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fa.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tf.hnjuh.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vy.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kv.nicolike.cn

[K05] 深拷贝对象
来源：http://vz.gzmigu.cn

Py:   copy.deepcopy(obj)
来源：http://ft.wgjwhj.cn

PHP:  unserialize(serialize($obj));
来源：http://vh.huixiangedu.cn

JS:   structuredClone(obj)
来源：http://is.huixiangedu.cn

TS:   structuredClone(obj)
来源：http://bs.521024.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ly.haigaiapp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ez.lnxyls.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ua.panjiajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cf.huixinmuqiang.cn

[K06] 解析 URL 查询串
来源：http://dg.yuexingan06.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yq.haigaiapp.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qu.panjiajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eu.asd995.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yl.asd995.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sb.shxzskj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://tq.huanxung.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fv.9csxet.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uu.shxzskj.cn

[K07] 进制转换
来源：http://af.bjjhwx.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pj.shxzskj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pl.jctech888.com.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bz.szsharing.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wy.muxihuayi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pi.panjiajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ct.hnjuh.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mc.jianghongdianzi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://eg.yuexingan06.cn

[K08] 二进制序列化（非 JSON）
来源：http://zn.nicolike.cn

Py:   pickle.dumps(obj)
来源：http://mi.hahajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gw.nicolike.cn

JS:   v8.serialize(obj)        // Node
来源：http://es.521024.cn

TS:   v8.serialize(obj)        // Node
来源：http://em.szxytkj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://aq.gzmigu.cn

Go:   encoding/gob
来源：http://hf.muxihuayi.cn

Ruby: Marshal.dump(obj)
来源：http://ji.szsharing.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dl.panjiajie.cn

================================================================================
来源：http://fx.yuntaijiaju.cn

L. 网络请求
来源：http://ee.yuntaijiaju.cn

================================================================================
来源：http://xk.nszjky.cn

[L01] 发送 GET 请求
来源：http://oq.muxihuayi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://te.shtwfgs.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vt.yuntaijiaju.cn

JS:   await fetch(url)
来源：http://fn.nszjky.cn

TS:   await fetch(url)
来源：http://ol.bookmarksfly.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nz.nicolike.cn

Go:   resp, err := http.Get(url)
来源：http://ce.bookmarksfly.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hs.haigaiapp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tq.nicolike.cn

[L02] 发送 POST JSON
来源：http://wu.huanxung.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zj.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://io.newstarts.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qw.9csxet.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vb.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qw.haigaiapp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jd.jctech888.com.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bz.haigaiapp.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vx.9csxet.cn

[L03] 设置自定义请求头
来源：http://lf.muxihuayi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bp.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kv.shxzskj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qh.muxihuayi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kh.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xg.asd995.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tj.huixinmuqiang.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tj.yuntaijiaju.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wh.hahajie.cn

[L04] 设置超时
来源：http://yp.lnxyls.cn

Py:   requests.get(url, timeout=5)
来源：http://xr.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ri.521024.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sx.chemitech.net.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xi.yuexingan06.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://iv.9csxet.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ow.wgjwhj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ug.haigaiapp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bi.panjiajie.cn

[L05] 上传文件（multipart）
来源：http://kv.newstarts.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://no.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://or.panjiajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lo.huixinmuqiang.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ux.huixinmuqiang.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bn.szsharing.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wf.shxzukj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kg.szxytkj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jv.yuexingan06.cn

[L06] 解析响应为 JSON
来源：http://sb.bjjhwx.cn

Py:   resp.json()
来源：http://pu.szsharing.cn

PHP:  json_decode($body, true);
来源：http://hm.panjiajie.cn

JS:   await resp.json()
来源：http://cv.panjiajie.cn

TS:   await resp.json()
来源：http://jn.nicolike.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nn.shtwfgs.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lh.hnjuh.cn

Ruby: JSON.parse(resp.body)
来源：http://kc.haigaiapp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mj.muxihuayi.cn

[L07] 处理 HTTP 状态码
来源：http://qs.huanxung.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dl.haigaiapp.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://av.chemitech.net.cn

JS:   resp.ok;  resp.status
来源：http://ty.jianghongdianzi.cn

TS:   resp.ok;  resp.status
来源：http://wr.521024.cn

Java: resp.statusCode()
来源：http://mz.521024.cn

Go:   resp.StatusCode
来源：http://qo.jianghongdianzi.cn

Ruby: resp.code.to_i
来源：http://ew.colortex.cn

C#:   (int)resp.StatusCode
来源：http://ph.521024.cn

[L08] 并发请求多个地址
来源：http://wo.huanxung.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sc.bjjhwx.cn

PHP:  curl_multi_init() 系列
来源：http://yl.jctech888.com.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gv.bookmarksfly.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fa.nicolike.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wu.newstarts.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rj.bjjhwx.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gt.haigaiapp.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yv.nicolike.cn

================================================================================
来源：http://id.nszjky.cn

M. 命令行 / 进程 / 环境
来源：http://er.szxytkj.cn

================================================================================
来源：http://wp.wgjwhj.cn

[M01] 读取命令行参数
来源：http://qo.huanxung.cn

Py:   sys.argv[1:]
来源：http://gf.shxzskj.cn

PHP:  $argv;  $argc;
来源：http://rz.jianghongdianzi.cn

JS:   process.argv.slice(2)
来源：http://yk.szxytkj.cn

TS:   process.argv.slice(2)
来源：http://vb.bookmarksfly.cn

Java: args 数组（main 方法参数）
来源：http://up.hnjuh.cn

Go:   os.Args[1:]
来源：http://zp.huanxung.cn

Ruby: ARGV
来源：http://mf.wgjwhj.cn

C#:   args 数组（Main 方法参数）
来源：http://js.szsharing.cn

[M02] 读取环境变量
来源：http://xi.gzmigu.cn

Py:   os.environ.get("HOME")
来源：http://qm.huanxung.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zb.yuexingan06.cn

JS:   process.env.HOME
来源：http://ma.lnxyls.cn

TS:   process.env.HOME
来源：http://ip.wgjwhj.cn

Java: System.getenv("HOME")
来源：http://hr.szxytkj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ft.asd995.cn

Ruby: ENV["HOME"]
来源：http://oa.jianghongdianzi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://em.hnjuh.cn

[M03] 执行外部命令
来源：http://wg.lnxyls.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cl.newstarts.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yj.bookmarksfly.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zi.yuexingan06.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://by.haigaiapp.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zf.huixiangedu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://yy.colortex.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ie.huixiangedu.cn

C#:   Process.Start("ls", "-l");
来源：http://mx.bookmarksfly.cn


<!-- 参考信息 -->