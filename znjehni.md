代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://mt.panjiajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xt.szsharing.cn

JS:   s.split(/\s*,\s*/)
来源：http://sw.haigaiapp.cn

TS:   s.split(/\s*,\s*/)
来源：http://ok.huixiangedu.cn

Java: s.split("\\s*,\\s*")
来源：http://zb.shtwfgs.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://no.521024.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qc.lnxyls.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vz.szsharing.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ns.shxzskj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jp.huanxung.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gk.szxytkj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ay.huixiangedu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nq.bookmarksfly.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cv.nicolike.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ck.shxzukj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mw.asd995.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://to.huanxung.cn

[I07] 忽略大小写与多行模式
来源：http://bd.szxytkj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vc.yuexingan06.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cl.szsharing.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://be.panjiajie.cn

TS:   /error/gim
来源：http://ej.nicolike.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hf.hnjuh.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mc.nicolike.cn

Ruby: s.scan(/error/i)
来源：http://at.shtwfgs.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mc.huixinmuqiang.cn

[I08] 贪婪与非贪婪匹配
来源：http://ej.shxzukj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jl.shxzskj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lc.yuexingan06.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mc.muxihuayi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rv.jianghongdianzi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zu.bookmarksfly.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://or.szsharing.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gp.muxihuayi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xh.nszjky.cn

================================================================================
来源：http://mt.hnjuh.cn

J. 日期与时间
来源：http://hz.szxytkj.cn

================================================================================
来源：http://hd.colortex.cn

[J01] 获取当前时间
来源：http://lh.hahajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://dk.bjjhwx.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xz.szsharing.cn

JS:   new Date();  Date.now()
来源：http://fn.bjjhwx.cn

TS:   new Date();  Date.now()
来源：http://wk.hnjuh.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://bv.521024.cn

Go:   time.Now()
来源：http://lt.jctech888.com.cn

Ruby: Time.now
来源：http://fc.asd995.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hh.wgjwhj.cn

[J02] 格式化输出
来源：http://gv.shtwfgs.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zl.szsharing.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hk.haigaiapp.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gk.shtwfgs.cn

TS:   d.toISOString()
来源：http://ro.colortex.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mu.huixinmuqiang.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kv.haigaiapp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hn.nszjky.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wg.bookmarksfly.cn

[J03] 字符串解析为日期
来源：http://yw.hnjuh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vf.bjjhwx.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://id.newstarts.cn

JS:   new Date("2024-01-02")
来源：http://gq.huanxung.cn

TS:   new Date("2024-01-02")
来源：http://fn.asd995.cn

Java: LocalDate.parse("2024-01-02")
来源：http://yk.shtwfgs.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zi.bookmarksfly.cn

Ruby: Date.parse("2024-01-02")
来源：http://ux.szxytkj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hs.haigaiapp.cn

[J04] 时间戳与日期互转
来源：http://mg.jianghongdianzi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ji.colortex.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zn.yuexingan06.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dy.bjjhwx.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qe.shxzukj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hb.newstarts.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://de.hnjuh.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ii.gzmigu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ir.wgjwhj.cn

[J05] 时间加减（加 7 天）
来源：http://hq.asd995.cn

Py:   now + timedelta(days=7)
来源：http://vp.wgjwhj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xr.521024.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kg.shxzskj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jh.haigaiapp.cn

Java: LocalDate.now().plusDays(7)
来源：http://jg.huixinmuqiang.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ct.panjiajie.cn

Ruby: Time.now + 7 * 86400
来源：http://ye.huixinmuqiang.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kh.huixinmuqiang.cn

[J06] 计算两时间之差
来源：http://uh.huixinmuqiang.cn

Py:   (end - start).total_seconds()
来源：http://ob.huixinmuqiang.cn

PHP:  $end->diff($start)->days;
来源：http://zj.521024.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jx.521024.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wi.hnjuh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ae.shxzskj.cn

Go:   end.Sub(start).Hours()
来源：http://fc.shtwfgs.cn

Ruby: end - start                 # 返回秒数
来源：http://yf.9csxet.cn

C#:   (end - start).TotalSeconds
来源：http://mx.hnjuh.cn

[J07] 比较两个日期
来源：http://ar.jianghongdianzi.cn

Py:   d1 < d2;  d1 == d2
来源：http://ni.chemitech.net.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hg.shtwfgs.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fc.szxytkj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://cp.shxzukj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yx.newstarts.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ii.newstarts.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cp.huixinmuqiang.cn

