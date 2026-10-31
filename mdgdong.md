代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://hs.szsharing.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hb.huixinmuqiang.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nn.huanxung.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pu.nszjky.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bc.yuntaijiaju.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hs.szxytkj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tl.hahajie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hj.shxzskj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bx.nszjky.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dm.shtwfgs.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wx.hahajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rb.bjjhwx.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wj.colortex.cn

[I07] 忽略大小写与多行模式
来源：http://yz.panjiajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pa.shtwfgs.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vz.haigaiapp.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mg.shxzukj.cn

TS:   /error/gim
来源：http://nj.newstarts.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ks.huanxung.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zc.szsharing.cn

Ruby: s.scan(/error/i)
来源：http://tf.nszjky.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cy.shxzskj.cn

[I08] 贪婪与非贪婪匹配
来源：http://xp.yuntaijiaju.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yw.shxzukj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kh.huanxung.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qf.9csxet.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ln.yuexingan06.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lw.szxytkj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pg.colortex.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://im.bjjhwx.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ua.jctech888.com.cn

================================================================================
来源：http://wh.szsharing.cn

J. 日期与时间
来源：http://kp.wgjwhj.cn

================================================================================
来源：http://hv.hnjuh.cn

[J01] 获取当前时间
来源：http://oe.bjjhwx.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ux.gzmigu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sx.wgjwhj.cn

JS:   new Date();  Date.now()
来源：http://hi.szxytkj.cn

TS:   new Date();  Date.now()
来源：http://up.gzmigu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://uu.asd995.cn

Go:   time.Now()
来源：http://va.colortex.cn

Ruby: Time.now
来源：http://gc.szsharing.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ru.nszjky.cn

[J02] 格式化输出
来源：http://ei.bjjhwx.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://om.nszjky.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ul.huanxung.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bx.wgjwhj.cn

TS:   d.toISOString()
来源：http://ua.gzmigu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ja.wgjwhj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yd.gzmigu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://al.shxzskj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cz.hnjuh.cn

[J03] 字符串解析为日期
来源：http://qo.9csxet.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ey.chemitech.net.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pl.wgjwhj.cn

JS:   new Date("2024-01-02")
来源：http://gk.lnxyls.cn

TS:   new Date("2024-01-02")
来源：http://au.nszjky.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ha.bookmarksfly.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://id.huixinmuqiang.cn

Ruby: Date.parse("2024-01-02")
来源：http://lk.nszjky.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vv.bjjhwx.cn

[J04] 时间戳与日期互转
来源：http://vu.jianghongdianzi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jg.yuntaijiaju.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://iy.hnjuh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wk.jctech888.com.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zd.haigaiapp.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tw.wgjwhj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lb.haigaiapp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ho.shxzskj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hw.jianghongdianzi.cn

[J05] 时间加减（加 7 天）
来源：http://px.huanxung.cn

Py:   now + timedelta(days=7)
来源：http://ei.yuntaijiaju.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ib.wgjwhj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lk.yuntaijiaju.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ik.yuntaijiaju.cn

Java: LocalDate.now().plusDays(7)
来源：http://xr.9csxet.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hw.yuexingan06.cn

Ruby: Time.now + 7 * 86400
来源：http://fb.9csxet.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vg.lnxyls.cn

[J06] 计算两时间之差
来源：http://hb.9csxet.cn

Py:   (end - start).total_seconds()
来源：http://cf.szsharing.cn

PHP:  $end->diff($start)->days;
来源：http://lg.haigaiapp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fq.chemitech.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://oj.521024.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ar.chemitech.net.cn

Go:   end.Sub(start).Hours()
来源：http://tv.muxihuayi.cn

Ruby: end - start                 # 返回秒数
来源：http://jh.huixiangedu.cn

C#:   (end - start).TotalSeconds
来源：http://xy.gzmigu.cn

[J07] 比较两个日期
来源：http://gi.hahajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://nk.hnjuh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wl.nszjky.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wy.shxzukj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://tt.huixiangedu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hw.hnjuh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fx.haigaiapp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://do.huixinmuqiang.cn

C#:   d1 < d2;  d1 == d2
来源：http://st.hnjuh.cn

[J08] 提取年月日与星期
来源：http://ay.huanxung.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jv.haigaiapp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pg.gzmigu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vr.newstarts.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hq.gzmigu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ik.szsharing.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ag.haigaiapp.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sm.lnxyls.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ij.huixinmuqiang.cn

