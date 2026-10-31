代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jh.bjjhwx.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ps.haigaiapp.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qh.yuntaijiaju.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://us.9csxet.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jk.jianghongdianzi.cn

[I07] 忽略大小写与多行模式
来源：http://xo.chemitech.net.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ma.nszjky.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://na.yuntaijiaju.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kq.huixiangedu.cn

TS:   /error/gim
来源：http://it.huixiangedu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://je.nicolike.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ud.szxytkj.cn

Ruby: s.scan(/error/i)
来源：http://vz.haigaiapp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qz.chemitech.net.cn

[I08] 贪婪与非贪婪匹配
来源：http://wg.szxytkj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://df.wgjwhj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bj.lnxyls.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pi.shtwfgs.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qa.9csxet.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gv.szsharing.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ep.hnjuh.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://li.shxzukj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tj.shtwfgs.cn

================================================================================
来源：http://sh.lnxyls.cn

J. 日期与时间
来源：http://bz.nszjky.cn

================================================================================
来源：http://gq.huanxung.cn

[J01] 获取当前时间
来源：http://ba.hahajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://aa.wgjwhj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wy.hahajie.cn

JS:   new Date();  Date.now()
来源：http://qm.hnjuh.cn

TS:   new Date();  Date.now()
来源：http://fh.yuexingan06.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fv.asd995.cn

Go:   time.Now()
来源：http://fr.chemitech.net.cn

Ruby: Time.now
来源：http://qt.wgjwhj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kz.jianghongdianzi.cn

[J02] 格式化输出
来源：http://ed.shxzukj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oe.shtwfgs.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hf.gzmigu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qx.hnjuh.cn

TS:   d.toISOString()
来源：http://qs.521024.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jv.bookmarksfly.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vy.9csxet.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zy.szsharing.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gg.chemitech.net.cn

[J03] 字符串解析为日期
来源：http://aq.muxihuayi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kc.hahajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://iw.haigaiapp.cn

JS:   new Date("2024-01-02")
来源：http://mn.bjjhwx.cn

TS:   new Date("2024-01-02")
来源：http://aj.bookmarksfly.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zx.shxzukj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tg.nicolike.cn

Ruby: Date.parse("2024-01-02")
来源：http://ll.shxzskj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nl.9csxet.cn

[J04] 时间戳与日期互转
来源：http://bx.huanxung.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hf.gzmigu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mt.panjiajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://is.haigaiapp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bu.huanxung.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tu.9csxet.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://us.muxihuayi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hw.bjjhwx.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ra.lnxyls.cn

[J05] 时间加减（加 7 天）
来源：http://no.shxzukj.cn

Py:   now + timedelta(days=7)
来源：http://nv.nszjky.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nz.huixinmuqiang.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://so.szxytkj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://te.nicolike.cn

Java: LocalDate.now().plusDays(7)
来源：http://qy.jctech888.com.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rp.yuexingan06.cn

Ruby: Time.now + 7 * 86400
来源：http://uv.bookmarksfly.cn

C#:   DateTime.Now.AddDays(7)
来源：http://tw.chemitech.net.cn

[J06] 计算两时间之差
来源：http://jr.huanxung.cn

Py:   (end - start).total_seconds()
来源：http://rl.shtwfgs.cn

PHP:  $end->diff($start)->days;
来源：http://ti.asd995.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yz.shxzskj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xi.shxzukj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://uo.hnjuh.cn

Go:   end.Sub(start).Hours()
来源：http://dd.jianghongdianzi.cn

Ruby: end - start                 # 返回秒数
来源：http://do.szsharing.cn

C#:   (end - start).TotalSeconds
来源：http://rc.huanxung.cn

[J07] 比较两个日期
来源：http://ep.lnxyls.cn

Py:   d1 < d2;  d1 == d2
来源：http://be.yuntaijiaju.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bv.szxytkj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ht.nszjky.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bb.shxzukj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tf.colortex.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://oh.shxzskj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://co.panjiajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://pk.bjjhwx.cn

[J08] 提取年月日与星期
来源：http://tm.yuexingan06.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wh.nicolike.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hi.bookmarksfly.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lx.gzmigu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uw.szsharing.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://md.jianghongdianzi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ju.bookmarksfly.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rw.yuexingan06.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vv.huixiangedu.cn

[J09] 时区处理
来源：http://bq.szsharing.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ip.gzmigu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://eq.szsharing.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ot.muxihuayi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eh.colortex.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kq.521024.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://va.nszjky.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lf.huanxung.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tq.yuexingan06.cn

