代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sl.szxytkj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uz.shxzskj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yo.shxzukj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tq.gzmigu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rh.haigaiapp.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wj.szsharing.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mb.yuntaijiaju.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wq.jctech888.com.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://aj.yuexingan06.cn

[I07] 忽略大小写与多行模式
来源：http://qz.shxzukj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://be.bjjhwx.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lo.asd995.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://oy.gzmigu.cn

TS:   /error/gim
来源：http://yn.9csxet.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tn.huanxung.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mf.shxzskj.cn

Ruby: s.scan(/error/i)
来源：http://sf.huanxung.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jg.muxihuayi.cn

[I08] 贪婪与非贪婪匹配
来源：http://oy.jctech888.com.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bv.panjiajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dy.shtwfgs.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://es.yuexingan06.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vi.hnjuh.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://dr.nszjky.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ww.jctech888.com.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mq.hahajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ot.yuexingan06.cn

================================================================================
来源：http://or.muxihuayi.cn

J. 日期与时间
来源：http://zn.shxzukj.cn

================================================================================
来源：http://kk.lnxyls.cn

[J01] 获取当前时间
来源：http://bc.colortex.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ys.nicolike.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lj.9csxet.cn

JS:   new Date();  Date.now()
来源：http://wd.szsharing.cn

TS:   new Date();  Date.now()
来源：http://fn.szxytkj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://oc.nszjky.cn

Go:   time.Now()
来源：http://zy.huixinmuqiang.cn

Ruby: Time.now
来源：http://nb.szxytkj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wg.huixinmuqiang.cn

[J02] 格式化输出
来源：http://is.nicolike.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bi.gzmigu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zm.szsharing.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kn.shxzukj.cn

TS:   d.toISOString()
来源：http://tg.9csxet.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dx.hnjuh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jl.bjjhwx.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://up.muxihuayi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bj.jianghongdianzi.cn

[J03] 字符串解析为日期
来源：http://ko.bookmarksfly.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zq.haigaiapp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gj.asd995.cn

JS:   new Date("2024-01-02")
来源：http://ol.jctech888.com.cn

TS:   new Date("2024-01-02")
来源：http://mj.shxzskj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fg.colortex.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ox.shtwfgs.cn

Ruby: Date.parse("2024-01-02")
来源：http://yr.wgjwhj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sk.jctech888.com.cn

[J04] 时间戳与日期互转
来源：http://cb.bookmarksfly.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tk.shtwfgs.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lq.hahajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://re.9csxet.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://kr.shxzukj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fh.gzmigu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bv.szsharing.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pj.bjjhwx.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://on.huanxung.cn

[J05] 时间加减（加 7 天）
来源：http://hs.shxzskj.cn

Py:   now + timedelta(days=7)
来源：http://sh.szxytkj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mx.jctech888.com.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yl.panjiajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jk.wgjwhj.cn

Java: LocalDate.now().plusDays(7)
来源：http://uo.shxzskj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://eq.9csxet.cn

Ruby: Time.now + 7 * 86400
来源：http://sd.hnjuh.cn

C#:   DateTime.Now.AddDays(7)
来源：http://dg.yuexingan06.cn

[J06] 计算两时间之差
来源：http://pr.newstarts.cn

Py:   (end - start).total_seconds()
来源：http://ft.huixinmuqiang.cn

PHP:  $end->diff($start)->days;
来源：http://oq.jianghongdianzi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://oh.shxzukj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ef.huixiangedu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ch.nicolike.cn

Go:   end.Sub(start).Hours()
来源：http://fl.shxzskj.cn

Ruby: end - start                 # 返回秒数
来源：http://ye.panjiajie.cn

C#:   (end - start).TotalSeconds
来源：http://jr.gzmigu.cn

[J07] 比较两个日期
来源：http://zc.nicolike.cn

Py:   d1 < d2;  d1 == d2
来源：http://ka.haigaiapp.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://us.lnxyls.cn

JS:   d1.getTime() < d2.getTime()
来源：http://av.bjjhwx.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rp.shxzskj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://oz.huixinmuqiang.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ez.shxzskj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://nx.huixinmuqiang.cn

C#:   d1 < d2;  d1 == d2
来源：http://im.muxihuayi.cn

[J08] 提取年月日与星期
来源：http://rw.shxzskj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fp.shtwfgs.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wm.521024.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pl.newstarts.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ns.muxihuayi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mq.szsharing.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://os.newstarts.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yc.yuexingan06.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hr.lnxyls.cn

