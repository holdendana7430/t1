代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bv.hnjuh.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lq.yuntaijiaju.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wi.colortex.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vt.yuexingan06.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ur.gzmigu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dn.huanxung.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mn.panjiajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ee.panjiajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gm.huixinmuqiang.cn

[I07] 忽略大小写与多行模式
来源：http://zg.jctech888.com.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jh.bjjhwx.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uy.colortex.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ih.colortex.cn

TS:   /error/gim
来源：http://qg.shtwfgs.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dz.nicolike.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tc.yuexingan06.cn

Ruby: s.scan(/error/i)
来源：http://rr.shtwfgs.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yf.huixiangedu.cn

[I08] 贪婪与非贪婪匹配
来源：http://ny.nszjky.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sn.jianghongdianzi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rw.szxytkj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cg.haigaiapp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gt.chemitech.net.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lv.hnjuh.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://oo.bookmarksfly.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hb.jianghongdianzi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://su.gzmigu.cn

================================================================================
来源：http://xa.lnxyls.cn

J. 日期与时间
来源：http://hu.yuntaijiaju.cn

================================================================================
来源：http://av.jctech888.com.cn

[J01] 获取当前时间
来源：http://hq.shxzukj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fc.bjjhwx.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hp.jianghongdianzi.cn

JS:   new Date();  Date.now()
来源：http://ve.huanxung.cn

TS:   new Date();  Date.now()
来源：http://fz.gzmigu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vt.asd995.cn

Go:   time.Now()
来源：http://hs.shtwfgs.cn

Ruby: Time.now
来源：http://li.newstarts.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jj.colortex.cn

[J02] 格式化输出
来源：http://we.wgjwhj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://on.huixiangedu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yh.muxihuayi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jx.huixinmuqiang.cn

TS:   d.toISOString()
来源：http://vm.521024.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://og.yuexingan06.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qf.yuntaijiaju.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://li.jianghongdianzi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hv.9csxet.cn

[J03] 字符串解析为日期
来源：http://hv.wgjwhj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nu.wgjwhj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hi.szsharing.cn

JS:   new Date("2024-01-02")
来源：http://tx.nszjky.cn

TS:   new Date("2024-01-02")
来源：http://cz.huixinmuqiang.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ab.wgjwhj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://le.shxzskj.cn

Ruby: Date.parse("2024-01-02")
来源：http://dh.yuexingan06.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xe.huanxung.cn

[J04] 时间戳与日期互转
来源：http://ob.521024.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dy.bookmarksfly.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sm.panjiajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tg.huixiangedu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ys.colortex.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hk.yuexingan06.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rz.9csxet.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ta.wgjwhj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qc.huixinmuqiang.cn

[J05] 时间加减（加 7 天）
来源：http://ij.huixinmuqiang.cn

Py:   now + timedelta(days=7)
来源：http://fq.shxzskj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pp.yuntaijiaju.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wf.bookmarksfly.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sy.lnxyls.cn

Java: LocalDate.now().plusDays(7)
来源：http://sb.szsharing.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sn.szxytkj.cn

Ruby: Time.now + 7 * 86400
来源：http://fp.yuexingan06.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gb.muxihuayi.cn

[J06] 计算两时间之差
来源：http://on.yuexingan06.cn

Py:   (end - start).total_seconds()
来源：http://tz.bookmarksfly.cn

PHP:  $end->diff($start)->days;
来源：http://il.panjiajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fw.hnjuh.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sy.haigaiapp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bn.jianghongdianzi.cn

Go:   end.Sub(start).Hours()
来源：http://mp.wgjwhj.cn

Ruby: end - start                 # 返回秒数
来源：http://hw.shxzskj.cn

C#:   (end - start).TotalSeconds
来源：http://ie.szxytkj.cn

[J07] 比较两个日期
来源：http://aq.huixinmuqiang.cn

Py:   d1 < d2;  d1 == d2
来源：http://ul.lnxyls.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wz.jctech888.com.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ko.panjiajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gh.asd995.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://al.yuexingan06.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xi.shxzskj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xy.yuntaijiaju.cn

C#:   d1 < d2;  d1 == d2
来源：http://kx.hnjuh.cn

[J08] 提取年月日与星期
来源：http://ws.wgjwhj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cz.chemitech.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ce.chemitech.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://in.jianghongdianzi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cc.yuntaijiaju.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wl.muxihuayi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ty.nszjky.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gm.lnxyls.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xq.shxzukj.cn

