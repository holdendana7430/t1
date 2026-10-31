代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://nv.shtwfgs.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lb.shtwfgs.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vk.szsharing.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hs.521024.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qn.panjiajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pv.wgjwhj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ay.shxzskj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ys.chemitech.net.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fp.muxihuayi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lr.yuexingan06.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zl.bookmarksfly.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bk.huixinmuqiang.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dq.muxihuayi.cn

[I07] 忽略大小写与多行模式
来源：http://te.hnjuh.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fl.huixiangedu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ps.bookmarksfly.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ha.gzmigu.cn

TS:   /error/gim
来源：http://bg.jctech888.com.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nq.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vr.newstarts.cn

Ruby: s.scan(/error/i)
来源：http://fc.haigaiapp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://af.huixinmuqiang.cn

[I08] 贪婪与非贪婪匹配
来源：http://sy.yuexingan06.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ad.nszjky.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ef.huixinmuqiang.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ne.jctech888.com.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xf.haigaiapp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vy.lnxyls.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hf.gzmigu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tn.nszjky.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xj.lnxyls.cn

================================================================================
来源：http://fs.newstarts.cn

J. 日期与时间
来源：http://zn.lnxyls.cn

================================================================================
来源：http://rj.bjjhwx.cn

[J01] 获取当前时间
来源：http://yo.shtwfgs.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://oe.bookmarksfly.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mp.szsharing.cn

JS:   new Date();  Date.now()
来源：http://fi.gzmigu.cn

TS:   new Date();  Date.now()
来源：http://tb.hnjuh.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mi.wgjwhj.cn

Go:   time.Now()
来源：http://hb.hahajie.cn

Ruby: Time.now
来源：http://fk.shxzukj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xz.jianghongdianzi.cn

[J02] 格式化输出
来源：http://zu.hahajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://az.colortex.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://am.szxytkj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ii.bookmarksfly.cn

TS:   d.toISOString()
来源：http://jz.nicolike.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ye.gzmigu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ia.jianghongdianzi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uz.wgjwhj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gs.haigaiapp.cn

[J03] 字符串解析为日期
来源：http://jw.hnjuh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ee.shtwfgs.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mj.yuntaijiaju.cn

JS:   new Date("2024-01-02")
来源：http://bc.yuexingan06.cn

TS:   new Date("2024-01-02")
来源：http://iz.hnjuh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rb.jianghongdianzi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ys.yuntaijiaju.cn

Ruby: Date.parse("2024-01-02")
来源：http://zo.jianghongdianzi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jg.shtwfgs.cn

[J04] 时间戳与日期互转
来源：http://kf.shxzskj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kw.lnxyls.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qj.jianghongdianzi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://la.hnjuh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://es.chemitech.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lh.asd995.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cq.panjiajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ht.bookmarksfly.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bj.chemitech.net.cn

[J05] 时间加减（加 7 天）
来源：http://pm.gzmigu.cn

Py:   now + timedelta(days=7)
来源：http://ux.hahajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://oa.wgjwhj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://io.newstarts.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cp.chemitech.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://bx.haigaiapp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nx.muxihuayi.cn

Ruby: Time.now + 7 * 86400
来源：http://mm.huixinmuqiang.cn

C#:   DateTime.Now.AddDays(7)
来源：http://la.9csxet.cn

[J06] 计算两时间之差
来源：http://sf.nszjky.cn

Py:   (end - start).total_seconds()
来源：http://hh.huanxung.cn

PHP:  $end->diff($start)->days;
来源：http://pu.jctech888.com.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hj.shxzskj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ax.shtwfgs.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zb.huixiangedu.cn

Go:   end.Sub(start).Hours()
来源：http://yt.yuntaijiaju.cn

Ruby: end - start                 # 返回秒数
来源：http://ij.hahajie.cn

C#:   (end - start).TotalSeconds
来源：http://mi.huixinmuqiang.cn

[J07] 比较两个日期
来源：http://af.nicolike.cn

Py:   d1 < d2;  d1 == d2
来源：http://zk.gzmigu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mv.lnxyls.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vj.521024.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ek.gzmigu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ww.huixiangedu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jt.szxytkj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kg.jianghongdianzi.cn

C#:   d1 < d2;  d1 == d2
来源：http://qz.bjjhwx.cn

[J08] 提取年月日与星期
来源：http://rs.521024.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://et.shtwfgs.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://np.yuexingan06.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ap.huanxung.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ih.panjiajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://og.lnxyls.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lx.yuexingan06.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ji.9csxet.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mv.szxytkj.cn

