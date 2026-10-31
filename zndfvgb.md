代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://re.jianghongdianzi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nl.jctech888.com.cn

Ruby: s.split(/\s*,\s*/)
来源：http://oe.asd995.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gp.szxytkj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lk.yuexingan06.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kj.shtwfgs.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ia.jianghongdianzi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ir.panjiajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yd.huixiangedu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qj.shtwfgs.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sq.newstarts.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ho.yuexingan06.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qc.wgjwhj.cn

[I07] 忽略大小写与多行模式
来源：http://ym.huixinmuqiang.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qz.521024.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vb.jctech888.com.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://aq.yuexingan06.cn

TS:   /error/gim
来源：http://il.shxzukj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jf.nicolike.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vk.yuexingan06.cn

Ruby: s.scan(/error/i)
来源：http://qo.asd995.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qj.shtwfgs.cn

[I08] 贪婪与非贪婪匹配
来源：http://aw.hahajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ts.huixinmuqiang.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ej.bookmarksfly.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yu.jctech888.com.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yv.szsharing.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://iy.huixinmuqiang.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://iv.lnxyls.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://sl.colortex.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ep.9csxet.cn

================================================================================
来源：http://yk.haigaiapp.cn

J. 日期与时间
来源：http://tg.yuexingan06.cn

================================================================================
来源：http://mb.shtwfgs.cn

[J01] 获取当前时间
来源：http://dc.colortex.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ac.nicolike.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hd.asd995.cn

JS:   new Date();  Date.now()
来源：http://vg.bookmarksfly.cn

TS:   new Date();  Date.now()
来源：http://vd.haigaiapp.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tm.newstarts.cn

Go:   time.Now()
来源：http://qa.muxihuayi.cn

Ruby: Time.now
来源：http://pn.jctech888.com.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://oq.yuexingan06.cn

[J02] 格式化输出
来源：http://tg.jctech888.com.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sv.hahajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yo.wgjwhj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://be.nicolike.cn

TS:   d.toISOString()
来源：http://qq.nszjky.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vo.haigaiapp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sg.colortex.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qg.hnjuh.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://io.521024.cn

[J03] 字符串解析为日期
来源：http://ml.newstarts.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sw.wgjwhj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ch.newstarts.cn

JS:   new Date("2024-01-02")
来源：http://qm.jctech888.com.cn

TS:   new Date("2024-01-02")
来源：http://fo.bjjhwx.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ec.gzmigu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kf.shxzskj.cn

Ruby: Date.parse("2024-01-02")
来源：http://kt.huixiangedu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mj.yuntaijiaju.cn

[J04] 时间戳与日期互转
来源：http://hj.szsharing.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vv.521024.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wb.lnxyls.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ie.huanxung.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hn.yuntaijiaju.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yl.shtwfgs.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fz.nicolike.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uj.colortex.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mq.hnjuh.cn

[J05] 时间加减（加 7 天）
来源：http://pq.newstarts.cn

Py:   now + timedelta(days=7)
来源：http://fy.gzmigu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ec.shxzskj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cn.shtwfgs.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mw.newstarts.cn

Java: LocalDate.now().plusDays(7)
来源：http://tj.muxihuayi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qq.nszjky.cn

Ruby: Time.now + 7 * 86400
来源：http://cu.wgjwhj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://oh.bookmarksfly.cn

[J06] 计算两时间之差
来源：http://jk.nszjky.cn

Py:   (end - start).total_seconds()
来源：http://ui.szxytkj.cn

PHP:  $end->diff($start)->days;
来源：http://iq.jianghongdianzi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kt.lnxyls.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tg.chemitech.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://tn.bjjhwx.cn

Go:   end.Sub(start).Hours()
来源：http://ng.9csxet.cn

Ruby: end - start                 # 返回秒数
来源：http://vl.shxzskj.cn

C#:   (end - start).TotalSeconds
来源：http://ii.wgjwhj.cn

[J07] 比较两个日期
来源：http://yp.yuexingan06.cn

Py:   d1 < d2;  d1 == d2
来源：http://px.colortex.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rs.gzmigu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ba.wgjwhj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://db.muxihuayi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xn.lnxyls.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tj.521024.cn

Ruby: d1 < d2;  d1 == d2
来源：http://sg.nicolike.cn

C#:   d1 < d2;  d1 == d2
来源：http://jn.huanxung.cn