[J09] 时区处理
来源：http://ip.haigaiapp.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gx.hahajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ca.521024.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gg.bjjhwx.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kb.521024.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cj.colortex.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ul.nszjky.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://nv.colortex.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ht.panjiajie.cn

[J10] 取今天 / 本月第一天
来源：http://mz.shtwfgs.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bi.hnjuh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zm.huanxung.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://by.bookmarksfly.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gu.jctech888.com.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qc.szxytkj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ad.shtwfgs.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vr.bjjhwx.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pp.huixinmuqiang.cn

================================================================================
来源：http://ju.bjjhwx.cn

K. JSON 与序列化
来源：http://fr.huanxung.cn

================================================================================
来源：http://es.szsharing.cn

[K01] 对象转 JSON 字符串
来源：http://mi.bjjhwx.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qy.yuexingan06.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cw.asd995.cn

JS:   JSON.stringify(obj)
来源：http://rj.shxzskj.cn

TS:   JSON.stringify(obj)
来源：http://xx.bookmarksfly.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fx.szsharing.cn

Go:   json.Marshal(obj)
来源：http://uq.huixiangedu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://iz.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vp.lnxyls.cn

[K02] JSON 字符串转对象
来源：http://lg.hnjuh.cn

Py:   json.loads(s)
来源：http://fv.hahajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dg.jianghongdianzi.cn

JS:   JSON.parse(s)
来源：http://dg.hahajie.cn

TS:   JSON.parse(s)
来源：http://kd.newstarts.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ga.jctech888.com.cn

Go:   json.Unmarshal(data, &v)
来源：http://nq.nicolike.cn

Ruby: JSON.parse(s)
来源：http://rv.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hl.shtwfgs.cn

[K03] JSON 美化输出（带缩进）
来源：http://mq.asd995.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lv.hahajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ik.haigaiapp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ok.newstarts.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mv.huixiangedu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://on.huixinmuqiang.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ce.hnjuh.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gz.szxytkj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bn.panjiajie.cn

[K04] 读取 JSON 文件
来源：http://gd.huanxung.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fu.shxzukj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gf.yuntaijiaju.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yl.huixinmuqiang.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yc.colortex.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jf.huanxung.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lw.colortex.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://kw.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qc.nicolike.cn

[K05] 深拷贝对象
来源：http://dc.yuexingan06.cn

Py:   copy.deepcopy(obj)
来源：http://wi.yuntaijiaju.cn

PHP:  unserialize(serialize($obj));
来源：http://uz.nszjky.cn

JS:   structuredClone(obj)
来源：http://yk.shtwfgs.cn

TS:   structuredClone(obj)
来源：http://ef.huanxung.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hv.yuexingan06.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cj.shxzskj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://iv.nicolike.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tv.szsharing.cn

[K06] 解析 URL 查询串
来源：http://cr.szsharing.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://oa.9csxet.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vm.asd995.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://af.shxzukj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nq.hnjuh.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uu.gzmigu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wg.asd995.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://er.szxytkj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lh.chemitech.net.cn

[K07] 进制转换
来源：http://ad.chemitech.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ts.yuexingan06.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ig.muxihuayi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://iv.gzmigu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rw.nszjky.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tl.haigaiapp.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bv.hahajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ez.bjjhwx.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wy.haigaiapp.cn

[K08] 二进制序列化（非 JSON）
来源：http://ss.shxzukj.cn

Py:   pickle.dumps(obj)
来源：http://nd.newstarts.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bw.shxzskj.cn

JS:   v8.serialize(obj)        // Node
来源：http://qh.asd995.cn

TS:   v8.serialize(obj)        // Node
来源：http://zu.panjiajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://oa.bjjhwx.cn

Go:   encoding/gob
来源：http://bm.muxihuayi.cn

Ruby: Marshal.dump(obj)
来源：http://uw.hahajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gs.gzmigu.cn

================================================================================
来源：http://hn.shxzskj.cn

L. 网络请求
来源：http://gl.hahajie.cn

================================================================================
来源：http://zp.jianghongdianzi.cn

[L01] 发送 GET 请求
来源：http://pt.colortex.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xe.hahajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lc.hnjuh.cn

JS:   await fetch(url)
来源：http://yt.shxzukj.cn

TS:   await fetch(url)
来源：http://ul.shxzskj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ok.bookmarksfly.cn

Go:   resp, err := http.Get(url)
来源：http://rd.nszjky.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://vs.nicolike.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ao.nszjky.cn