[J09] 时区处理
来源：http://kx.muxihuayi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wf.bjjhwx.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wh.chemitech.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tt.szsharing.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ml.lnxyls.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pd.asd995.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://aq.jianghongdianzi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://dc.panjiajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hk.jianghongdianzi.cn

[J10] 取今天 / 本月第一天
来源：http://hy.haigaiapp.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://le.lnxyls.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qr.nszjky.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vb.wgjwhj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qe.shxzukj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ui.gzmigu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yq.szsharing.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fu.szsharing.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jp.szsharing.cn

================================================================================
来源：http://on.haigaiapp.cn

K. JSON 与序列化
来源：http://yz.shtwfgs.cn

================================================================================
来源：http://nc.huixiangedu.cn

[K01] 对象转 JSON 字符串
来源：http://ak.asd995.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xy.asd995.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hf.yuntaijiaju.cn

JS:   JSON.stringify(obj)
来源：http://ui.haigaiapp.cn

TS:   JSON.stringify(obj)
来源：http://zb.nicolike.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qg.huanxung.cn

Go:   json.Marshal(obj)
来源：http://ik.bjjhwx.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ws.521024.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xf.panjiajie.cn

[K02] JSON 字符串转对象
来源：http://ej.colortex.cn

Py:   json.loads(s)
来源：http://ro.chemitech.net.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fc.huixiangedu.cn

JS:   JSON.parse(s)
来源：http://lf.newstarts.cn

TS:   JSON.parse(s)
来源：http://ty.yuntaijiaju.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mw.wgjwhj.cn

Go:   json.Unmarshal(data, &v)
来源：http://lo.colortex.cn

Ruby: JSON.parse(s)
来源：http://hn.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bs.lnxyls.cn

[K03] JSON 美化输出（带缩进）
来源：http://ct.hahajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hp.9csxet.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://el.wgjwhj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hv.asd995.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://lb.panjiajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ve.lnxyls.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ec.huixiangedu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ze.shxzukj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gk.9csxet.cn

[K04] 读取 JSON 文件
来源：http://dk.yuntaijiaju.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yh.jctech888.com.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://og.bookmarksfly.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ya.panjiajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wu.huanxung.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lp.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ar.wgjwhj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://eo.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ol.haigaiapp.cn

[K05] 深拷贝对象
来源：http://xv.wgjwhj.cn

Py:   copy.deepcopy(obj)
来源：http://sm.nicolike.cn

PHP:  unserialize(serialize($obj));
来源：http://qi.bjjhwx.cn

JS:   structuredClone(obj)
来源：http://ds.szxytkj.cn

TS:   structuredClone(obj)
来源：http://ym.newstarts.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://om.nicolike.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tv.521024.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ke.yuexingan06.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yy.nszjky.cn

[K06] 解析 URL 查询串
来源：http://fl.gzmigu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pc.szxytkj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ux.shtwfgs.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hy.szsharing.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cg.szsharing.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ku.lnxyls.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://lj.521024.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xu.nicolike.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kj.gzmigu.cn

[K07] 进制转换
来源：http://rp.bjjhwx.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xr.hnjuh.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ox.newstarts.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qq.gzmigu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xb.jctech888.com.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tr.shxzukj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ql.huixiangedu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kk.chemitech.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://as.jctech888.com.cn

[K08] 二进制序列化（非 JSON）
来源：http://bv.yuntaijiaju.cn

Py:   pickle.dumps(obj)
来源：http://no.szxytkj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bj.huixiangedu.cn

JS:   v8.serialize(obj)        // Node
来源：http://bc.yuexingan06.cn

TS:   v8.serialize(obj)        // Node
来源：http://yw.gzmigu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://il.nicolike.cn

Go:   encoding/gob
来源：http://gq.huixinmuqiang.cn

Ruby: Marshal.dump(obj)
来源：http://mw.gzmigu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jv.shxzskj.cn

================================================================================
来源：http://je.jianghongdianzi.cn

L. 网络请求
来源：http://im.asd995.cn

================================================================================
来源：http://vy.jianghongdianzi.cn

[L01] 发送 GET 请求
来源：http://js.gzmigu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kh.nicolike.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ze.yuexingan06.cn

JS:   await fetch(url)
来源：http://pt.shtwfgs.cn

