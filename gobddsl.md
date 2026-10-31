代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://co.muxihuayi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bf.nszjky.cn

Ruby: s.split(/\s*,\s*/)
来源：http://hh.chemitech.net.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sf.lnxyls.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://le.huixinmuqiang.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uc.9csxet.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yo.huanxung.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xp.muxihuayi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uz.huanxung.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qr.shxzskj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qs.hahajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zs.panjiajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yb.muxihuayi.cn

[I07] 忽略大小写与多行模式
来源：http://nx.jctech888.com.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gk.chemitech.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sx.huixinmuqiang.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://iv.huixiangedu.cn

TS:   /error/gim
来源：http://lo.nicolike.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cj.huixiangedu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xl.shxzskj.cn

Ruby: s.scan(/error/i)
来源：http://ae.shxzukj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cp.muxihuayi.cn

[I08] 贪婪与非贪婪匹配
来源：http://nl.huanxung.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fe.hnjuh.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lt.szxytkj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yp.jianghongdianzi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ro.shxzskj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://rk.huixiangedu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://db.szxytkj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://no.huixinmuqiang.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qi.yuntaijiaju.cn

================================================================================
来源：http://sk.yuntaijiaju.cn

J. 日期与时间
来源：http://ps.chemitech.net.cn

================================================================================
来源：http://cj.szsharing.cn

[J01] 获取当前时间
来源：http://bz.szxytkj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://jf.521024.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cb.shxzukj.cn

JS:   new Date();  Date.now()
来源：http://nx.shxzukj.cn

TS:   new Date();  Date.now()
来源：http://ri.nicolike.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vz.muxihuayi.cn

Go:   time.Now()
来源：http://ju.yuexingan06.cn

Ruby: Time.now
来源：http://zv.haigaiapp.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jn.szsharing.cn

[J02] 格式化输出
来源：http://ys.shxzskj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xt.bookmarksfly.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zn.huanxung.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mk.shtwfgs.cn

TS:   d.toISOString()
来源：http://ry.shtwfgs.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vp.huixinmuqiang.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ci.bookmarksfly.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ml.muxihuayi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ti.nicolike.cn

[J03] 字符串解析为日期
来源：http://yt.asd995.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fu.hahajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ij.hahajie.cn

JS:   new Date("2024-01-02")
来源：http://gl.9csxet.cn

TS:   new Date("2024-01-02")
来源：http://sl.jianghongdianzi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ph.bookmarksfly.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://um.nszjky.cn

Ruby: Date.parse("2024-01-02")
来源：http://vk.szsharing.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yx.szxytkj.cn

[J04] 时间戳与日期互转
来源：http://on.wgjwhj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ba.muxihuayi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://px.szxytkj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gj.hnjuh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://nv.jctech888.com.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ws.521024.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zy.hahajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sq.gzmigu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qk.shxzskj.cn

[J05] 时间加减（加 7 天）
来源：http://nl.9csxet.cn

Py:   now + timedelta(days=7)
来源：http://nv.shxzukj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xl.bjjhwx.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vi.gzmigu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rr.newstarts.cn

Java: LocalDate.now().plusDays(7)
来源：http://ir.bookmarksfly.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nc.hnjuh.cn

Ruby: Time.now + 7 * 86400
来源：http://vi.bjjhwx.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qv.gzmigu.cn

[J06] 计算两时间之差
来源：http://mc.shxzukj.cn

Py:   (end - start).total_seconds()
来源：http://ne.colortex.cn

PHP:  $end->diff($start)->days;
来源：http://oz.bjjhwx.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gy.huixinmuqiang.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ro.szsharing.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qa.shxzukj.cn

Go:   end.Sub(start).Hours()
来源：http://bl.haigaiapp.cn

Ruby: end - start                 # 返回秒数
来源：http://kj.huixiangedu.cn

C#:   (end - start).TotalSeconds
来源：http://yh.shtwfgs.cn

[J07] 比较两个日期
来源：http://wv.521024.cn

Py:   d1 < d2;  d1 == d2
来源：http://yg.colortex.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wg.9csxet.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hq.huixinmuqiang.cn

TS:   d1.getTime() < d2.getTime()
来源：http://kz.huixinmuqiang.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ph.yuntaijiaju.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kk.hahajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wd.bookmarksfly.cn

C#:   d1 < d2;  d1 == d2
来源：http://wk.hnjuh.cn

