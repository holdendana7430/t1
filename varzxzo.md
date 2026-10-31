代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mk.huixiangedu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uo.hahajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yq.huixiangedu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rb.panjiajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://we.huixiangedu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ik.shtwfgs.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://co.jctech888.com.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://is.colortex.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jf.huixinmuqiang.cn

[I07] 忽略大小写与多行模式
来源：http://lp.huixinmuqiang.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hk.haigaiapp.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hj.jianghongdianzi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ri.gzmigu.cn

TS:   /error/gim
来源：http://gm.lnxyls.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dh.jianghongdianzi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xb.lnxyls.cn

Ruby: s.scan(/error/i)
来源：http://fv.shxzukj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mc.szsharing.cn

[I08] 贪婪与非贪婪匹配
来源：http://ym.jianghongdianzi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ec.shxzukj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zf.huixinmuqiang.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fh.nszjky.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uk.yuntaijiaju.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qk.huanxung.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://za.szsharing.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xf.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jn.lnxyls.cn

================================================================================
来源：http://nn.shxzskj.cn

J. 日期与时间
来源：http://sf.nicolike.cn

================================================================================
来源：http://jf.yuexingan06.cn

[J01] 获取当前时间
来源：http://fn.bjjhwx.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://eu.haigaiapp.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ze.hahajie.cn

JS:   new Date();  Date.now()
来源：http://hn.panjiajie.cn

TS:   new Date();  Date.now()
来源：http://sr.bookmarksfly.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yu.huixiangedu.cn

Go:   time.Now()
来源：http://bp.chemitech.net.cn

Ruby: Time.now
来源：http://pa.yuntaijiaju.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kh.wgjwhj.cn

[J02] 格式化输出
来源：http://zf.muxihuayi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://en.gzmigu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yd.huanxung.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://la.jianghongdianzi.cn

TS:   d.toISOString()
来源：http://fx.521024.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pn.521024.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gt.huixiangedu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ub.shxzskj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pb.shtwfgs.cn

[J03] 字符串解析为日期
来源：http://iu.huixinmuqiang.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://df.bjjhwx.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://te.bookmarksfly.cn

JS:   new Date("2024-01-02")
来源：http://hv.szxytkj.cn

TS:   new Date("2024-01-02")
来源：http://qf.yuntaijiaju.cn

Java: LocalDate.parse("2024-01-02")
来源：http://se.szsharing.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ec.newstarts.cn

Ruby: Date.parse("2024-01-02")
来源：http://xl.newstarts.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ji.yuexingan06.cn

[J04] 时间戳与日期互转
来源：http://ch.521024.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qh.yuexingan06.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zr.colortex.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hu.wgjwhj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://uz.yuexingan06.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xe.gzmigu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ci.nszjky.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://as.szxytkj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mx.wgjwhj.cn

[J05] 时间加减（加 7 天）
来源：http://ls.shtwfgs.cn

Py:   now + timedelta(days=7)
来源：http://vm.asd995.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://hc.jctech888.com.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://il.521024.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://oa.9csxet.cn

Java: LocalDate.now().plusDays(7)
来源：http://ne.hahajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://su.yuexingan06.cn

Ruby: Time.now + 7 * 86400
来源：http://hd.chemitech.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://no.szxytkj.cn

[J06] 计算两时间之差
来源：http://er.yuntaijiaju.cn

Py:   (end - start).total_seconds()
来源：http://qw.haigaiapp.cn

PHP:  $end->diff($start)->days;
来源：http://wb.newstarts.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vd.szxytkj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://td.gzmigu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rr.colortex.cn

Go:   end.Sub(start).Hours()
来源：http://ap.jianghongdianzi.cn

Ruby: end - start                 # 返回秒数
来源：http://kq.bjjhwx.cn

C#:   (end - start).TotalSeconds
来源：http://ic.hnjuh.cn

[J07] 比较两个日期
来源：http://gq.haigaiapp.cn

Py:   d1 < d2;  d1 == d2
来源：http://rd.gzmigu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ul.lnxyls.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bz.bjjhwx.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vy.hnjuh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://at.muxihuayi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vb.shxzskj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ek.hnjuh.cn

C#:   d1 < d2;  d1 == d2
来源：http://sa.gzmigu.cn

[J08] 提取年月日与星期
来源：http://pt.newstarts.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fw.shxzskj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tv.muxihuayi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rl.shxzukj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vg.chemitech.net.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mw.szxytkj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://oh.asd995.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yq.huixinmuqiang.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fn.panjiajie.cn

