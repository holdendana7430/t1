代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://fk.jianghongdianzi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bb.shxzukj.cn

JS:   s.split(/\s*,\s*/)
来源：http://bs.panjiajie.cn

TS:   s.split(/\s*,\s*/)
来源：http://ix.bjjhwx.cn

Java: s.split("\\s*,\\s*")
来源：http://ad.newstarts.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kj.chemitech.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bb.asd995.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nm.shtwfgs.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sy.yuexingan06.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fb.huixinmuqiang.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lh.huanxung.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zu.muxihuayi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ow.shxzukj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zu.asd995.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jr.521024.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yj.yuexingan06.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hs.gzmigu.cn

[I07] 忽略大小写与多行模式
来源：http://ho.nicolike.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kj.huixinmuqiang.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://om.jianghongdianzi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://po.panjiajie.cn

TS:   /error/gim
来源：http://zc.bjjhwx.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tg.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fd.yuntaijiaju.cn

Ruby: s.scan(/error/i)
来源：http://hj.bookmarksfly.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ht.jianghongdianzi.cn

[I08] 贪婪与非贪婪匹配
来源：http://jp.haigaiapp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nf.bookmarksfly.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sh.haigaiapp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yo.szsharing.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hg.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nv.panjiajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xy.bjjhwx.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ir.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cc.lnxyls.cn

================================================================================
来源：http://tt.szxytkj.cn

J. 日期与时间
来源：http://zk.huanxung.cn

================================================================================
来源：http://za.haigaiapp.cn

[J01] 获取当前时间
来源：http://fo.bjjhwx.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://il.panjiajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gj.yuexingan06.cn

JS:   new Date();  Date.now()
来源：http://ew.hahajie.cn

TS:   new Date();  Date.now()
来源：http://cu.nicolike.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ti.yuntaijiaju.cn

Go:   time.Now()
来源：http://ml.huanxung.cn

Ruby: Time.now
来源：http://gf.lnxyls.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hj.muxihuayi.cn

[J02] 格式化输出
来源：http://hp.shxzukj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fl.shxzukj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sa.hnjuh.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tg.yuexingan06.cn

TS:   d.toISOString()
来源：http://xn.yuexingan06.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qz.hnjuh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ds.newstarts.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://da.huixiangedu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bh.bookmarksfly.cn

[J03] 字符串解析为日期
来源：http://ag.chemitech.net.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cp.bookmarksfly.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ug.szsharing.cn

JS:   new Date("2024-01-02")
来源：http://ck.newstarts.cn

TS:   new Date("2024-01-02")
来源：http://yp.huanxung.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rh.yuntaijiaju.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uz.yuexingan06.cn

Ruby: Date.parse("2024-01-02")
来源：http://kh.huixiangedu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yo.bjjhwx.cn

[J04] 时间戳与日期互转
来源：http://ed.newstarts.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ji.wgjwhj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ki.panjiajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ql.nicolike.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://rq.szsharing.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cb.shxzukj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hx.bjjhwx.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fc.asd995.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pl.jianghongdianzi.cn

[J05] 时间加减（加 7 天）
来源：http://pd.521024.cn

Py:   now + timedelta(days=7)
来源：http://ss.bjjhwx.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mj.hnjuh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xv.chemitech.net.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ip.chemitech.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://ms.wgjwhj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bk.hahajie.cn

Ruby: Time.now + 7 * 86400
来源：http://bw.521024.cn

C#:   DateTime.Now.AddDays(7)
来源：http://sk.jctech888.com.cn

[J06] 计算两时间之差
来源：http://qt.huixinmuqiang.cn

Py:   (end - start).total_seconds()
来源：http://fo.panjiajie.cn

PHP:  $end->diff($start)->days;
来源：http://jh.gzmigu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yi.wgjwhj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gz.bjjhwx.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fa.asd995.cn

Go:   end.Sub(start).Hours()
来源：http://lr.colortex.cn

Ruby: end - start                 # 返回秒数
来源：http://as.nicolike.cn

C#:   (end - start).TotalSeconds
来源：http://hu.hnjuh.cn

[J07] 比较两个日期
来源：http://yb.521024.cn

Py:   d1 < d2;  d1 == d2
来源：http://kx.colortex.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cb.colortex.cn

JS:   d1.getTime() < d2.getTime()
来源：http://dy.wgjwhj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mh.newstarts.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://od.huanxung.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jn.asd995.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kl.nszjky.cn