C#:   d1 < d2;  d1 == d2
来源：http://mf.wgjwhj.cn

[J08] 提取年月日与星期
来源：http://wg.yuexingan06.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://py.haigaiapp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://si.muxihuayi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zg.szxytkj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qk.jctech888.com.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://je.huixiangedu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qf.szsharing.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qw.hnjuh.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lt.szxytkj.cn

[J09] 时区处理
来源：http://ok.hahajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://og.jianghongdianzi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bn.jctech888.com.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://in.szsharing.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jr.huixiangedu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zp.asd995.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nw.shtwfgs.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cc.huixiangedu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cl.jianghongdianzi.cn

[J10] 取今天 / 本月第一天
来源：http://cv.nicolike.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://mn.asd995.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dj.521024.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wj.szxytkj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://la.hahajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gy.szxytkj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jr.shtwfgs.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kn.wgjwhj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oc.chemitech.net.cn

================================================================================
来源：http://ij.jianghongdianzi.cn

K. JSON 与序列化
来源：http://fv.hnjuh.cn

================================================================================
来源：http://hv.newstarts.cn

[K01] 对象转 JSON 字符串
来源：http://yc.muxihuayi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bp.hnjuh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hv.hahajie.cn

JS:   JSON.stringify(obj)
来源：http://ai.shtwfgs.cn

TS:   JSON.stringify(obj)
来源：http://zg.asd995.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fz.chemitech.net.cn

Go:   json.Marshal(obj)
来源：http://ta.newstarts.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ig.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vq.shtwfgs.cn

[K02] JSON 字符串转对象
来源：http://wv.colortex.cn

Py:   json.loads(s)
来源：http://bo.wgjwhj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vy.shtwfgs.cn

JS:   JSON.parse(s)
来源：http://om.gzmigu.cn

TS:   JSON.parse(s)
来源：http://ih.bjjhwx.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nu.asd995.cn

Go:   json.Unmarshal(data, &v)
来源：http://wv.asd995.cn

Ruby: JSON.parse(s)
来源：http://wa.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ch.shxzukj.cn

[K03] JSON 美化输出（带缩进）
来源：http://zo.huixiangedu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wl.shxzukj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fg.gzmigu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://cl.muxihuayi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gl.nicolike.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://aj.haigaiapp.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lf.bookmarksfly.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wz.shxzukj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rg.colortex.cn

[K04] 读取 JSON 文件
来源：http://ts.colortex.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ir.szsharing.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zg.jianghongdianzi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xy.shtwfgs.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gd.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ja.newstarts.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zq.muxihuayi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vh.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rq.hahajie.cn

[K05] 深拷贝对象
来源：http://gf.hahajie.cn

Py:   copy.deepcopy(obj)
来源：http://jm.asd995.cn

PHP:  unserialize(serialize($obj));
来源：http://qn.asd995.cn

JS:   structuredClone(obj)
来源：http://ku.jctech888.com.cn

TS:   structuredClone(obj)
来源：http://cv.521024.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://oz.colortex.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qw.newstarts.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://iw.521024.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://af.hahajie.cn

[K06] 解析 URL 查询串
来源：http://lj.9csxet.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ht.521024.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kl.jianghongdianzi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xb.panjiajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zi.521024.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rj.asd995.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vx.nszjky.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ml.jctech888.com.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fi.jctech888.com.cn

[K07] 进制转换
来源：http://ic.521024.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mh.jctech888.com.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vp.huixinmuqiang.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ft.gzmigu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dp.huanxung.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rk.huixiangedu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gl.colortex.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qi.bookmarksfly.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bf.521024.cn

[K08] 二进制序列化（非 JSON）
来源：http://og.newstarts.cn

Py:   pickle.dumps(obj)
来源：http://wp.9csxet.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cs.jianghongdianzi.cn

JS:   v8.serialize(obj)        // Node
来源：http://cr.shxzskj.cn

TS:   v8.serialize(obj)        // Node
来源：http://pr.shxzukj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://if.hahajie.cn

Go:   encoding/gob
来源：http://so.521024.cn

Ruby: Marshal.dump(obj)
来源：http://oh.bjjhwx.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qk.shxzukj.cn

================================================================================
来源：http://jp.lnxyls.cn

L. 网络请求
来源：http://cu.huixinmuqiang.cn

================================================================================
来源：http://wq.asd995.cn

[L01] 发送 GET 请求
来源：http://iy.wgjwhj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xv.shxzskj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sk.jianghongdianzi.cn

