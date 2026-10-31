代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jy.panjiajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dd.shtwfgs.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lo.huixiangedu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pw.yuntaijiaju.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://on.lnxyls.cn

[I07] 忽略大小写与多行模式
来源：http://kt.yuntaijiaju.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cz.shxzukj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vs.muxihuayi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zc.yuntaijiaju.cn

TS:   /error/gim
来源：http://js.bjjhwx.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://di.colortex.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ls.newstarts.cn

Ruby: s.scan(/error/i)
来源：http://fa.huixinmuqiang.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sz.shxzukj.cn

[I08] 贪婪与非贪婪匹配
来源：http://zr.yuexingan06.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bs.gzmigu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vt.bookmarksfly.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ji.chemitech.net.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://si.huixiangedu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://yy.hnjuh.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qt.hahajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xq.lnxyls.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ys.haigaiapp.cn

================================================================================
来源：http://fb.colortex.cn

J. 日期与时间
来源：http://qb.colortex.cn

================================================================================
来源：http://yy.9csxet.cn

[J01] 获取当前时间
来源：http://le.shtwfgs.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://mc.yuntaijiaju.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://es.lnxyls.cn

JS:   new Date();  Date.now()
来源：http://io.521024.cn

TS:   new Date();  Date.now()
来源：http://vn.wgjwhj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hv.shxzukj.cn

Go:   time.Now()
来源：http://hr.bookmarksfly.cn

Ruby: Time.now
来源：http://vg.gzmigu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xz.nszjky.cn

[J02] 格式化输出
来源：http://et.jctech888.com.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ob.hahajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hh.hahajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mx.muxihuayi.cn

TS:   d.toISOString()
来源：http://za.panjiajie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zv.muxihuayi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rs.hnjuh.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vh.nszjky.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://he.asd995.cn

[J03] 字符串解析为日期
来源：http://hp.gzmigu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wj.nicolike.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://al.asd995.cn

JS:   new Date("2024-01-02")
来源：http://dw.szsharing.cn

TS:   new Date("2024-01-02")
来源：http://xk.shtwfgs.cn

Java: LocalDate.parse("2024-01-02")
来源：http://sc.hahajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xg.szxytkj.cn

Ruby: Date.parse("2024-01-02")
来源：http://bl.wgjwhj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uf.yuexingan06.cn

[J04] 时间戳与日期互转
来源：http://sj.asd995.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xz.lnxyls.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qx.9csxet.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tx.nicolike.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ci.jianghongdianzi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gr.nszjky.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wj.jctech888.com.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qt.bjjhwx.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wj.bjjhwx.cn

[J05] 时间加减（加 7 天）
来源：http://ox.szsharing.cn

Py:   now + timedelta(days=7)
来源：http://ev.szsharing.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sj.haigaiapp.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://px.shtwfgs.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://se.wgjwhj.cn

Java: LocalDate.now().plusDays(7)
来源：http://da.huixiangedu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pk.muxihuayi.cn

Ruby: Time.now + 7 * 86400
来源：http://fr.huixinmuqiang.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xa.muxihuayi.cn

[J06] 计算两时间之差
来源：http://kq.panjiajie.cn

Py:   (end - start).total_seconds()
来源：http://xl.panjiajie.cn

PHP:  $end->diff($start)->days;
来源：http://mz.bookmarksfly.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lb.jianghongdianzi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cf.bookmarksfly.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hc.szxytkj.cn

Go:   end.Sub(start).Hours()
来源：http://lm.muxihuayi.cn

Ruby: end - start                 # 返回秒数
来源：http://gv.szxytkj.cn

C#:   (end - start).TotalSeconds
来源：http://cf.szsharing.cn

[J07] 比较两个日期
来源：http://xt.shxzukj.cn

Py:   d1 < d2;  d1 == d2
来源：http://ph.wgjwhj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lc.521024.cn

JS:   d1.getTime() < d2.getTime()
来源：http://za.nszjky.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xj.chemitech.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sw.hnjuh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rg.szsharing.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ti.nszjky.cn

C#:   d1 < d2;  d1 == d2
来源：http://ej.jianghongdianzi.cn

[J08] 提取年月日与星期
来源：http://kl.chemitech.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hd.shtwfgs.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kj.nszjky.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yl.muxihuayi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hh.muxihuayi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ig.nszjky.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gi.hahajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kv.szxytkj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rc.yuntaijiaju.cn

[J09] 时区处理
来源：http://ff.hnjuh.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fv.shtwfgs.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ao.jianghongdianzi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yw.chemitech.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://us.shxzukj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://id.colortex.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ba.huixinmuqiang.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yb.shxzskj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nd.panjiajie.cn