C#:   d1 < d2;  d1 == d2
来源：http://yi.nszjky.cn

[J08] 提取年月日与星期
来源：http://pg.huanxung.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sg.szxytkj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gf.asd995.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://at.wgjwhj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ib.yuexingan06.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mh.shxzskj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xh.gzmigu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yo.chemitech.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ty.haigaiapp.cn

[J09] 时区处理
来源：http://dh.muxihuayi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wh.asd995.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dm.jianghongdianzi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mo.shxzukj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wb.521024.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qa.521024.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sj.jctech888.com.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yf.hnjuh.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fk.szxytkj.cn

[J10] 取今天 / 本月第一天
来源：http://ce.yuexingan06.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://pf.shxzskj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://oy.haigaiapp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://oq.huixiangedu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rt.hnjuh.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://te.hnjuh.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yn.jianghongdianzi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sp.jctech888.com.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cv.9csxet.cn

================================================================================
来源：http://vr.bjjhwx.cn

K. JSON 与序列化
来源：http://ml.nicolike.cn

================================================================================
来源：http://fs.lnxyls.cn

[K01] 对象转 JSON 字符串
来源：http://ca.szxytkj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://py.9csxet.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wn.lnxyls.cn

JS:   JSON.stringify(obj)
来源：http://gx.yuexingan06.cn

TS:   JSON.stringify(obj)
来源：http://la.colortex.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wq.nszjky.cn

Go:   json.Marshal(obj)
来源：http://ki.hahajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ja.szxytkj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bt.chemitech.net.cn

[K02] JSON 字符串转对象
来源：http://zs.muxihuayi.cn

Py:   json.loads(s)
来源：http://of.shxzukj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ji.9csxet.cn

JS:   JSON.parse(s)
来源：http://io.lnxyls.cn

TS:   JSON.parse(s)
来源：http://hv.asd995.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pg.shxzukj.cn

Go:   json.Unmarshal(data, &v)
来源：http://wz.szsharing.cn

Ruby: JSON.parse(s)
来源：http://ov.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yn.hnjuh.cn

[K03] JSON 美化输出（带缩进）
来源：http://ir.nicolike.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xy.521024.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pz.wgjwhj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://on.szsharing.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://er.huanxung.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uh.lnxyls.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ly.panjiajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://my.asd995.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bv.shtwfgs.cn

[K04] 读取 JSON 文件
来源：http://tf.lnxyls.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yq.jctech888.com.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://il.gzmigu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://er.panjiajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ht.jctech888.com.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ew.hahajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ae.shtwfgs.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dc.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jq.jianghongdianzi.cn

[K05] 深拷贝对象
来源：http://gd.521024.cn

Py:   copy.deepcopy(obj)
来源：http://rg.lnxyls.cn

PHP:  unserialize(serialize($obj));
来源：http://uh.chemitech.net.cn

JS:   structuredClone(obj)
来源：http://rf.nszjky.cn

TS:   structuredClone(obj)
来源：http://js.yuntaijiaju.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jc.jianghongdianzi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dz.colortex.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://eq.wgjwhj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://if.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://aq.szsharing.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fj.colortex.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xv.nicolike.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qy.szsharing.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://de.bjjhwx.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bx.yuntaijiaju.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zo.colortex.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uh.newstarts.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mh.huixiangedu.cn

[K07] 进制转换
来源：http://hc.jctech888.com.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yy.shxzskj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cs.lnxyls.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xl.szxytkj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hj.bookmarksfly.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sj.bookmarksfly.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nr.yuexingan06.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gh.bookmarksfly.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ae.asd995.cn

[K08] 二进制序列化（非 JSON）
来源：http://lg.jctech888.com.cn

Py:   pickle.dumps(obj)
来源：http://ij.521024.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fd.panjiajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://yn.haigaiapp.cn

TS:   v8.serialize(obj)        // Node
来源：http://vh.9csxet.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ry.szsharing.cn

Go:   encoding/gob
来源：http://ow.szsharing.cn

Ruby: Marshal.dump(obj)
来源：http://cn.bjjhwx.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wd.asd995.cn

================================================================================
来源：http://qw.jianghongdianzi.cn

L. 网络请求
来源：http://yy.huanxung.cn

================================================================================
来源：http://te.bookmarksfly.cn

[L01] 发送 GET 请求
来源：http://zs.nszjky.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zq.nszjky.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lx.shtwfgs.cn