[J09] 时区处理
来源：http://yu.nicolike.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yj.newstarts.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wr.szxytkj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wf.nicolike.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wa.lnxyls.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lg.bookmarksfly.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jx.yuexingan06.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gw.haigaiapp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://im.colortex.cn

[J10] 取今天 / 本月第一天
来源：http://wm.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ht.colortex.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xi.szsharing.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uq.szxytkj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lx.chemitech.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fy.haigaiapp.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wt.chemitech.net.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://le.jctech888.com.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://us.hahajie.cn

================================================================================
来源：http://ca.hnjuh.cn

K. JSON 与序列化
来源：http://tc.szsharing.cn

================================================================================
来源：http://kq.yuntaijiaju.cn

[K01] 对象转 JSON 字符串
来源：http://gt.wgjwhj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://er.521024.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hy.jianghongdianzi.cn

JS:   JSON.stringify(obj)
来源：http://qi.huixiangedu.cn

TS:   JSON.stringify(obj)
来源：http://gr.szxytkj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://be.panjiajie.cn

Go:   json.Marshal(obj)
来源：http://mm.nszjky.cn

Ruby: obj.to_json                                     // require "json"
来源：http://kt.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xz.shxzskj.cn

[K02] JSON 字符串转对象
来源：http://ii.gzmigu.cn

Py:   json.loads(s)
来源：http://tz.yuexingan06.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pw.chemitech.net.cn

JS:   JSON.parse(s)
来源：http://fz.shxzskj.cn

TS:   JSON.parse(s)
来源：http://gq.shxzskj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zv.yuexingan06.cn

Go:   json.Unmarshal(data, &v)
来源：http://by.shxzukj.cn

Ruby: JSON.parse(s)
来源：http://bh.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vv.jianghongdianzi.cn

[K03] JSON 美化输出（带缩进）
来源：http://ex.colortex.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qa.nicolike.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qb.huixinmuqiang.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://uc.yuntaijiaju.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nf.521024.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://op.lnxyls.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zn.bookmarksfly.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ah.colortex.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hd.9csxet.cn

[K04] 读取 JSON 文件
来源：http://it.muxihuayi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fc.gzmigu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://is.nszjky.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hi.haigaiapp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ud.wgjwhj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mt.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gx.szsharing.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ac.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mm.yuexingan06.cn

[K05] 深拷贝对象
来源：http://go.colortex.cn

Py:   copy.deepcopy(obj)
来源：http://ur.panjiajie.cn

PHP:  unserialize(serialize($obj));
来源：http://tf.colortex.cn

JS:   structuredClone(obj)
来源：http://dd.jctech888.com.cn

TS:   structuredClone(obj)
来源：http://hu.bookmarksfly.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ji.haigaiapp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ug.yuntaijiaju.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tv.yuexingan06.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mc.hahajie.cn

[K06] 解析 URL 查询串
来源：http://ge.colortex.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ar.nicolike.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fw.wgjwhj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hv.asd995.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://in.yuexingan06.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gh.panjiajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mc.jianghongdianzi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vh.bookmarksfly.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://le.nszjky.cn

[K07] 进制转换
来源：http://hj.haigaiapp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://up.chemitech.net.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://oa.jianghongdianzi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lz.hnjuh.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hc.huixiangedu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vx.szxytkj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pv.bookmarksfly.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ui.huixiangedu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rq.shtwfgs.cn

[K08] 二进制序列化（非 JSON）
来源：http://uq.huixinmuqiang.cn

Py:   pickle.dumps(obj)
来源：http://lf.9csxet.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vz.huanxung.cn

JS:   v8.serialize(obj)        // Node
来源：http://pt.521024.cn

TS:   v8.serialize(obj)        // Node
来源：http://cb.newstarts.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qs.panjiajie.cn

Go:   encoding/gob
来源：http://aj.yuntaijiaju.cn

Ruby: Marshal.dump(obj)
来源：http://gb.521024.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ci.nicolike.cn

================================================================================
来源：http://pa.nszjky.cn

L. 网络请求
来源：http://qj.huixinmuqiang.cn

================================================================================
来源：http://nh.huixiangedu.cn

[L01] 发送 GET 请求
来源：http://wf.lnxyls.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yc.colortex.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ir.wgjwhj.cn

JS:   await fetch(url)
来源：http://gh.bookmarksfly.cn