[J10] 取今天 / 本月第一天
来源：http://uw.chemitech.net.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gs.9csxet.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tx.yuntaijiaju.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://no.shtwfgs.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jo.newstarts.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hf.shxzskj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wl.huanxung.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fy.huanxung.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wu.colortex.cn

================================================================================
来源：http://eb.shtwfgs.cn

K. JSON 与序列化
来源：http://qa.huixinmuqiang.cn

================================================================================
来源：http://nc.asd995.cn

[K01] 对象转 JSON 字符串
来源：http://kz.colortex.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bv.hnjuh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xy.nicolike.cn

JS:   JSON.stringify(obj)
来源：http://tg.yuntaijiaju.cn

TS:   JSON.stringify(obj)
来源：http://kb.jianghongdianzi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://me.jianghongdianzi.cn

Go:   json.Marshal(obj)
来源：http://jb.nicolike.cn

Ruby: obj.to_json                                     // require "json"
来源：http://pf.shxzukj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://la.huixiangedu.cn

[K02] JSON 字符串转对象
来源：http://vw.haigaiapp.cn

Py:   json.loads(s)
来源：http://fw.szxytkj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gt.haigaiapp.cn

JS:   JSON.parse(s)
来源：http://hy.bjjhwx.cn

TS:   JSON.parse(s)
来源：http://dq.huanxung.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tf.gzmigu.cn

Go:   json.Unmarshal(data, &v)
来源：http://ow.muxihuayi.cn

Ruby: JSON.parse(s)
来源：http://wu.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ic.shxzukj.cn

[K03] JSON 美化输出（带缩进）
来源：http://ft.szsharing.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fw.gzmigu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ct.lnxyls.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://va.shxzukj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vo.gzmigu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://om.shxzskj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kq.nszjky.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dg.hnjuh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wq.muxihuayi.cn

[K04] 读取 JSON 文件
来源：http://kd.nicolike.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ta.huanxung.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fu.lnxyls.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ry.wgjwhj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cw.newstarts.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://db.shxzskj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ee.bjjhwx.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://kx.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hb.hahajie.cn

[K05] 深拷贝对象
来源：http://ac.shtwfgs.cn

Py:   copy.deepcopy(obj)
来源：http://er.yuexingan06.cn

PHP:  unserialize(serialize($obj));
来源：http://hh.lnxyls.cn

JS:   structuredClone(obj)
来源：http://oj.hnjuh.cn

TS:   structuredClone(obj)
来源：http://gc.yuntaijiaju.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qu.521024.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bx.gzmigu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yr.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ty.chemitech.net.cn

[K06] 解析 URL 查询串
来源：http://hy.huixiangedu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kb.hnjuh.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yk.shxzskj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vl.gzmigu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ue.panjiajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gd.newstarts.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gp.9csxet.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://it.asd995.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dw.muxihuayi.cn

[K07] 进制转换
来源：http://fm.shxzskj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ml.9csxet.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lv.9csxet.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ik.haigaiapp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ak.muxihuayi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sm.shxzskj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rp.huanxung.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bl.huixinmuqiang.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pn.asd995.cn

[K08] 二进制序列化（非 JSON）
来源：http://rj.huixiangedu.cn

Py:   pickle.dumps(obj)
来源：http://wm.newstarts.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hv.jctech888.com.cn

JS:   v8.serialize(obj)        // Node
来源：http://qc.muxihuayi.cn

TS:   v8.serialize(obj)        // Node
来源：http://iq.shxzskj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://da.hahajie.cn

Go:   encoding/gob
来源：http://af.wgjwhj.cn

Ruby: Marshal.dump(obj)
来源：http://js.shxzukj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ty.nszjky.cn

================================================================================
来源：http://wq.panjiajie.cn

L. 网络请求
来源：http://op.muxihuayi.cn

================================================================================
来源：http://rg.yuexingan06.cn

[L01] 发送 GET 请求
来源：http://is.haigaiapp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ah.bjjhwx.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ia.hnjuh.cn

JS:   await fetch(url)
来源：http://jg.panjiajie.cn

TS:   await fetch(url)
来源：http://nv.panjiajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sh.haigaiapp.cn

Go:   resp, err := http.Get(url)
来源：http://nw.hnjuh.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ld.huixinmuqiang.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ke.521024.cn

[L02] 发送 POST JSON
来源：http://gw.hnjuh.cn

Py:   requests.post(url, json={"a": 1})
来源：http://dt.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yd.asd995.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vq.521024.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qz.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ud.muxihuayi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wx.huanxung.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ei.muxihuayi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nq.huixiangedu.cn