[L02] 发送 POST JSON
来源：http://cz.lnxyls.cn

Py:   requests.post(url, json={"a": 1})
来源：http://jj.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ry.szsharing.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://se.muxihuayi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://se.colortex.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pk.521024.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jq.gzmigu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ew.jctech888.com.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sk.nicolike.cn

[L03] 设置自定义请求头
来源：http://ga.yuexingan06.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ln.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lj.bjjhwx.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://du.hnjuh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wb.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://st.newstarts.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rh.huanxung.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uo.chemitech.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mq.newstarts.cn

[L04] 设置超时
来源：http://xh.hahajie.cn

Py:   requests.get(url, timeout=5)
来源：http://dd.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ws.jianghongdianzi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lb.hahajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bw.panjiajie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fo.bookmarksfly.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://oa.shxzskj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nk.lnxyls.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rh.szsharing.cn

[L05] 上传文件（multipart）
来源：http://ql.shxzskj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://im.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sh.shtwfgs.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ha.shtwfgs.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://iw.jianghongdianzi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bc.shtwfgs.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xl.gzmigu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tq.hnjuh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ue.szxytkj.cn

[L06] 解析响应为 JSON
来源：http://vx.haigaiapp.cn

Py:   resp.json()
来源：http://dk.panjiajie.cn

PHP:  json_decode($body, true);
来源：http://sd.muxihuayi.cn

JS:   await resp.json()
来源：http://lx.newstarts.cn

TS:   await resp.json()
来源：http://cf.shtwfgs.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mi.bookmarksfly.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vu.9csxet.cn

Ruby: JSON.parse(resp.body)
来源：http://lw.shxzukj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kr.huanxung.cn

[L07] 处理 HTTP 状态码
来源：http://mb.wgjwhj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ob.nszjky.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cy.gzmigu.cn

JS:   resp.ok;  resp.status
来源：http://cl.jianghongdianzi.cn

TS:   resp.ok;  resp.status
来源：http://ho.huixiangedu.cn

Java: resp.statusCode()
来源：http://lr.bjjhwx.cn

Go:   resp.StatusCode
来源：http://zy.wgjwhj.cn

Ruby: resp.code.to_i
来源：http://xs.yuntaijiaju.cn

C#:   (int)resp.StatusCode
来源：http://tj.jctech888.com.cn

[L08] 并发请求多个地址
来源：http://tc.521024.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mc.newstarts.cn

PHP:  curl_multi_init() 系列
来源：http://ik.hnjuh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://my.haigaiapp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qr.newstarts.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hc.gzmigu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ch.bjjhwx.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pq.newstarts.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://op.huanxung.cn

================================================================================
来源：http://ok.huanxung.cn

M. 命令行 / 进程 / 环境
来源：http://xn.szsharing.cn

================================================================================
来源：http://jy.521024.cn

[M01] 读取命令行参数
来源：http://zq.wgjwhj.cn

Py:   sys.argv[1:]
来源：http://dl.huixinmuqiang.cn

PHP:  $argv;  $argc;
来源：http://za.nicolike.cn

JS:   process.argv.slice(2)
来源：http://bk.chemitech.net.cn

TS:   process.argv.slice(2)
来源：http://va.bjjhwx.cn

Java: args 数组（main 方法参数）
来源：http://mq.hahajie.cn

Go:   os.Args[1:]
来源：http://ry.newstarts.cn

Ruby: ARGV
来源：http://kk.szsharing.cn

C#:   args 数组（Main 方法参数）
来源：http://ad.yuexingan06.cn

[M02] 读取环境变量
来源：http://mf.huixiangedu.cn

Py:   os.environ.get("HOME")
来源：http://qq.szsharing.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wc.colortex.cn

JS:   process.env.HOME
来源：http://qh.nszjky.cn

TS:   process.env.HOME
来源：http://ae.bjjhwx.cn

Java: System.getenv("HOME")
来源：http://fb.panjiajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://km.colortex.cn

Ruby: ENV["HOME"]
来源：http://mc.shxzukj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fg.gzmigu.cn

[M03] 执行外部命令
来源：http://sk.nicolike.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://oh.haigaiapp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ks.9csxet.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ia.yuntaijiaju.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nq.jctech888.com.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mv.521024.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://kf.nicolike.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yg.hahajie.cn

C#:   Process.Start("ls", "-l");
来源：http://hh.colortex.cn


<!-- 参考信息 -->