TS:   await fetch(url)
来源：http://xx.newstarts.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tw.colortex.cn

Go:   resp, err := http.Get(url)
来源：http://tb.yuexingan06.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://kj.gzmigu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lq.shxzukj.cn

[L02] 发送 POST JSON
来源：http://po.huanxung.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cg.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://md.chemitech.net.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zh.wgjwhj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wo.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ru.lnxyls.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fd.shtwfgs.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yr.yuexingan06.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zr.shxzskj.cn

[L03] 设置自定义请求头
来源：http://vq.asd995.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ih.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ip.newstarts.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lj.9csxet.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mo.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sg.shtwfgs.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ge.szsharing.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gv.newstarts.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ab.9csxet.cn

[L04] 设置超时
来源：http://ns.hnjuh.cn

Py:   requests.get(url, timeout=5)
来源：http://mh.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ck.hnjuh.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ct.shxzukj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ho.asd995.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hk.9csxet.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://oy.panjiajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://el.hahajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pr.chemitech.net.cn

[L05] 上传文件（multipart）
来源：http://hg.gzmigu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vo.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sv.hahajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ov.gzmigu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pu.yuexingan06.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ef.nszjky.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vz.yuntaijiaju.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bb.wgjwhj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kp.yuexingan06.cn

[L06] 解析响应为 JSON
来源：http://za.colortex.cn

Py:   resp.json()
来源：http://gj.szsharing.cn

PHP:  json_decode($body, true);
来源：http://tx.shxzskj.cn

JS:   await resp.json()
来源：http://bw.nszjky.cn

TS:   await resp.json()
来源：http://uh.asd995.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cn.szsharing.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zx.yuntaijiaju.cn

Ruby: JSON.parse(resp.body)
来源：http://ni.hnjuh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rp.asd995.cn

[L07] 处理 HTTP 状态码
来源：http://sj.chemitech.net.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vf.muxihuayi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://oq.panjiajie.cn

JS:   resp.ok;  resp.status
来源：http://qk.panjiajie.cn

TS:   resp.ok;  resp.status
来源：http://wy.bookmarksfly.cn

Java: resp.statusCode()
来源：http://pj.asd995.cn

Go:   resp.StatusCode
来源：http://ud.jctech888.com.cn

Ruby: resp.code.to_i
来源：http://vd.newstarts.cn

C#:   (int)resp.StatusCode
来源：http://oy.yuntaijiaju.cn

[L08] 并发请求多个地址
来源：http://cs.newstarts.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xp.newstarts.cn

PHP:  curl_multi_init() 系列
来源：http://ar.bjjhwx.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uz.bjjhwx.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aa.jctech888.com.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sf.huixinmuqiang.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vl.jianghongdianzi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mi.9csxet.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nc.hahajie.cn

================================================================================
来源：http://lp.asd995.cn

M. 命令行 / 进程 / 环境
来源：http://tr.wgjwhj.cn

================================================================================
来源：http://jg.asd995.cn

[M01] 读取命令行参数
来源：http://bj.haigaiapp.cn

Py:   sys.argv[1:]
来源：http://mb.shxzskj.cn

PHP:  $argv;  $argc;
来源：http://oa.yuntaijiaju.cn

JS:   process.argv.slice(2)
来源：http://ck.gzmigu.cn

TS:   process.argv.slice(2)
来源：http://zs.colortex.cn

Java: args 数组（main 方法参数）
来源：http://tk.bjjhwx.cn

Go:   os.Args[1:]
来源：http://tl.newstarts.cn

Ruby: ARGV
来源：http://as.shxzukj.cn

C#:   args 数组（Main 方法参数）
来源：http://wx.huanxung.cn

[M02] 读取环境变量
来源：http://hv.bookmarksfly.cn

Py:   os.environ.get("HOME")
来源：http://ez.huixiangedu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ap.nicolike.cn

JS:   process.env.HOME
来源：http://dp.bookmarksfly.cn

TS:   process.env.HOME
来源：http://aa.shxzukj.cn

Java: System.getenv("HOME")
来源：http://jl.wgjwhj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kr.wgjwhj.cn

Ruby: ENV["HOME"]
来源：http://mi.huanxung.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wh.chemitech.net.cn

[M03] 执行外部命令
来源：http://pr.chemitech.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rv.gzmigu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jn.huanxung.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ya.9csxet.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fe.shxzskj.cn


<!-- 参考信息 -->