代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://lk.yuntaijiaju.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rs.chemitech.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gx.yuexingan06.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tr.huanxung.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wb.huixiangedu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zc.asd995.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nb.jianghongdianzi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fi.hahajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://he.lnxyls.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bs.jctech888.com.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bh.shxzskj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yg.wgjwhj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sq.newstarts.cn

[I07] 忽略大小写与多行模式
来源：http://jx.huanxung.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zr.hahajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dw.panjiajie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://od.shxzukj.cn

TS:   /error/gim
来源：http://qi.521024.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xs.chemitech.net.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yc.nicolike.cn

Ruby: s.scan(/error/i)
来源：http://wi.shxzskj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dk.lnxyls.cn

[I08] 贪婪与非贪婪匹配
来源：http://fr.gzmigu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://le.521024.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qo.szxytkj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tb.szsharing.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ja.haigaiapp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://kj.huanxung.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://li.nicolike.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vn.asd995.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wj.huanxung.cn

================================================================================
来源：http://fz.hahajie.cn

J. 日期与时间
来源：http://bg.panjiajie.cn

================================================================================
来源：http://gh.jctech888.com.cn

[J01] 获取当前时间
来源：http://fn.hahajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://aj.yuntaijiaju.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kg.nicolike.cn

JS:   new Date();  Date.now()
来源：http://iz.muxihuayi.cn

TS:   new Date();  Date.now()
来源：http://fq.huixinmuqiang.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://is.nszjky.cn

Go:   time.Now()
来源：http://se.szsharing.cn

Ruby: Time.now
来源：http://ed.huanxung.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ts.jctech888.com.cn

[J02] 格式化输出
来源：http://bq.nicolike.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uv.huanxung.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ci.muxihuayi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lk.szxytkj.cn

TS:   d.toISOString()
来源：http://vt.jctech888.com.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kw.colortex.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lk.szxytkj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mo.shxzskj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ep.yuexingan06.cn

[J03] 字符串解析为日期
来源：http://le.lnxyls.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kd.huixinmuqiang.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xo.gzmigu.cn

JS:   new Date("2024-01-02")
来源：http://hf.panjiajie.cn

TS:   new Date("2024-01-02")
来源：http://sk.colortex.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fc.yuexingan06.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://me.yuexingan06.cn

Ruby: Date.parse("2024-01-02")
来源：http://gj.huixiangedu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zc.hahajie.cn

[J04] 时间戳与日期互转
来源：http://ya.panjiajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lf.huixiangedu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://or.shxzskj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jz.newstarts.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ls.panjiajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rw.hnjuh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sn.shxzskj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ye.panjiajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qs.newstarts.cn

[J05] 时间加减（加 7 天）
来源：http://im.shxzukj.cn

Py:   now + timedelta(days=7)
来源：http://nx.shxzukj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pn.shtwfgs.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ba.huixiangedu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wx.hnjuh.cn

Java: LocalDate.now().plusDays(7)
来源：http://dh.shxzskj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://oh.9csxet.cn

Ruby: Time.now + 7 * 86400
来源：http://bw.muxihuayi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vr.huixinmuqiang.cn

[J06] 计算两时间之差
来源：http://cg.jianghongdianzi.cn

Py:   (end - start).total_seconds()
来源：http://my.asd995.cn

PHP:  $end->diff($start)->days;
来源：http://bk.bjjhwx.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ee.jianghongdianzi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zm.bookmarksfly.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ba.muxihuayi.cn

Go:   end.Sub(start).Hours()
来源：http://zv.yuexingan06.cn

Ruby: end - start                 # 返回秒数
来源：http://fc.shtwfgs.cn

C#:   (end - start).TotalSeconds
来源：http://tw.colortex.cn

[J07] 比较两个日期
来源：http://af.panjiajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://sp.huixiangedu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ag.bookmarksfly.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gi.nszjky.cn

TS:   d1.getTime() < d2.getTime()
来源：http://nf.nszjky.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ep.bjjhwx.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jk.521024.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ix.hnjuh.cn

C#:   d1 < d2;  d1 == d2
来源：http://sc.colortex.cn

[J08] 提取年月日与星期
来源：http://es.newstarts.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://is.jianghongdianzi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zk.9csxet.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yi.shxzskj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ff.lnxyls.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hb.shxzukj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://da.chemitech.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qb.bookmarksfly.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zj.shxzskj.cn