[L03] 设置自定义请求头
来源：http://qu.hnjuh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ui.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fb.szsharing.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ir.chemitech.net.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yy.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rj.wgjwhj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://au.chemitech.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pg.shtwfgs.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bv.newstarts.cn

[L04] 设置超时
来源：http://mt.gzmigu.cn

Py:   requests.get(url, timeout=5)
来源：http://xm.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hs.hahajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jw.gzmigu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ew.bookmarksfly.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fz.gzmigu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lk.panjiajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kx.panjiajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jh.asd995.cn

[L05] 上传文件（multipart）
来源：http://zp.szxytkj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rn.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gd.bjjhwx.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rs.gzmigu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jk.panjiajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ji.wgjwhj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pp.gzmigu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ix.szxytkj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yn.lnxyls.cn

[L06] 解析响应为 JSON
来源：http://nf.gzmigu.cn

Py:   resp.json()
来源：http://hi.shxzukj.cn

PHP:  json_decode($body, true);
来源：http://av.shxzukj.cn

JS:   await resp.json()
来源：http://sh.wgjwhj.cn

TS:   await resp.json()
来源：http://tp.gzmigu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dq.jianghongdianzi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ed.521024.cn

Ruby: JSON.parse(resp.body)
来源：http://fl.colortex.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bm.szxytkj.cn

[L07] 处理 HTTP 状态码
来源：http://oe.szsharing.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jc.yuexingan06.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cw.nicolike.cn

JS:   resp.ok;  resp.status
来源：http://pc.shxzukj.cn

TS:   resp.ok;  resp.status
来源：http://tn.haigaiapp.cn

Java: resp.statusCode()
来源：http://vf.bjjhwx.cn

Go:   resp.StatusCode
来源：http://kl.asd995.cn

Ruby: resp.code.to_i
来源：http://cv.jianghongdianzi.cn

C#:   (int)resp.StatusCode
来源：http://zj.huixinmuqiang.cn

[L08] 并发请求多个地址
来源：http://pw.yuntaijiaju.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xi.huanxung.cn

PHP:  curl_multi_init() 系列
来源：http://ld.jctech888.com.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cd.shxzskj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tb.bjjhwx.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mv.bjjhwx.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xm.521024.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qq.shxzukj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qw.521024.cn

================================================================================
来源：http://fh.hnjuh.cn

M. 命令行 / 进程 / 环境
来源：http://xk.shxzukj.cn

================================================================================
来源：http://sa.shtwfgs.cn

[M01] 读取命令行参数
来源：http://yb.hahajie.cn

Py:   sys.argv[1:]
来源：http://sf.shtwfgs.cn

PHP:  $argv;  $argc;
来源：http://cx.521024.cn

JS:   process.argv.slice(2)
来源：http://dh.shtwfgs.cn

TS:   process.argv.slice(2)
来源：http://na.bookmarksfly.cn

Java: args 数组（main 方法参数）
来源：http://jr.lnxyls.cn

Go:   os.Args[1:]
来源：http://jz.jctech888.com.cn

Ruby: ARGV
来源：http://wf.nicolike.cn

C#:   args 数组（Main 方法参数）
来源：http://ak.lnxyls.cn

[M02] 读取环境变量
来源：http://av.jianghongdianzi.cn

Py:   os.environ.get("HOME")
来源：http://wt.wgjwhj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ie.yuntaijiaju.cn

JS:   process.env.HOME
来源：http://ai.szxytkj.cn

TS:   process.env.HOME
来源：http://xp.colortex.cn

Java: System.getenv("HOME")
来源：http://vi.huixinmuqiang.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://uf.yuexingan06.cn

Ruby: ENV["HOME"]
来源：http://vy.shxzskj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://eb.bjjhwx.cn

[M03] 执行外部命令
来源：http://ft.521024.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://iq.wgjwhj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://eh.lnxyls.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gz.521024.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://en.wgjwhj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://oz.shxzukj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vf.huixiangedu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://dd.jianghongdianzi.cn

C#:   Process.Start("ls", "-l");
来源：http://ul.huanxung.cn

[M04] 获取当前工作目录
来源：http://hs.panjiajie.cn

Py:   os.getcwd()
来源：http://ms.szsharing.cn

PHP:  getcwd();
来源：http://xj.bjjhwx.cn

JS:   process.cwd()
来源：http://oq.haigaiapp.cn


<!-- 参考信息 -->