[J08] 提取年月日与星期
来源：http://jr.panjiajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yf.panjiajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://an.szxytkj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xk.muxihuayi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rw.muxihuayi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ij.521024.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bp.muxihuayi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hh.huixiangedu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://co.muxihuayi.cn

[J09] 时区处理
来源：http://tk.521024.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://io.wgjwhj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://on.huixiangedu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ns.nszjky.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ys.nicolike.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sq.gzmigu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ve.bookmarksfly.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://oj.szsharing.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dc.bjjhwx.cn

[J10] 取今天 / 本月第一天
来源：http://hm.huanxung.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cz.shtwfgs.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jo.asd995.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cp.panjiajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yh.asd995.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ar.yuexingan06.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sr.panjiajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zd.shtwfgs.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ry.shxzukj.cn

================================================================================
来源：http://xb.huixiangedu.cn

K. JSON 与序列化
来源：http://qu.huixinmuqiang.cn

================================================================================
来源：http://os.haigaiapp.cn

[K01] 对象转 JSON 字符串
来源：http://ic.szxytkj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cw.asd995.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cw.lnxyls.cn

JS:   JSON.stringify(obj)
来源：http://hj.szsharing.cn

TS:   JSON.stringify(obj)
来源：http://me.gzmigu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nu.shxzskj.cn

Go:   json.Marshal(obj)
来源：http://uh.9csxet.cn

Ruby: obj.to_json                                     // require "json"
来源：http://za.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://js.bjjhwx.cn

[K02] JSON 字符串转对象
来源：http://qz.gzmigu.cn

Py:   json.loads(s)
来源：http://vs.hnjuh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rz.colortex.cn

JS:   JSON.parse(s)
来源：http://kl.521024.cn

TS:   JSON.parse(s)
来源：http://ut.asd995.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kk.bjjhwx.cn

Go:   json.Unmarshal(data, &v)
来源：http://ye.szsharing.cn

Ruby: JSON.parse(s)
来源：http://pb.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://oq.huanxung.cn

[K03] JSON 美化输出（带缩进）
来源：http://zh.gzmigu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pe.huixiangedu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mm.szsharing.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://td.lnxyls.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fx.shxzskj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gs.shxzskj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fh.panjiajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nn.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kl.shxzskj.cn

[K04] 读取 JSON 文件
来源：http://nx.shxzskj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://iz.bjjhwx.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fd.shtwfgs.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ca.yuntaijiaju.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qy.szsharing.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yo.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lo.yuexingan06.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mv.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ou.yuexingan06.cn

[K05] 深拷贝对象
来源：http://bn.szsharing.cn

Py:   copy.deepcopy(obj)
来源：http://db.521024.cn

PHP:  unserialize(serialize($obj));
来源：http://qn.asd995.cn

JS:   structuredClone(obj)
来源：http://hl.521024.cn

TS:   structuredClone(obj)
来源：http://zd.jctech888.com.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ea.huixiangedu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://la.muxihuayi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ht.shtwfgs.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gl.yuexingan06.cn

[K06] 解析 URL 查询串
来源：http://dv.hahajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ct.nszjky.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pc.521024.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xw.shxzukj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yw.newstarts.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yd.muxihuayi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ac.hahajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lm.gzmigu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nu.yuntaijiaju.cn

[K07] 进制转换
来源：http://ng.hahajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lg.shxzukj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yw.newstarts.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cn.jctech888.com.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vg.muxihuayi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vg.szsharing.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://le.shxzskj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jm.yuntaijiaju.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://er.jctech888.com.cn

[K08] 二进制序列化（非 JSON）
来源：http://qo.haigaiapp.cn

Py:   pickle.dumps(obj)
来源：http://gr.huixiangedu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ir.panjiajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://zm.9csxet.cn

TS:   v8.serialize(obj)        // Node
来源：http://pu.shtwfgs.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uk.hahajie.cn

Go:   encoding/gob
来源：http://xk.panjiajie.cn

Ruby: Marshal.dump(obj)
来源：http://na.jctech888.com.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uh.jctech888.com.cn

================================================================================
来源：http://xf.muxihuayi.cn

L. 网络请求
来源：http://se.muxihuayi.cn

================================================================================
来源：http://gt.shtwfgs.cn

[L01] 发送 GET 请求
来源：http://yf.jctech888.com.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yk.hnjuh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vy.chemitech.net.cn

JS:   await fetch(url)
来源：http://nf.lnxyls.cn