[J09] 时区处理
来源：http://bu.nicolike.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ez.hnjuh.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cs.szxytkj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kn.szxytkj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sa.newstarts.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ye.chemitech.net.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zr.shxzskj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wx.wgjwhj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jv.szsharing.cn

[J10] 取今天 / 本月第一天
来源：http://vy.huixinmuqiang.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://uq.panjiajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://br.panjiajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gf.chemitech.net.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yh.gzmigu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kh.hahajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pj.521024.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://to.hnjuh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hd.huixiangedu.cn

================================================================================
来源：http://zn.haigaiapp.cn

K. JSON 与序列化
来源：http://wb.gzmigu.cn

================================================================================
来源：http://uw.bjjhwx.cn

[K01] 对象转 JSON 字符串
来源：http://hm.nszjky.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vo.521024.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wh.wgjwhj.cn

JS:   JSON.stringify(obj)
来源：http://wj.hahajie.cn

TS:   JSON.stringify(obj)
来源：http://px.jctech888.com.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xa.colortex.cn

Go:   json.Marshal(obj)
来源：http://kc.asd995.cn

Ruby: obj.to_json                                     // require "json"
来源：http://eg.asd995.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://js.huanxung.cn

[K02] JSON 字符串转对象
来源：http://xe.haigaiapp.cn

Py:   json.loads(s)
来源：http://xj.yuexingan06.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jz.szxytkj.cn

JS:   JSON.parse(s)
来源：http://fu.muxihuayi.cn

TS:   JSON.parse(s)
来源：http://va.hnjuh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hu.huixiangedu.cn

Go:   json.Unmarshal(data, &v)
来源：http://gh.bjjhwx.cn

Ruby: JSON.parse(s)
来源：http://wf.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sx.huixiangedu.cn

[K03] JSON 美化输出（带缩进）
来源：http://mt.jianghongdianzi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://od.yuexingan06.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xn.huanxung.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jy.wgjwhj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://lz.nszjky.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yo.shtwfgs.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zi.yuntaijiaju.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qt.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pw.shxzukj.cn

[K04] 读取 JSON 文件
来源：http://cs.muxihuayi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sz.shtwfgs.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iv.hahajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://re.panjiajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://da.huanxung.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ib.shxzukj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mc.shxzukj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ut.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://by.lnxyls.cn

[K05] 深拷贝对象
来源：http://nw.szsharing.cn

Py:   copy.deepcopy(obj)
来源：http://bq.jctech888.com.cn

PHP:  unserialize(serialize($obj));
来源：http://ab.bjjhwx.cn

JS:   structuredClone(obj)
来源：http://yf.gzmigu.cn

TS:   structuredClone(obj)
来源：http://zr.nicolike.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://oc.colortex.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ii.nszjky.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ee.gzmigu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://uz.lnxyls.cn

[K06] 解析 URL 查询串
来源：http://pa.hahajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dj.shxzukj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vf.lnxyls.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mr.bjjhwx.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yi.nszjky.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://du.hnjuh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ti.bookmarksfly.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uj.haigaiapp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jm.hnjuh.cn

[K07] 进制转换
来源：http://mx.yuexingan06.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ly.szxytkj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hu.chemitech.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zn.bookmarksfly.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://go.nszjky.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wi.chemitech.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ma.nicolike.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xl.hahajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ku.hnjuh.cn

[K08] 二进制序列化（非 JSON）
来源：http://nk.521024.cn

Py:   pickle.dumps(obj)
来源：http://hw.yuntaijiaju.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://js.muxihuayi.cn

JS:   v8.serialize(obj)        // Node
来源：http://jj.gzmigu.cn

TS:   v8.serialize(obj)        // Node
来源：http://pn.lnxyls.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bq.colortex.cn

Go:   encoding/gob
来源：http://gw.gzmigu.cn

Ruby: Marshal.dump(obj)
来源：http://rq.haigaiapp.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fn.asd995.cn

================================================================================
来源：http://fl.szsharing.cn

L. 网络请求
来源：http://vp.gzmigu.cn

================================================================================
来源：http://jf.shtwfgs.cn

[L01] 发送 GET 请求
来源：http://vt.muxihuayi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ki.shtwfgs.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://he.huanxung.cn

JS:   await fetch(url)
来源：http://bm.szxytkj.cn

TS:   await fetch(url)
来源：http://nu.yuexingan06.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sq.asd995.cn