[J08] 提取年月日与星期
来源：http://ma.asd995.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fq.muxihuayi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cx.yuntaijiaju.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://eo.521024.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://sg.szsharing.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xe.jctech888.com.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ue.jctech888.com.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vq.chemitech.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bl.wgjwhj.cn

[J09] 时区处理
来源：http://kq.521024.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://um.chemitech.net.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pe.hnjuh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dr.newstarts.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jv.wgjwhj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://eu.shtwfgs.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dm.szxytkj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vj.yuntaijiaju.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sb.shtwfgs.cn

[J10] 取今天 / 本月第一天
来源：http://pf.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://aa.bjjhwx.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://db.shxzskj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mj.lnxyls.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dk.huixiangedu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tx.panjiajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hl.lnxyls.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ji.szsharing.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ar.colortex.cn

================================================================================
来源：http://lq.shtwfgs.cn

K. JSON 与序列化
来源：http://bb.shxzukj.cn

================================================================================
来源：http://gt.muxihuayi.cn

[K01] 对象转 JSON 字符串
来源：http://af.szxytkj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bs.huanxung.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ll.yuexingan06.cn

JS:   JSON.stringify(obj)
来源：http://pw.chemitech.net.cn

TS:   JSON.stringify(obj)
来源：http://yp.jctech888.com.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zh.shtwfgs.cn

Go:   json.Marshal(obj)
来源：http://hj.wgjwhj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bc.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://eb.shxzukj.cn

[K02] JSON 字符串转对象
来源：http://zh.gzmigu.cn

Py:   json.loads(s)
来源：http://bc.bjjhwx.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://eu.nszjky.cn

JS:   JSON.parse(s)
来源：http://gs.yuexingan06.cn

TS:   JSON.parse(s)
来源：http://kt.huanxung.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fp.huixiangedu.cn

Go:   json.Unmarshal(data, &v)
来源：http://ho.szsharing.cn

Ruby: JSON.parse(s)
来源：http://ph.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://oe.huixinmuqiang.cn

[K03] JSON 美化输出（带缩进）
来源：http://ge.newstarts.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rl.lnxyls.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://df.asd995.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ys.9csxet.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://dy.colortex.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mf.wgjwhj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://op.muxihuayi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ki.nszjky.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mw.chemitech.net.cn

[K04] 读取 JSON 文件
来源：http://do.hahajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kh.nicolike.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ac.nicolike.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gc.hnjuh.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://if.chemitech.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kp.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://iv.521024.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gi.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uu.panjiajie.cn

[K05] 深拷贝对象
来源：http://kq.lnxyls.cn

Py:   copy.deepcopy(obj)
来源：http://lb.shxzukj.cn

PHP:  unserialize(serialize($obj));
来源：http://id.nszjky.cn

JS:   structuredClone(obj)
来源：http://uo.huanxung.cn

TS:   structuredClone(obj)
来源：http://im.muxihuayi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jj.shxzukj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zr.huixinmuqiang.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fp.bookmarksfly.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cc.szsharing.cn

[K06] 解析 URL 查询串
来源：http://oi.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xx.muxihuayi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cc.haigaiapp.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wv.gzmigu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ce.huixinmuqiang.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://od.szsharing.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://so.nicolike.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uh.nicolike.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://di.hnjuh.cn

[K07] 进制转换
来源：http://sm.huanxung.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lr.chemitech.net.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ee.szsharing.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lu.szsharing.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ds.jianghongdianzi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vg.yuntaijiaju.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://he.muxihuayi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ge.haigaiapp.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://oo.huanxung.cn

[K08] 二进制序列化（非 JSON）
来源：http://qu.shxzukj.cn

Py:   pickle.dumps(obj)
来源：http://bt.lnxyls.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mc.shxzskj.cn

JS:   v8.serialize(obj)        // Node
来源：http://fp.lnxyls.cn

TS:   v8.serialize(obj)        // Node
来源：http://qv.gzmigu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bg.yuntaijiaju.cn

Go:   encoding/gob
来源：http://si.haigaiapp.cn

Ruby: Marshal.dump(obj)
来源：http://is.asd995.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pv.szsharing.cn

================================================================================
来源：http://qm.newstarts.cn

L. 网络请求
来源：http://jt.newstarts.cn

================================================================================
来源：http://ub.szsharing.cn

[L01] 发送 GET 请求
来源：http://fr.wgjwhj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rt.wgjwhj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ke.jianghongdianzi.cn

JS:   await fetch(url)
来源：http://rq.colortex.cn