[J10] 取今天 / 本月第一天
来源：http://ki.colortex.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://oo.wgjwhj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ni.nszjky.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cc.hnjuh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bw.yuexingan06.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xw.hnjuh.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lc.bookmarksfly.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fv.huixinmuqiang.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://du.huixinmuqiang.cn

================================================================================
来源：http://nu.9csxet.cn

K. JSON 与序列化
来源：http://ag.jianghongdianzi.cn

================================================================================
来源：http://lg.panjiajie.cn

[K01] 对象转 JSON 字符串
来源：http://gg.muxihuayi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rr.lnxyls.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cm.lnxyls.cn

JS:   JSON.stringify(obj)
来源：http://zi.bjjhwx.cn

TS:   JSON.stringify(obj)
来源：http://kv.haigaiapp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pv.muxihuayi.cn

Go:   json.Marshal(obj)
来源：http://bs.panjiajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ug.szsharing.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://oz.hnjuh.cn

[K02] JSON 字符串转对象
来源：http://wr.panjiajie.cn

Py:   json.loads(s)
来源：http://sm.gzmigu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ba.yuntaijiaju.cn

JS:   JSON.parse(s)
来源：http://fp.bookmarksfly.cn

TS:   JSON.parse(s)
来源：http://br.bjjhwx.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dj.shxzskj.cn

Go:   json.Unmarshal(data, &v)
来源：http://dm.hahajie.cn

Ruby: JSON.parse(s)
来源：http://ga.521024.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tk.hahajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://zs.chemitech.net.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://st.colortex.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mk.huixinmuqiang.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://lx.bjjhwx.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tj.hahajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gc.shtwfgs.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lr.yuexingan06.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wx.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pv.lnxyls.cn

[K04] 读取 JSON 文件
来源：http://gf.shtwfgs.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ge.shtwfgs.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://am.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vm.hahajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kg.nicolike.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hv.hahajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ne.haigaiapp.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mz.asd995.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sd.muxihuayi.cn

[K05] 深拷贝对象
来源：http://wu.jctech888.com.cn

Py:   copy.deepcopy(obj)
来源：http://bx.jctech888.com.cn

PHP:  unserialize(serialize($obj));
来源：http://tm.huixinmuqiang.cn

JS:   structuredClone(obj)
来源：http://lj.chemitech.net.cn

TS:   structuredClone(obj)
来源：http://sz.huixinmuqiang.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ov.nszjky.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://eg.hahajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bb.asd995.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zu.asd995.cn

[K06] 解析 URL 查询串
来源：http://cl.jctech888.com.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bk.nszjky.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dr.yuexingan06.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gp.wgjwhj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gt.huixinmuqiang.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ec.yuexingan06.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rz.jianghongdianzi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hc.lnxyls.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xe.jianghongdianzi.cn

[K07] 进制转换
来源：http://zw.muxihuayi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wb.yuntaijiaju.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fx.colortex.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tz.yuexingan06.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vf.haigaiapp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://eh.bookmarksfly.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bz.wgjwhj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fb.lnxyls.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jd.newstarts.cn

[K08] 二进制序列化（非 JSON）
来源：http://aq.huixiangedu.cn

Py:   pickle.dumps(obj)
来源：http://cl.colortex.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ui.huixiangedu.cn

JS:   v8.serialize(obj)        // Node
来源：http://kk.9csxet.cn

TS:   v8.serialize(obj)        // Node
来源：http://bl.gzmigu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mu.nicolike.cn

Go:   encoding/gob
来源：http://ul.shtwfgs.cn

Ruby: Marshal.dump(obj)
来源：http://bo.shtwfgs.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yc.gzmigu.cn

================================================================================
来源：http://fe.yuntaijiaju.cn

L. 网络请求
来源：http://nz.lnxyls.cn

================================================================================
来源：http://ty.huixiangedu.cn

[L01] 发送 GET 请求
来源：http://fd.panjiajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nt.wgjwhj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rz.huanxung.cn

JS:   await fetch(url)
来源：http://qp.bookmarksfly.cn

TS:   await fetch(url)
来源：http://qr.huixinmuqiang.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xv.hahajie.cn

Go:   resp, err := http.Get(url)
来源：http://oo.lnxyls.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ri.szsharing.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bg.colortex.cn

[L02] 发送 POST JSON
来源：http://jw.colortex.cn