JS:   await fetch(url)
来源：http://vk.newstarts.cn

TS:   await fetch(url)
来源：http://fd.asd995.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ms.panjiajie.cn

Go:   resp, err := http.Get(url)
来源：http://xj.9csxet.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rv.muxihuayi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tg.shxzukj.cn

[L02] 发送 POST JSON
来源：http://vq.chemitech.net.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qb.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wh.shtwfgs.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ff.lnxyls.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kk.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ad.huixiangedu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bw.newstarts.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sx.huanxung.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pq.chemitech.net.cn

[L03] 设置自定义请求头
来源：http://vg.huixinmuqiang.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ie.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://za.muxihuayi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gn.nszjky.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vx.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bu.yuntaijiaju.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ju.panjiajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sk.huixiangedu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ai.shxzukj.cn

[L04] 设置超时
来源：http://sl.shtwfgs.cn

Py:   requests.get(url, timeout=5)
来源：http://no.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://te.haigaiapp.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ps.9csxet.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://li.hnjuh.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://he.hnjuh.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sg.bookmarksfly.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nv.huanxung.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rg.yuexingan06.cn

[L05] 上传文件（multipart）
来源：http://jh.haigaiapp.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pf.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bt.nicolike.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fu.yuntaijiaju.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xp.colortex.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vk.szxytkj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ur.bookmarksfly.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mo.newstarts.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wp.9csxet.cn

[L06] 解析响应为 JSON
来源：http://ke.hnjuh.cn

Py:   resp.json()
来源：http://no.nicolike.cn

PHP:  json_decode($body, true);
来源：http://ao.9csxet.cn

JS:   await resp.json()
来源：http://py.bjjhwx.cn

TS:   await resp.json()
来源：http://bj.asd995.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mh.chemitech.net.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rr.nicolike.cn

Ruby: JSON.parse(resp.body)
来源：http://vw.panjiajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fy.hahajie.cn

[L07] 处理 HTTP 状态码
来源：http://nz.szxytkj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cy.jianghongdianzi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bo.shxzskj.cn

JS:   resp.ok;  resp.status
来源：http://lw.shxzukj.cn

TS:   resp.ok;  resp.status
来源：http://gx.szxytkj.cn

Java: resp.statusCode()
来源：http://ms.yuntaijiaju.cn

Go:   resp.StatusCode
来源：http://nq.nicolike.cn

Ruby: resp.code.to_i
来源：http://qt.huixinmuqiang.cn

C#:   (int)resp.StatusCode
来源：http://rc.wgjwhj.cn

[L08] 并发请求多个地址
来源：http://rg.lnxyls.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jq.asd995.cn

PHP:  curl_multi_init() 系列
来源：http://so.jctech888.com.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ut.nszjky.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rv.hnjuh.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://do.lnxyls.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nt.nszjky.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hr.yuexingan06.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uq.colortex.cn

================================================================================
来源：http://wz.huixinmuqiang.cn

M. 命令行 / 进程 / 环境
来源：http://gx.lnxyls.cn

================================================================================
来源：http://uo.chemitech.net.cn

[M01] 读取命令行参数
来源：http://dz.huanxung.cn

Py:   sys.argv[1:]
来源：http://bg.szsharing.cn

PHP:  $argv;  $argc;
来源：http://ar.huanxung.cn

JS:   process.argv.slice(2)
来源：http://br.huanxung.cn

TS:   process.argv.slice(2)
来源：http://yh.yuntaijiaju.cn

Java: args 数组（main 方法参数）
来源：http://bz.huixinmuqiang.cn

Go:   os.Args[1:]
来源：http://kt.chemitech.net.cn

Ruby: ARGV
来源：http://fg.jianghongdianzi.cn

C#:   args 数组（Main 方法参数）
来源：http://yl.huanxung.cn

[M02] 读取环境变量
来源：http://do.shtwfgs.cn

Py:   os.environ.get("HOME")
来源：http://uz.chemitech.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mu.shtwfgs.cn

JS:   process.env.HOME
来源：http://ss.nicolike.cn

TS:   process.env.HOME
来源：http://zm.huixinmuqiang.cn

Java: System.getenv("HOME")
来源：http://yx.szxytkj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://le.9csxet.cn

Ruby: ENV["HOME"]
来源：http://se.asd995.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wh.lnxyls.cn

[M03] 执行外部命令
来源：http://us.huixinmuqiang.cn


<!-- 参考信息 -->