[J09] 时区处理
来源：http://kb.hahajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zs.huanxung.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yv.huanxung.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ib.huanxung.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fn.9csxet.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://it.nszjky.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hn.bookmarksfly.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jj.shtwfgs.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tc.chemitech.net.cn

[J10] 取今天 / 本月第一天
来源：http://vm.521024.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zz.521024.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fb.szsharing.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wx.hnjuh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ln.chemitech.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kp.yuexingan06.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tx.huanxung.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hw.wgjwhj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bk.yuntaijiaju.cn

================================================================================
来源：http://zl.haigaiapp.cn

K. JSON 与序列化
来源：http://hk.panjiajie.cn

================================================================================
来源：http://fi.muxihuayi.cn

[K01] 对象转 JSON 字符串
来源：http://xg.newstarts.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mk.wgjwhj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://sx.shxzskj.cn

JS:   JSON.stringify(obj)
来源：http://lc.bookmarksfly.cn

TS:   JSON.stringify(obj)
来源：http://jj.jianghongdianzi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mk.shxzukj.cn

Go:   json.Marshal(obj)
来源：http://lz.yuexingan06.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cl.hnjuh.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://uo.jctech888.com.cn

[K02] JSON 字符串转对象
来源：http://zj.newstarts.cn

Py:   json.loads(s)
来源：http://vs.jianghongdianzi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ki.szsharing.cn

JS:   JSON.parse(s)
来源：http://qe.asd995.cn

TS:   JSON.parse(s)
来源：http://hn.lnxyls.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zc.nszjky.cn

Go:   json.Unmarshal(data, &v)
来源：http://mc.newstarts.cn

Ruby: JSON.parse(s)
来源：http://cw.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tx.colortex.cn

[K03] JSON 美化输出（带缩进）
来源：http://jr.shtwfgs.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ar.newstarts.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fu.hnjuh.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hh.yuexingan06.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yq.9csxet.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kj.chemitech.net.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vk.wgjwhj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bd.colortex.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jl.huixinmuqiang.cn

[K04] 读取 JSON 文件
来源：http://md.huanxung.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xy.shtwfgs.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qf.lnxyls.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xk.hahajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cn.haigaiapp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nc.521024.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://om.shtwfgs.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://lz.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zw.shxzukj.cn

[K05] 深拷贝对象
来源：http://jr.nicolike.cn

Py:   copy.deepcopy(obj)
来源：http://zu.szxytkj.cn

PHP:  unserialize(serialize($obj));
来源：http://aq.jctech888.com.cn

JS:   structuredClone(obj)
来源：http://ls.panjiajie.cn

TS:   structuredClone(obj)
来源：http://fg.colortex.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gl.shxzukj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qy.colortex.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://me.lnxyls.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mf.haigaiapp.cn

[K06] 解析 URL 查询串
来源：http://xp.521024.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://br.huixiangedu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hg.colortex.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vr.shxzukj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hq.wgjwhj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://np.jianghongdianzi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://kd.9csxet.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sg.szxytkj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://st.panjiajie.cn

[K07] 进制转换
来源：http://yh.nicolike.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qi.shxzukj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nm.shxzukj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yh.szsharing.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vr.bookmarksfly.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uw.huixinmuqiang.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yr.panjiajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ss.yuexingan06.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vn.hnjuh.cn

[K08] 二进制序列化（非 JSON）
来源：http://pf.shxzukj.cn

Py:   pickle.dumps(obj)
来源：http://lc.szxytkj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://jc.wgjwhj.cn

JS:   v8.serialize(obj)        // Node
来源：http://bv.gzmigu.cn

TS:   v8.serialize(obj)        // Node
来源：http://kz.shtwfgs.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cd.wgjwhj.cn

Go:   encoding/gob
来源：http://bl.521024.cn

Ruby: Marshal.dump(obj)
来源：http://nk.shxzskj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ow.haigaiapp.cn

================================================================================
来源：http://lz.bjjhwx.cn

L. 网络请求
来源：http://kf.panjiajie.cn

================================================================================
来源：http://hb.521024.cn

[L01] 发送 GET 请求
来源：http://qy.szxytkj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fi.hahajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zh.asd995.cn

JS:   await fetch(url)
来源：http://ou.hnjuh.cn

TS:   await fetch(url)
来源：http://vo.colortex.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uj.9csxet.cn

Go:   resp, err := http.Get(url)
来源：http://pa.nicolike.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xt.huanxung.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xc.shxzskj.cn