[J09] 时区处理
来源：http://ee.521024.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gs.bjjhwx.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ur.521024.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vj.panjiajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hw.lnxyls.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pi.colortex.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pr.gzmigu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xj.jianghongdianzi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ii.521024.cn

[J10] 取今天 / 本月第一天
来源：http://kn.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://aa.hnjuh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sx.muxihuayi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gp.panjiajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ch.huixiangedu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hv.wgjwhj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pg.haigaiapp.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vl.hahajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://iq.nicolike.cn

================================================================================
来源：http://uu.colortex.cn

K. JSON 与序列化
来源：http://lc.shxzukj.cn

================================================================================
来源：http://cq.521024.cn

[K01] 对象转 JSON 字符串
来源：http://gx.jctech888.com.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fc.colortex.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qw.nszjky.cn

JS:   JSON.stringify(obj)
来源：http://hw.bjjhwx.cn

TS:   JSON.stringify(obj)
来源：http://og.yuexingan06.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bu.gzmigu.cn

Go:   json.Marshal(obj)
来源：http://uy.asd995.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ms.gzmigu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jg.lnxyls.cn

[K02] JSON 字符串转对象
来源：http://hc.asd995.cn

Py:   json.loads(s)
来源：http://vq.newstarts.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wj.521024.cn

JS:   JSON.parse(s)
来源：http://ps.colortex.cn

TS:   JSON.parse(s)
来源：http://wo.jianghongdianzi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rb.huixiangedu.cn

Go:   json.Unmarshal(data, &v)
来源：http://oq.szxytkj.cn

Ruby: JSON.parse(s)
来源：http://gm.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cf.szsharing.cn

[K03] JSON 美化输出（带缩进）
来源：http://jh.hnjuh.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ry.huixiangedu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fj.muxihuayi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ia.huixinmuqiang.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qu.shtwfgs.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ig.szsharing.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zy.asd995.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kf.gzmigu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xh.9csxet.cn

[K04] 读取 JSON 文件
来源：http://wx.chemitech.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nq.haigaiapp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ks.gzmigu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oj.jctech888.com.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://it.szxytkj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bn.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nn.szxytkj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yj.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qb.jianghongdianzi.cn

[K05] 深拷贝对象
来源：http://jm.521024.cn

Py:   copy.deepcopy(obj)
来源：http://or.gzmigu.cn

PHP:  unserialize(serialize($obj));
来源：http://yu.szxytkj.cn

JS:   structuredClone(obj)
来源：http://kq.bjjhwx.cn

TS:   structuredClone(obj)
来源：http://yl.yuexingan06.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dt.shxzskj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cy.nszjky.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wg.yuexingan06.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xl.9csxet.cn

[K06] 解析 URL 查询串
来源：http://dj.nszjky.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ww.asd995.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hc.yuexingan06.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vh.shxzskj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xv.colortex.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lb.asd995.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ef.szsharing.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mh.521024.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ja.shxzskj.cn

[K07] 进制转换
来源：http://kp.9csxet.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fj.shxzukj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mp.colortex.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vr.521024.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dr.hahajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nx.jctech888.com.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yr.shxzskj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zs.newstarts.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://su.newstarts.cn

[K08] 二进制序列化（非 JSON）
来源：http://qr.jianghongdianzi.cn

Py:   pickle.dumps(obj)
来源：http://nj.hnjuh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lj.szxytkj.cn

JS:   v8.serialize(obj)        // Node
来源：http://gh.chemitech.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://ld.asd995.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qh.hahajie.cn

Go:   encoding/gob
来源：http://aq.jianghongdianzi.cn

Ruby: Marshal.dump(obj)
来源：http://ur.colortex.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ni.gzmigu.cn

================================================================================
来源：http://al.chemitech.net.cn

L. 网络请求
来源：http://cx.asd995.cn

================================================================================
来源：http://xt.yuexingan06.cn

[L01] 发送 GET 请求
来源：http://ts.muxihuayi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kn.haigaiapp.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gd.muxihuayi.cn

JS:   await fetch(url)
来源：http://qo.9csxet.cn

TS:   await fetch(url)
来源：http://xu.521024.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gz.shtwfgs.cn

Go:   resp, err := http.Get(url)
来源：http://xv.yuexingan06.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xn.haigaiapp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qv.newstarts.cn