JS:   await fetch(url)
来源：http://sz.9csxet.cn

TS:   await fetch(url)
来源：http://zn.bookmarksfly.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://iz.haigaiapp.cn

Go:   resp, err := http.Get(url)
来源：http://lf.jianghongdianzi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://mp.szsharing.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hb.yuexingan06.cn

[L02] 发送 POST JSON
来源：http://ri.hahajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mm.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://io.shxzskj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zh.panjiajie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zi.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://en.shxzskj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://di.nicolike.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hm.bjjhwx.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gb.hahajie.cn

[L03] 设置自定义请求头
来源：http://oj.muxihuayi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vz.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gd.wgjwhj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ku.yuexingan06.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://no.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ab.szxytkj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gf.muxihuayi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lp.wgjwhj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dy.yuntaijiaju.cn

[L04] 设置超时
来源：http://zn.panjiajie.cn

Py:   requests.get(url, timeout=5)
来源：http://tc.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mc.9csxet.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yv.newstarts.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yi.szxytkj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cy.newstarts.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fu.chemitech.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dx.521024.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gy.jctech888.com.cn

[L05] 上传文件（multipart）
来源：http://cw.shxzukj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jm.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jh.chemitech.net.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://of.jctech888.com.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mn.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uc.shxzskj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yk.szsharing.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dp.521024.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lh.hahajie.cn

[L06] 解析响应为 JSON
来源：http://wb.jctech888.com.cn

Py:   resp.json()
来源：http://ox.gzmigu.cn

PHP:  json_decode($body, true);
来源：http://ma.asd995.cn

JS:   await resp.json()
来源：http://mz.newstarts.cn

TS:   await resp.json()
来源：http://wn.shtwfgs.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rz.huanxung.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ns.hnjuh.cn

Ruby: JSON.parse(resp.body)
来源：http://zw.panjiajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fn.nszjky.cn

[L07] 处理 HTTP 状态码
来源：http://kv.yuexingan06.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ov.nszjky.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://eh.lnxyls.cn

JS:   resp.ok;  resp.status
来源：http://ka.wgjwhj.cn

TS:   resp.ok;  resp.status
来源：http://ln.chemitech.net.cn

Java: resp.statusCode()
来源：http://js.hnjuh.cn

Go:   resp.StatusCode
来源：http://vr.hnjuh.cn

Ruby: resp.code.to_i
来源：http://mk.colortex.cn

C#:   (int)resp.StatusCode
来源：http://io.521024.cn

[L08] 并发请求多个地址
来源：http://ez.9csxet.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ty.shxzukj.cn

PHP:  curl_multi_init() 系列
来源：http://ql.shtwfgs.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bn.haigaiapp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yy.yuexingan06.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xp.chemitech.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gi.bookmarksfly.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vr.jctech888.com.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://oq.yuexingan06.cn

================================================================================
来源：http://sf.huixiangedu.cn

M. 命令行 / 进程 / 环境
来源：http://hu.shxzskj.cn

================================================================================
来源：http://oy.hnjuh.cn

[M01] 读取命令行参数
来源：http://zd.jianghongdianzi.cn

Py:   sys.argv[1:]
来源：http://xz.bookmarksfly.cn

PHP:  $argv;  $argc;
来源：http://nm.chemitech.net.cn

JS:   process.argv.slice(2)
来源：http://hk.nicolike.cn

TS:   process.argv.slice(2)
来源：http://al.wgjwhj.cn

Java: args 数组（main 方法参数）
来源：http://hf.nszjky.cn

Go:   os.Args[1:]
来源：http://hj.gzmigu.cn

Ruby: ARGV
来源：http://bt.haigaiapp.cn

C#:   args 数组（Main 方法参数）
来源：http://mc.huanxung.cn

[M02] 读取环境变量
来源：http://ly.szxytkj.cn

Py:   os.environ.get("HOME")
来源：http://so.yuntaijiaju.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bp.shtwfgs.cn

JS:   process.env.HOME
来源：http://nr.shxzukj.cn

TS:   process.env.HOME
来源：http://ay.huixinmuqiang.cn

Java: System.getenv("HOME")
来源：http://hi.yuexingan06.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ep.panjiajie.cn

Ruby: ENV["HOME"]
来源：http://uf.521024.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wi.521024.cn

[M03] 执行外部命令
来源：http://nq.chemitech.net.cn


<!-- 参考信息 -->