TS:   await fetch(url)
来源：http://oh.521024.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sc.newstarts.cn

Go:   resp, err := http.Get(url)
来源：http://xp.colortex.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qj.yuntaijiaju.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yo.521024.cn

[L02] 发送 POST JSON
来源：http://ll.haigaiapp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ym.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jl.huanxung.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xj.nszjky.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fs.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cq.newstarts.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cy.szxytkj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ug.bookmarksfly.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tp.jianghongdianzi.cn

[L03] 设置自定义请求头
来源：http://cn.hnjuh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://km.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cz.newstarts.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zr.lnxyls.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ss.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://oj.panjiajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sg.9csxet.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kj.shtwfgs.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kn.szsharing.cn

[L04] 设置超时
来源：http://zx.huanxung.cn

Py:   requests.get(url, timeout=5)
来源：http://xn.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xx.bjjhwx.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lw.colortex.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://un.hahajie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gm.wgjwhj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hs.chemitech.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://os.9csxet.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://eh.yuexingan06.cn

[L05] 上传文件（multipart）
来源：http://ey.shxzskj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ya.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ht.shxzukj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bm.bookmarksfly.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sj.lnxyls.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kg.haigaiapp.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sa.yuntaijiaju.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ls.hahajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sy.shxzukj.cn

[L06] 解析响应为 JSON
来源：http://cf.muxihuayi.cn

Py:   resp.json()
来源：http://xn.haigaiapp.cn

PHP:  json_decode($body, true);
来源：http://na.shxzukj.cn

JS:   await resp.json()
来源：http://eb.wgjwhj.cn

TS:   await resp.json()
来源：http://xe.huixiangedu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bi.colortex.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xw.lnxyls.cn

Ruby: JSON.parse(resp.body)
来源：http://ti.bjjhwx.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ne.haigaiapp.cn

[L07] 处理 HTTP 状态码
来源：http://zn.colortex.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lk.521024.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yn.nicolike.cn

JS:   resp.ok;  resp.status
来源：http://bm.huixinmuqiang.cn

TS:   resp.ok;  resp.status
来源：http://sd.bookmarksfly.cn

Java: resp.statusCode()
来源：http://nv.huixiangedu.cn

Go:   resp.StatusCode
来源：http://xa.huixiangedu.cn

Ruby: resp.code.to_i
来源：http://ig.shxzskj.cn

C#:   (int)resp.StatusCode
来源：http://sh.muxihuayi.cn

[L08] 并发请求多个地址
来源：http://jk.huixinmuqiang.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zo.yuntaijiaju.cn

PHP:  curl_multi_init() 系列
来源：http://bc.asd995.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bg.shxzskj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ix.gzmigu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lr.nszjky.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fm.szsharing.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tk.chemitech.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lg.bjjhwx.cn

================================================================================
来源：http://ld.huixiangedu.cn

M. 命令行 / 进程 / 环境
来源：http://wu.yuntaijiaju.cn

================================================================================
来源：http://ge.panjiajie.cn

[M01] 读取命令行参数
来源：http://uo.panjiajie.cn

Py:   sys.argv[1:]
来源：http://wy.yuexingan06.cn

PHP:  $argv;  $argc;
来源：http://zg.shxzukj.cn

JS:   process.argv.slice(2)
来源：http://av.bookmarksfly.cn

TS:   process.argv.slice(2)
来源：http://gf.shtwfgs.cn

Java: args 数组（main 方法参数）
来源：http://we.jctech888.com.cn

Go:   os.Args[1:]
来源：http://gx.haigaiapp.cn

Ruby: ARGV
来源：http://rg.9csxet.cn

C#:   args 数组（Main 方法参数）
来源：http://xz.huixinmuqiang.cn

[M02] 读取环境变量
来源：http://mh.huixinmuqiang.cn

Py:   os.environ.get("HOME")
来源：http://rp.szsharing.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gu.hnjuh.cn

JS:   process.env.HOME
来源：http://ft.521024.cn

TS:   process.env.HOME
来源：http://mp.asd995.cn

Java: System.getenv("HOME")
来源：http://bo.gzmigu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sx.shtwfgs.cn

Ruby: ENV["HOME"]
来源：http://xp.hnjuh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hq.szxytkj.cn

[M03] 执行外部命令
来源：http://xx.szsharing.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://on.shxzukj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kg.colortex.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ah.bjjhwx.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zo.jianghongdianzi.cn


<!-- 参考信息 -->