[L02] 发送 POST JSON
来源：http://do.panjiajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://sh.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://oy.shxzukj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ao.wgjwhj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ih.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kb.hahajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oy.hnjuh.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lf.lnxyls.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dz.shxzukj.cn

[L03] 设置自定义请求头
来源：http://oe.huixiangedu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fv.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uo.colortex.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ww.nszjky.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sc.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jt.bookmarksfly.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://je.lnxyls.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wb.szsharing.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jr.bookmarksfly.cn

[L04] 设置超时
来源：http://is.huixiangedu.cn

Py:   requests.get(url, timeout=5)
来源：http://ky.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://te.szxytkj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mr.wgjwhj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jd.shtwfgs.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ng.bjjhwx.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nb.nicolike.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qm.asd995.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mr.szxytkj.cn

[L05] 上传文件（multipart）
来源：http://ej.huixiangedu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nk.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lp.colortex.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jb.hahajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kx.huixiangedu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ox.asd995.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uz.gzmigu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zw.nszjky.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bn.panjiajie.cn

[L06] 解析响应为 JSON
来源：http://xq.wgjwhj.cn

Py:   resp.json()
来源：http://vv.hnjuh.cn

PHP:  json_decode($body, true);
来源：http://mc.hahajie.cn

JS:   await resp.json()
来源：http://db.yuexingan06.cn

TS:   await resp.json()
来源：http://bs.jctech888.com.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nj.lnxyls.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://on.jianghongdianzi.cn

Ruby: JSON.parse(resp.body)
来源：http://ar.nszjky.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cc.newstarts.cn

[L07] 处理 HTTP 状态码
来源：http://kc.nszjky.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cf.huixinmuqiang.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://az.chemitech.net.cn

JS:   resp.ok;  resp.status
来源：http://ew.huixinmuqiang.cn

TS:   resp.ok;  resp.status
来源：http://qa.lnxyls.cn

Java: resp.statusCode()
来源：http://uj.shxzukj.cn

Go:   resp.StatusCode
来源：http://vd.521024.cn

Ruby: resp.code.to_i
来源：http://gc.newstarts.cn

C#:   (int)resp.StatusCode
来源：http://oe.huixiangedu.cn

[L08] 并发请求多个地址
来源：http://jt.panjiajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fo.nicolike.cn

PHP:  curl_multi_init() 系列
来源：http://oy.colortex.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ki.hahajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qn.521024.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yg.shtwfgs.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jv.jianghongdianzi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vl.shxzskj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pw.521024.cn

================================================================================
来源：http://ae.nicolike.cn

M. 命令行 / 进程 / 环境
来源：http://zh.9csxet.cn

================================================================================
来源：http://nx.huixinmuqiang.cn

[M01] 读取命令行参数
来源：http://nk.chemitech.net.cn

Py:   sys.argv[1:]
来源：http://eo.huixinmuqiang.cn

PHP:  $argv;  $argc;
来源：http://ap.bjjhwx.cn

JS:   process.argv.slice(2)
来源：http://vj.szxytkj.cn

TS:   process.argv.slice(2)
来源：http://iz.huixinmuqiang.cn

Java: args 数组（main 方法参数）
来源：http://ap.lnxyls.cn

Go:   os.Args[1:]
来源：http://jy.szsharing.cn

Ruby: ARGV
来源：http://pc.shxzskj.cn

C#:   args 数组（Main 方法参数）
来源：http://au.9csxet.cn

[M02] 读取环境变量
来源：http://ko.yuntaijiaju.cn

Py:   os.environ.get("HOME")
来源：http://sc.hahajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cb.hnjuh.cn

JS:   process.env.HOME
来源：http://qw.newstarts.cn

TS:   process.env.HOME
来源：http://ve.haigaiapp.cn

Java: System.getenv("HOME")
来源：http://bt.jctech888.com.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zj.gzmigu.cn

Ruby: ENV["HOME"]
来源：http://ew.muxihuayi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yd.nszjky.cn

[M03] 执行外部命令
来源：http://ld.yuexingan06.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hq.muxihuayi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://so.yuntaijiaju.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ob.haigaiapp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pj.yuexingan06.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fw.chemitech.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://kn.huixiangedu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://cs.panjiajie.cn

C#:   Process.Start("ls", "-l");
来源：http://ky.chemitech.net.cn


<!-- 参考信息 -->