TS:   await fetch(url)
来源：http://qs.yuntaijiaju.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ub.szsharing.cn

Go:   resp, err := http.Get(url)
来源：http://sb.haigaiapp.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hd.newstarts.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://eo.gzmigu.cn

[L02] 发送 POST JSON
来源：http://xz.shtwfgs.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pr.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://km.jianghongdianzi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uo.hnjuh.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yu.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sq.shxzskj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uq.szxytkj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kj.colortex.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ys.gzmigu.cn

[L03] 设置自定义请求头
来源：http://ch.hnjuh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tb.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://np.wgjwhj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tb.huanxung.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jm.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hb.bookmarksfly.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sf.nicolike.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zz.muxihuayi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ux.asd995.cn

[L04] 设置超时
来源：http://yq.huixinmuqiang.cn

Py:   requests.get(url, timeout=5)
来源：http://if.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mn.nszjky.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://af.bookmarksfly.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vf.yuntaijiaju.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sw.hahajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://aq.hahajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ub.521024.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tf.szxytkj.cn

[L05] 上传文件（multipart）
来源：http://xw.szxytkj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wr.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ji.panjiajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qn.chemitech.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ro.shxzskj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kg.hnjuh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uo.muxihuayi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jl.muxihuayi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://se.colortex.cn

[L06] 解析响应为 JSON
来源：http://ki.jianghongdianzi.cn

Py:   resp.json()
来源：http://io.huixinmuqiang.cn

PHP:  json_decode($body, true);
来源：http://ia.muxihuayi.cn

JS:   await resp.json()
来源：http://lb.9csxet.cn

TS:   await resp.json()
来源：http://lp.szsharing.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://eh.huanxung.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vh.haigaiapp.cn

Ruby: JSON.parse(resp.body)
来源：http://oa.newstarts.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ip.521024.cn

[L07] 处理 HTTP 状态码
来源：http://rl.bjjhwx.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dw.wgjwhj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://th.yuntaijiaju.cn

JS:   resp.ok;  resp.status
来源：http://pm.asd995.cn

TS:   resp.ok;  resp.status
来源：http://ma.gzmigu.cn

Java: resp.statusCode()
来源：http://kx.haigaiapp.cn

Go:   resp.StatusCode
来源：http://bb.asd995.cn

Ruby: resp.code.to_i
来源：http://yd.shxzukj.cn

C#:   (int)resp.StatusCode
来源：http://gt.panjiajie.cn

[L08] 并发请求多个地址
来源：http://ni.shxzskj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vr.haigaiapp.cn

PHP:  curl_multi_init() 系列
来源：http://em.nicolike.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jq.newstarts.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vf.shtwfgs.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hl.szsharing.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nd.hnjuh.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lk.521024.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hy.wgjwhj.cn

================================================================================
来源：http://jb.lnxyls.cn

M. 命令行 / 进程 / 环境
来源：http://yo.shxzukj.cn

================================================================================
来源：http://jg.nszjky.cn

[M01] 读取命令行参数
来源：http://ko.nszjky.cn

Py:   sys.argv[1:]
来源：http://ph.muxihuayi.cn

PHP:  $argv;  $argc;
来源：http://oj.bookmarksfly.cn

JS:   process.argv.slice(2)
来源：http://ad.lnxyls.cn

TS:   process.argv.slice(2)
来源：http://vr.yuntaijiaju.cn

Java: args 数组（main 方法参数）
来源：http://fj.szsharing.cn

Go:   os.Args[1:]
来源：http://zi.szxytkj.cn

Ruby: ARGV
来源：http://nb.haigaiapp.cn

C#:   args 数组（Main 方法参数）
来源：http://yx.hnjuh.cn

[M02] 读取环境变量
来源：http://lh.huixiangedu.cn

Py:   os.environ.get("HOME")
来源：http://fx.jianghongdianzi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xw.nicolike.cn

JS:   process.env.HOME
来源：http://hh.nszjky.cn

TS:   process.env.HOME
来源：http://dp.colortex.cn

Java: System.getenv("HOME")
来源：http://zb.haigaiapp.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pc.newstarts.cn

Ruby: ENV["HOME"]
来源：http://zx.jianghongdianzi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ch.9csxet.cn

[M03] 执行外部命令
来源：http://jn.szxytkj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dt.yuntaijiaju.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wt.haigaiapp.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jo.bjjhwx.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zj.9csxet.cn


<!-- 参考信息 -->