Py:   requests.post(url, json={"a": 1})
来源：http://jh.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sr.gzmigu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ik.hahajie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ug.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qw.jctech888.com.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vc.yuntaijiaju.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ff.nszjky.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kh.shxzskj.cn

[L03] 设置自定义请求头
来源：http://rv.huanxung.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kl.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wy.nszjky.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vx.wgjwhj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mn.asd995.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jj.haigaiapp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sr.huixiangedu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uh.jctech888.com.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://in.wgjwhj.cn

[L04] 设置超时
来源：http://um.huixinmuqiang.cn

Py:   requests.get(url, timeout=5)
来源：http://cm.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qd.shtwfgs.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dm.huanxung.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ii.colortex.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://oy.asd995.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ry.jctech888.com.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://oh.huixinmuqiang.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gd.yuntaijiaju.cn

[L05] 上传文件（multipart）
来源：http://id.huixinmuqiang.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://iy.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mf.9csxet.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dp.szsharing.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://in.jianghongdianzi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://eu.szsharing.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pr.hahajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gn.newstarts.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gf.lnxyls.cn

[L06] 解析响应为 JSON
来源：http://hu.haigaiapp.cn

Py:   resp.json()
来源：http://zk.panjiajie.cn

PHP:  json_decode($body, true);
来源：http://jz.9csxet.cn

JS:   await resp.json()
来源：http://tt.huixinmuqiang.cn

TS:   await resp.json()
来源：http://jn.jctech888.com.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://np.jctech888.com.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vl.yuexingan06.cn

Ruby: JSON.parse(resp.body)
来源：http://vk.9csxet.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://da.chemitech.net.cn

[L07] 处理 HTTP 状态码
来源：http://mz.gzmigu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://is.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ij.newstarts.cn

JS:   resp.ok;  resp.status
来源：http://hw.wgjwhj.cn

TS:   resp.ok;  resp.status
来源：http://fq.haigaiapp.cn

Java: resp.statusCode()
来源：http://no.panjiajie.cn

Go:   resp.StatusCode
来源：http://sv.newstarts.cn

Ruby: resp.code.to_i
来源：http://xp.hnjuh.cn

C#:   (int)resp.StatusCode
来源：http://uj.asd995.cn

[L08] 并发请求多个地址
来源：http://dm.9csxet.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kb.colortex.cn

PHP:  curl_multi_init() 系列
来源：http://lx.szsharing.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rg.nszjky.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bd.yuexingan06.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://us.yuexingan06.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gf.chemitech.net.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jg.shxzskj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ig.yuntaijiaju.cn

================================================================================
来源：http://kc.nicolike.cn

M. 命令行 / 进程 / 环境
来源：http://im.yuntaijiaju.cn

================================================================================
来源：http://bp.bjjhwx.cn

[M01] 读取命令行参数
来源：http://bt.bjjhwx.cn

Py:   sys.argv[1:]
来源：http://ap.nicolike.cn

PHP:  $argv;  $argc;
来源：http://zj.colortex.cn

JS:   process.argv.slice(2)
来源：http://fj.wgjwhj.cn

TS:   process.argv.slice(2)
来源：http://rx.shxzukj.cn

Java: args 数组（main 方法参数）
来源：http://pf.521024.cn

Go:   os.Args[1:]
来源：http://gj.521024.cn

Ruby: ARGV
来源：http://jf.hahajie.cn

C#:   args 数组（Main 方法参数）
来源：http://ip.newstarts.cn

[M02] 读取环境变量
来源：http://uu.yuexingan06.cn

Py:   os.environ.get("HOME")
来源：http://jy.yuntaijiaju.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pr.muxihuayi.cn

JS:   process.env.HOME
来源：http://gj.9csxet.cn

TS:   process.env.HOME
来源：http://rt.wgjwhj.cn

Java: System.getenv("HOME")
来源：http://nn.jctech888.com.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xm.chemitech.net.cn

Ruby: ENV["HOME"]
来源：http://qu.nszjky.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kt.asd995.cn

[M03] 执行外部命令
来源：http://jw.muxihuayi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gm.yuntaijiaju.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yt.hnjuh.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xi.lnxyls.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://im.chemitech.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yn.bookmarksfly.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://iv.asd995.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rf.huixinmuqiang.cn

C#:   Process.Start("ls", "-l");
来源：http://ga.chemitech.net.cn

[M04] 获取当前工作目录
来源：http://js.szxytkj.cn

Py:   os.getcwd()
来源：http://ij.newstarts.cn

PHP:  getcwd();
来源：http://yl.asd995.cn

JS:   process.cwd()
来源：http://pi.gzmigu.cn


<!-- 参考信息 -->