[L02] 发送 POST JSON
来源：http://ua.521024.cn

Py:   requests.post(url, json={"a": 1})
来源：http://af.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sl.521024.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pb.asd995.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hw.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wr.jianghongdianzi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rf.yuntaijiaju.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ep.colortex.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gs.nicolike.cn

[L03] 设置自定义请求头
来源：http://sf.chemitech.net.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fz.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xm.bjjhwx.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vo.muxihuayi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qy.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ft.9csxet.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://we.colortex.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gr.huixiangedu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ou.bjjhwx.cn

[L04] 设置超时
来源：http://jw.newstarts.cn

Py:   requests.get(url, timeout=5)
来源：http://sy.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zq.yuntaijiaju.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ax.hahajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hb.bjjhwx.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ft.huixinmuqiang.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wo.muxihuayi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zm.9csxet.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fz.yuntaijiaju.cn

[L05] 上传文件（multipart）
来源：http://up.huixinmuqiang.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zq.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jv.shxzskj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vk.hahajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://us.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cn.521024.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nb.hnjuh.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kh.newstarts.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ae.huanxung.cn

[L06] 解析响应为 JSON
来源：http://yk.colortex.cn

Py:   resp.json()
来源：http://dr.szxytkj.cn

PHP:  json_decode($body, true);
来源：http://ne.bookmarksfly.cn

JS:   await resp.json()
来源：http://yc.haigaiapp.cn

TS:   await resp.json()
来源：http://cd.nszjky.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dj.chemitech.net.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vu.hnjuh.cn

Ruby: JSON.parse(resp.body)
来源：http://vf.haigaiapp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://an.shxzskj.cn

[L07] 处理 HTTP 状态码
来源：http://xu.jianghongdianzi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xe.huixiangedu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ox.szxytkj.cn

JS:   resp.ok;  resp.status
来源：http://al.haigaiapp.cn

TS:   resp.ok;  resp.status
来源：http://ax.panjiajie.cn

Java: resp.statusCode()
来源：http://pz.huanxung.cn

Go:   resp.StatusCode
来源：http://pl.colortex.cn

Ruby: resp.code.to_i
来源：http://fb.bookmarksfly.cn

C#:   (int)resp.StatusCode
来源：http://wo.panjiajie.cn

[L08] 并发请求多个地址
来源：http://nm.newstarts.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ie.hahajie.cn

PHP:  curl_multi_init() 系列
来源：http://ag.chemitech.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ma.shtwfgs.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fi.shxzskj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ig.muxihuayi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hi.hnjuh.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://aj.wgjwhj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://or.bjjhwx.cn

================================================================================
来源：http://ze.jctech888.com.cn

M. 命令行 / 进程 / 环境
来源：http://sb.gzmigu.cn

================================================================================
来源：http://wq.yuexingan06.cn

[M01] 读取命令行参数
来源：http://sq.muxihuayi.cn

Py:   sys.argv[1:]
来源：http://ug.wgjwhj.cn

PHP:  $argv;  $argc;
来源：http://ad.bjjhwx.cn

JS:   process.argv.slice(2)
来源：http://pa.yuexingan06.cn

TS:   process.argv.slice(2)
来源：http://vt.hahajie.cn

Java: args 数组（main 方法参数）
来源：http://bk.shtwfgs.cn

Go:   os.Args[1:]
来源：http://ju.asd995.cn

Ruby: ARGV
来源：http://tn.jianghongdianzi.cn

C#:   args 数组（Main 方法参数）
来源：http://ew.colortex.cn

[M02] 读取环境变量
来源：http://ky.9csxet.cn

Py:   os.environ.get("HOME")
来源：http://rq.yuntaijiaju.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uz.nszjky.cn

JS:   process.env.HOME
来源：http://nj.wgjwhj.cn

TS:   process.env.HOME
来源：http://in.haigaiapp.cn

Java: System.getenv("HOME")
来源：http://vm.panjiajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cn.colortex.cn

Ruby: ENV["HOME"]
来源：http://xv.nicolike.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uk.wgjwhj.cn

[M03] 执行外部命令
来源：http://ns.jctech888.com.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ed.chemitech.net.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cb.wgjwhj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://tc.shxzukj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wl.colortex.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bp.lnxyls.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://no.hnjuh.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pr.nicolike.cn

C#:   Process.Start("ls", "-l");
来源：http://qq.lnxyls.cn


<!-- 参考信息 -->