TS:   await fetch(url)
来源：http://uo.newstarts.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dc.shtwfgs.cn

Go:   resp, err := http.Get(url)
来源：http://xl.chemitech.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gu.yuexingan06.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ou.hahajie.cn

[L02] 发送 POST JSON
来源：http://xd.chemitech.net.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pz.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bv.huixiangedu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pk.shtwfgs.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zq.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gs.lnxyls.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fd.newstarts.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lt.muxihuayi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xq.jianghongdianzi.cn

[L03] 设置自定义请求头
来源：http://je.bookmarksfly.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://or.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mp.lnxyls.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nc.panjiajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hs.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://df.9csxet.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://te.shxzskj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sd.shxzukj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fb.huixinmuqiang.cn

[L04] 设置超时
来源：http://lc.hahajie.cn

Py:   requests.get(url, timeout=5)
来源：http://lc.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qh.newstarts.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dg.lnxyls.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rt.yuexingan06.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dc.wgjwhj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://za.colortex.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wv.huanxung.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rl.panjiajie.cn

[L05] 上传文件（multipart）
来源：http://bo.lnxyls.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ia.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://is.colortex.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lr.jianghongdianzi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wg.521024.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://js.chemitech.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ib.bjjhwx.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zn.newstarts.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://eo.colortex.cn

[L06] 解析响应为 JSON
来源：http://qh.szsharing.cn

Py:   resp.json()
来源：http://dh.shxzskj.cn

PHP:  json_decode($body, true);
来源：http://tv.jctech888.com.cn

JS:   await resp.json()
来源：http://kw.shxzskj.cn

TS:   await resp.json()
来源：http://ho.panjiajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ra.huixinmuqiang.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bi.wgjwhj.cn

Ruby: JSON.parse(resp.body)
来源：http://ji.bookmarksfly.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zn.wgjwhj.cn

[L07] 处理 HTTP 状态码
来源：http://ts.haigaiapp.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nn.huixinmuqiang.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mf.haigaiapp.cn

JS:   resp.ok;  resp.status
来源：http://ul.yuntaijiaju.cn

TS:   resp.ok;  resp.status
来源：http://ii.colortex.cn

Java: resp.statusCode()
来源：http://no.huixinmuqiang.cn

Go:   resp.StatusCode
来源：http://pl.jianghongdianzi.cn

Ruby: resp.code.to_i
来源：http://ky.szxytkj.cn

C#:   (int)resp.StatusCode
来源：http://eb.chemitech.net.cn

[L08] 并发请求多个地址
来源：http://jl.chemitech.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rc.shtwfgs.cn

PHP:  curl_multi_init() 系列
来源：http://bw.hnjuh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xg.haigaiapp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://so.hahajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qo.bjjhwx.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vd.shxzskj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fb.521024.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bv.shtwfgs.cn

================================================================================
来源：http://dv.yuntaijiaju.cn

M. 命令行 / 进程 / 环境
来源：http://ae.muxihuayi.cn

================================================================================
来源：http://fz.szsharing.cn

[M01] 读取命令行参数
来源：http://yd.hahajie.cn

Py:   sys.argv[1:]
来源：http://tc.bjjhwx.cn

PHP:  $argv;  $argc;
来源：http://es.hnjuh.cn

JS:   process.argv.slice(2)
来源：http://ba.colortex.cn

TS:   process.argv.slice(2)
来源：http://ez.szxytkj.cn

Java: args 数组（main 方法参数）
来源：http://ia.huixinmuqiang.cn

Go:   os.Args[1:]
来源：http://ip.9csxet.cn

Ruby: ARGV
来源：http://gp.colortex.cn

C#:   args 数组（Main 方法参数）
来源：http://wc.yuntaijiaju.cn

[M02] 读取环境变量
来源：http://ww.bjjhwx.cn

Py:   os.environ.get("HOME")
来源：http://ha.shxzskj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nl.9csxet.cn

JS:   process.env.HOME
来源：http://ie.colortex.cn

TS:   process.env.HOME
来源：http://vr.9csxet.cn

Java: System.getenv("HOME")
来源：http://xd.gzmigu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jj.9csxet.cn

Ruby: ENV["HOME"]
来源：http://xy.huixiangedu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bd.shxzskj.cn

[M03] 执行外部命令
来源：http://uj.jianghongdianzi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://sh.huixinmuqiang.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ui.nszjky.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hf.haigaiapp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pq.szsharing.cn


<!-- 参考信息 -->