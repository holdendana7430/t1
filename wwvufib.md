代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ly.shxzukj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gi.nszjky.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ax.huixiangedu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dw.chemitech.net.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vl.bookmarksfly.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pl.gzmigu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jj.lnxyls.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rm.huixiangedu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bu.521024.cn

[I07] 忽略大小写与多行模式
来源：http://no.muxihuayi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ah.huixiangedu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ea.9csxet.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sw.521024.cn

TS:   /error/gim
来源：http://zi.shtwfgs.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://er.yuexingan06.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jj.colortex.cn

Ruby: s.scan(/error/i)
来源：http://qc.huixinmuqiang.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xe.wgjwhj.cn

[I08] 贪婪与非贪婪匹配
来源：http://tn.gzmigu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ou.huixinmuqiang.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sa.panjiajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xy.newstarts.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yg.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ru.chemitech.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lu.jianghongdianzi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://sn.gzmigu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nb.yuntaijiaju.cn

================================================================================
来源：http://sm.jctech888.com.cn

J. 日期与时间
来源：http://nm.huanxung.cn

================================================================================
来源：http://qm.bookmarksfly.cn

[J01] 获取当前时间
来源：http://cu.gzmigu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fd.hnjuh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bh.panjiajie.cn

JS:   new Date();  Date.now()
来源：http://zs.jctech888.com.cn

TS:   new Date();  Date.now()
来源：http://ob.szsharing.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ob.shxzskj.cn

Go:   time.Now()
来源：http://fp.wgjwhj.cn

Ruby: Time.now
来源：http://fv.nszjky.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gq.huixiangedu.cn

[J02] 格式化输出
来源：http://ox.9csxet.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://as.bookmarksfly.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tu.hnjuh.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qj.521024.cn

TS:   d.toISOString()
来源：http://vm.shtwfgs.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vc.hnjuh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sf.bjjhwx.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gv.szxytkj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lg.yuexingan06.cn

[J03] 字符串解析为日期
来源：http://tk.hnjuh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yl.wgjwhj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tg.bjjhwx.cn

JS:   new Date("2024-01-02")
来源：http://ng.hnjuh.cn

TS:   new Date("2024-01-02")
来源：http://jm.gzmigu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gh.haigaiapp.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://be.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://ac.szxytkj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jw.lnxyls.cn

[J04] 时间戳与日期互转
来源：http://ht.nicolike.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ul.hnjuh.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wh.nszjky.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://as.asd995.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ip.gzmigu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qs.gzmigu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ti.yuexingan06.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yz.muxihuayi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yr.lnxyls.cn

[J05] 时间加减（加 7 天）
来源：http://rr.huixiangedu.cn

Py:   now + timedelta(days=7)
来源：http://cl.shxzskj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nv.huixinmuqiang.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wh.haigaiapp.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gp.shxzskj.cn

Java: LocalDate.now().plusDays(7)
来源：http://yy.haigaiapp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fn.521024.cn

Ruby: Time.now + 7 * 86400
来源：http://vv.nszjky.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zn.bookmarksfly.cn

[J06] 计算两时间之差
来源：http://ti.nszjky.cn

Py:   (end - start).total_seconds()
来源：http://we.panjiajie.cn

PHP:  $end->diff($start)->days;
来源：http://jx.huanxung.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cq.szxytkj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kf.chemitech.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://if.szsharing.cn

Go:   end.Sub(start).Hours()
来源：http://qp.haigaiapp.cn

Ruby: end - start                 # 返回秒数
来源：http://vf.jianghongdianzi.cn

C#:   (end - start).TotalSeconds
来源：http://ay.asd995.cn

[J07] 比较两个日期
来源：http://pc.9csxet.cn

Py:   d1 < d2;  d1 == d2
来源：http://kw.asd995.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mc.nszjky.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ag.521024.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bj.yuntaijiaju.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qp.chemitech.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fa.yuexingan06.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lr.hnjuh.cn

C#:   d1 < d2;  d1 == d2
来源：http://rt.panjiajie.cn

[J08] 提取年月日与星期
来源：http://ve.wgjwhj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ot.yuntaijiaju.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zh.jctech888.com.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rw.newstarts.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ch.szsharing.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gn.haigaiapp.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ki.9csxet.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mx.panjiajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nk.lnxyls.cn