Go:   resp, err := http.Get(url)
来源：http://fb.9csxet.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gy.lnxyls.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bz.shxzukj.cn

[L02] 发送 POST JSON
来源：http://ja.shxzukj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cj.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rr.jianghongdianzi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jh.gzmigu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sy.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xp.muxihuayi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://as.shtwfgs.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ic.shxzskj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vy.chemitech.net.cn

[L03] 设置自定义请求头
来源：http://jo.shtwfgs.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fn.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jd.yuexingan06.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ff.asd995.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zp.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gn.bookmarksfly.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://oz.gzmigu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fa.huixinmuqiang.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bv.asd995.cn

[L04] 设置超时
来源：http://po.panjiajie.cn

Py:   requests.get(url, timeout=5)
来源：http://wc.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lp.haigaiapp.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pb.lnxyls.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mq.colortex.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gy.nszjky.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ch.haigaiapp.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tt.jctech888.com.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tm.gzmigu.cn

[L05] 上传文件（multipart）
来源：http://lf.muxihuayi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pc.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uw.muxihuayi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://be.lnxyls.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dp.yuexingan06.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qh.szsharing.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ys.wgjwhj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wa.colortex.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ts.wgjwhj.cn

[L06] 解析响应为 JSON
来源：http://ec.huanxung.cn

Py:   resp.json()
来源：http://jk.jctech888.com.cn

PHP:  json_decode($body, true);
来源：http://iv.huixiangedu.cn

JS:   await resp.json()
来源：http://zz.huanxung.cn

TS:   await resp.json()
来源：http://zo.huixinmuqiang.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tv.hnjuh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hg.colortex.cn

Ruby: JSON.parse(resp.body)
来源：http://nv.szsharing.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gy.nicolike.cn

[L07] 处理 HTTP 状态码
来源：http://cl.asd995.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ve.shtwfgs.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sc.yuntaijiaju.cn

JS:   resp.ok;  resp.status
来源：http://td.shtwfgs.cn

TS:   resp.ok;  resp.status
来源：http://eg.chemitech.net.cn

Java: resp.statusCode()
来源：http://tk.shxzskj.cn

Go:   resp.StatusCode
来源：http://rg.haigaiapp.cn

Ruby: resp.code.to_i
来源：http://ma.yuntaijiaju.cn

C#:   (int)resp.StatusCode
来源：http://nb.huixiangedu.cn

[L08] 并发请求多个地址
来源：http://ai.yuntaijiaju.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jo.gzmigu.cn

PHP:  curl_multi_init() 系列
来源：http://kb.shxzukj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hn.gzmigu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hq.szxytkj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lq.nszjky.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://on.szsharing.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kk.shxzukj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xj.nszjky.cn

================================================================================
来源：http://ze.haigaiapp.cn

M. 命令行 / 进程 / 环境
来源：http://cr.bookmarksfly.cn

================================================================================
来源：http://iz.chemitech.net.cn

[M01] 读取命令行参数
来源：http://vo.nszjky.cn

Py:   sys.argv[1:]
来源：http://qh.bjjhwx.cn

PHP:  $argv;  $argc;
来源：http://qp.yuexingan06.cn

JS:   process.argv.slice(2)
来源：http://hn.yuntaijiaju.cn

TS:   process.argv.slice(2)
来源：http://mp.asd995.cn

Java: args 数组（main 方法参数）
来源：http://pt.szxytkj.cn

Go:   os.Args[1:]
来源：http://zd.haigaiapp.cn

Ruby: ARGV
来源：http://hy.huanxung.cn

C#:   args 数组（Main 方法参数）
来源：http://jo.muxihuayi.cn

[M02] 读取环境变量
来源：http://kj.jctech888.com.cn

Py:   os.environ.get("HOME")
来源：http://hc.bjjhwx.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ad.hahajie.cn

JS:   process.env.HOME
来源：http://vv.asd995.cn

TS:   process.env.HOME
来源：http://pu.nicolike.cn

Java: System.getenv("HOME")
来源：http://lo.hahajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gm.bookmarksfly.cn

Ruby: ENV["HOME"]
来源：http://in.lnxyls.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oc.lnxyls.cn

[M03] 执行外部命令
来源：http://xg.jianghongdianzi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uz.szsharing.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://us.chemitech.net.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://mf.521024.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://df.yuntaijiaju.cn


<!-- 参考信息 -->