[J09] 时区处理
来源：http://ol.shtwfgs.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hv.chemitech.net.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yn.bookmarksfly.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ka.muxihuayi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hq.nszjky.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://te.bjjhwx.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zh.nszjky.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ge.bookmarksfly.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lf.asd995.cn

[J10] 取今天 / 本月第一天
来源：http://ow.bjjhwx.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kf.huixiangedu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mw.wgjwhj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jm.szsharing.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pz.shtwfgs.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nu.jctech888.com.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ha.huanxung.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pc.haigaiapp.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fq.haigaiapp.cn

================================================================================
来源：http://os.jctech888.com.cn

K. JSON 与序列化
来源：http://qz.bookmarksfly.cn

================================================================================
来源：http://ea.panjiajie.cn

[K01] 对象转 JSON 字符串
来源：http://wh.chemitech.net.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vh.szxytkj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://eh.huanxung.cn

JS:   JSON.stringify(obj)
来源：http://nl.muxihuayi.cn

TS:   JSON.stringify(obj)
来源：http://im.yuexingan06.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://iv.szxytkj.cn

Go:   json.Marshal(obj)
来源：http://xr.shxzskj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bg.hnjuh.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fb.521024.cn

[K02] JSON 字符串转对象
来源：http://ce.shxzukj.cn

Py:   json.loads(s)
来源：http://qh.huixinmuqiang.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vy.bookmarksfly.cn

JS:   JSON.parse(s)
来源：http://ti.asd995.cn

TS:   JSON.parse(s)
来源：http://zr.nicolike.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kh.asd995.cn

Go:   json.Unmarshal(data, &v)
来源：http://fm.521024.cn

Ruby: JSON.parse(s)
来源：http://ng.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://st.shtwfgs.cn

[K03] JSON 美化输出（带缩进）
来源：http://mz.asd995.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mj.panjiajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sj.bjjhwx.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://za.szsharing.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xq.szxytkj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qz.jctech888.com.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jj.yuexingan06.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xn.colortex.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bc.nszjky.cn

[K04] 读取 JSON 文件
来源：http://xz.chemitech.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tf.haigaiapp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nm.shxzukj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pg.gzmigu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mm.shxzskj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zf.colortex.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ho.shxzukj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ng.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://se.panjiajie.cn

[K05] 深拷贝对象
来源：http://dc.521024.cn

Py:   copy.deepcopy(obj)
来源：http://ov.yuexingan06.cn

PHP:  unserialize(serialize($obj));
来源：http://og.huixiangedu.cn

JS:   structuredClone(obj)
来源：http://lq.hnjuh.cn

TS:   structuredClone(obj)
来源：http://qg.shxzskj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://en.9csxet.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gy.huixiangedu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lx.shtwfgs.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hf.colortex.cn

[K06] 解析 URL 查询串
来源：http://lk.jianghongdianzi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://au.yuntaijiaju.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pw.yuntaijiaju.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mo.gzmigu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ch.panjiajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ne.shxzukj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wb.szxytkj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pv.shxzskj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fe.shxzukj.cn

[K07] 进制转换
来源：http://ek.521024.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xw.shtwfgs.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tl.yuexingan06.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yr.jctech888.com.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vy.hahajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nx.hnjuh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tf.hahajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kj.shxzskj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://eh.muxihuayi.cn

[K08] 二进制序列化（非 JSON）
来源：http://fh.shxzukj.cn

Py:   pickle.dumps(obj)
来源：http://bc.bjjhwx.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pj.haigaiapp.cn

JS:   v8.serialize(obj)        // Node
来源：http://rs.shxzukj.cn

TS:   v8.serialize(obj)        // Node
来源：http://hh.521024.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dn.yuntaijiaju.cn

Go:   encoding/gob
来源：http://tb.huixinmuqiang.cn

Ruby: Marshal.dump(obj)
来源：http://bt.chemitech.net.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ky.chemitech.net.cn

================================================================================
来源：http://fp.9csxet.cn

L. 网络请求
来源：http://ak.panjiajie.cn

================================================================================
来源：http://uk.wgjwhj.cn

[L01] 发送 GET 请求
来源：http://ab.panjiajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sd.asd995.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ra.bookmarksfly.cn

JS:   await fetch(url)
来源：http://gj.9csxet.cn

TS:   await fetch(url)
来源：http://cm.huanxung.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dg.nicolike.cn

Go:   resp, err := http.Get(url)
来源：http://tl.bookmarksfly.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fb.gzmigu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nc.chemitech.net.cn

[L02] 发送 POST JSON
来源：http://qa.521024.cn

Py:   requests.post(url, json={"a": 1})
来源：http://un.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uz.newstarts.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uo.shtwfgs.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fa.asd995.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lp.panjiajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ii.nicolike.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dg.asd995.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bl.colortex.cn

[L03] 设置自定义请求头
来源：http://qg.szxytkj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hq.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zi.panjiajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fu.panjiajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xy.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ew.haigaiapp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ld.chemitech.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://id.jctech888.com.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yx.newstarts.cn

[L04] 设置超时
来源：http://yv.yuntaijiaju.cn

Py:   requests.get(url, timeout=5)
来源：http://ti.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ot.asd995.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wp.newstarts.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ga.huanxung.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vz.newstarts.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ge.hahajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fz.asd995.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ou.hnjuh.cn

[L05] 上传文件（multipart）
来源：http://sh.yuexingan06.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vr.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xz.newstarts.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bg.bjjhwx.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ti.hahajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ud.lnxyls.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ka.wgjwhj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xg.chemitech.net.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ka.huixiangedu.cn

[L06] 解析响应为 JSON
来源：http://xj.hahajie.cn

Py:   resp.json()
来源：http://jq.huixinmuqiang.cn

PHP:  json_decode($body, true);
来源：http://xp.hahajie.cn

JS:   await resp.json()
来源：http://de.yuexingan06.cn

TS:   await resp.json()
来源：http://hw.szsharing.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://iu.newstarts.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fc.asd995.cn

Ruby: JSON.parse(resp.body)
来源：http://cz.huixiangedu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dy.jctech888.com.cn

[L07] 处理 HTTP 状态码
来源：http://ck.shtwfgs.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zu.9csxet.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://up.hnjuh.cn

JS:   resp.ok;  resp.status
来源：http://dq.jctech888.com.cn

TS:   resp.ok;  resp.status
来源：http://lj.hnjuh.cn

Java: resp.statusCode()
来源：http://hl.bjjhwx.cn

Go:   resp.StatusCode
来源：http://ez.asd995.cn

Ruby: resp.code.to_i
来源：http://sg.shtwfgs.cn

C#:   (int)resp.StatusCode
来源：http://rs.shxzskj.cn

[L08] 并发请求多个地址
来源：http://tq.colortex.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ol.hahajie.cn

PHP:  curl_multi_init() 系列
来源：http://uu.521024.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dv.bjjhwx.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cw.jctech888.com.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nz.hahajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://no.jctech888.com.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://if.bookmarksfly.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ng.szsharing.cn

================================================================================
来源：http://iq.9csxet.cn

M. 命令行 / 进程 / 环境
来源：http://bo.521024.cn

================================================================================
来源：http://mo.jianghongdianzi.cn

[M01] 读取命令行参数
来源：http://qt.panjiajie.cn

Py:   sys.argv[1:]
来源：http://pd.lnxyls.cn

PHP:  $argv;  $argc;
来源：http://ix.huixiangedu.cn

JS:   process.argv.slice(2)
来源：http://pf.bjjhwx.cn

TS:   process.argv.slice(2)
来源：http://gs.yuexingan06.cn

Java: args 数组（main 方法参数）
来源：http://em.wgjwhj.cn

Go:   os.Args[1:]
来源：http://rl.colortex.cn

Ruby: ARGV
来源：http://ge.shxzukj.cn

C#:   args 数组（Main 方法参数）
来源：http://hv.panjiajie.cn

[M02] 读取环境变量
来源：http://kj.colortex.cn

Py:   os.environ.get("HOME")
来源：http://bu.colortex.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hf.gzmigu.cn

JS:   process.env.HOME
来源：http://pj.shtwfgs.cn

TS:   process.env.HOME
来源：http://tc.shxzukj.cn

Java: System.getenv("HOME")
来源：http://ll.hahajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mj.newstarts.cn

Ruby: ENV["HOME"]
来源：http://wh.bjjhwx.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://no.colortex.cn

[M03] 执行外部命令
来源：http://gq.huixinmuqiang.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ws.asd995.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gw.hahajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://it.chemitech.net.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://bg.yuexingan06.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wk.yuntaijiaju.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zm.shxzskj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rx.shxzskj.cn

C#:   Process.Start("ls", "-l");
来源：http://gb.521024.cn


<!-- 参考信息 -->