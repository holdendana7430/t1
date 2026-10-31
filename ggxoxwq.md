代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vy.huixinmuqiang.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bq.wgjwhj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xw.nicolike.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ow.panjiajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hs.hnjuh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pa.szsharing.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hx.newstarts.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nx.bjjhwx.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://va.521024.cn

[I07] 忽略大小写与多行模式
来源：http://me.jctech888.com.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pg.shxzukj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uz.yuntaijiaju.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cu.panjiajie.cn

TS:   /error/gim
来源：http://rb.huixinmuqiang.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ca.yuntaijiaju.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ji.hahajie.cn

Ruby: s.scan(/error/i)
来源：http://hp.huanxung.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uv.lnxyls.cn

[I08] 贪婪与非贪婪匹配
来源：http://re.bookmarksfly.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jc.bookmarksfly.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kg.panjiajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ij.jctech888.com.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uc.nicolike.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bd.lnxyls.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cm.hahajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ec.hahajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jk.wgjwhj.cn

================================================================================
来源：http://pc.lnxyls.cn

J. 日期与时间
来源：http://br.521024.cn

================================================================================
来源：http://at.9csxet.cn

[J01] 获取当前时间
来源：http://hp.huanxung.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://od.hnjuh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xh.panjiajie.cn

JS:   new Date();  Date.now()
来源：http://fa.shxzukj.cn

TS:   new Date();  Date.now()
来源：http://ir.lnxyls.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://iz.huanxung.cn

Go:   time.Now()
来源：http://kq.yuexingan06.cn

Ruby: Time.now
来源：http://py.jctech888.com.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hb.shtwfgs.cn

[J02] 格式化输出
来源：http://dz.hahajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uz.panjiajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sb.jctech888.com.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ks.nicolike.cn

TS:   d.toISOString()
来源：http://gx.bjjhwx.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sg.hnjuh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ut.asd995.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sx.colortex.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hp.gzmigu.cn

[J03] 字符串解析为日期
来源：http://qr.szsharing.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qy.haigaiapp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://om.nszjky.cn

JS:   new Date("2024-01-02")
来源：http://mi.jianghongdianzi.cn

TS:   new Date("2024-01-02")
来源：http://zm.bookmarksfly.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pb.wgjwhj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://oc.szxytkj.cn

Ruby: Date.parse("2024-01-02")
来源：http://tf.szxytkj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gl.huixiangedu.cn

[J04] 时间戳与日期互转
来源：http://fj.gzmigu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vz.shxzukj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vt.shxzukj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xc.newstarts.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tp.huanxung.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xg.hnjuh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nn.jianghongdianzi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qc.panjiajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pl.newstarts.cn

[J05] 时间加减（加 7 天）
来源：http://zm.shxzskj.cn

Py:   now + timedelta(days=7)
来源：http://lu.muxihuayi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ch.asd995.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fc.huixiangedu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xt.shxzskj.cn

Java: LocalDate.now().plusDays(7)
来源：http://ev.muxihuayi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://je.shxzukj.cn

Ruby: Time.now + 7 * 86400
来源：http://gv.bjjhwx.cn

C#:   DateTime.Now.AddDays(7)
来源：http://oi.asd995.cn

[J06] 计算两时间之差
来源：http://qi.shxzskj.cn

Py:   (end - start).total_seconds()
来源：http://ic.shtwfgs.cn

PHP:  $end->diff($start)->days;
来源：http://fl.newstarts.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ef.yuexingan06.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zl.hahajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://av.hnjuh.cn

Go:   end.Sub(start).Hours()
来源：http://fq.521024.cn

Ruby: end - start                 # 返回秒数
来源：http://gu.yuexingan06.cn

C#:   (end - start).TotalSeconds
来源：http://zu.yuexingan06.cn

[J07] 比较两个日期
来源：http://qy.jianghongdianzi.cn

Py:   d1 < d2;  d1 == d2
来源：http://oa.jianghongdianzi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://my.yuexingan06.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kd.shxzukj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xo.bookmarksfly.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qq.hnjuh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yh.huixiangedu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ko.yuntaijiaju.cn

C#:   d1 < d2;  d1 == d2
来源：http://hz.lnxyls.cn

[J08] 提取年月日与星期
来源：http://cg.huanxung.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hf.shxzukj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xt.hahajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://oi.wgjwhj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://da.nicolike.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://eu.huixiangedu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dx.szsharing.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zm.shxzskj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pr.yuexingan06.cn

[J09] 时区处理
来源：http://iw.yuexingan06.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mm.hnjuh.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ti.yuntaijiaju.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xe.hahajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mz.haigaiapp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gw.521024.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://em.lnxyls.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hg.yuexingan06.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ep.haigaiapp.cn

[J10] 取今天 / 本月第一天
来源：http://hl.huixinmuqiang.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://za.gzmigu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kc.nszjky.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://da.newstarts.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bt.521024.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hf.9csxet.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xm.haigaiapp.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://os.yuntaijiaju.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gc.nszjky.cn

================================================================================
来源：http://qf.yuntaijiaju.cn

K. JSON 与序列化
来源：http://ul.nicolike.cn

================================================================================
来源：http://wg.bjjhwx.cn

[K01] 对象转 JSON 字符串
来源：http://gf.haigaiapp.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nx.521024.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ip.newstarts.cn

JS:   JSON.stringify(obj)
来源：http://qu.jctech888.com.cn

TS:   JSON.stringify(obj)
来源：http://bt.521024.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ur.shxzukj.cn

Go:   json.Marshal(obj)
来源：http://ve.hahajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://su.hahajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lu.bookmarksfly.cn

[K02] JSON 字符串转对象
来源：http://tp.nszjky.cn

Py:   json.loads(s)
来源：http://qh.newstarts.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nc.szsharing.cn

JS:   JSON.parse(s)
来源：http://ib.yuexingan06.cn

TS:   JSON.parse(s)
来源：http://zn.hahajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://or.huixiangedu.cn

Go:   json.Unmarshal(data, &v)
来源：http://ws.huixiangedu.cn

Ruby: JSON.parse(s)
来源：http://fe.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mu.colortex.cn

[K03] JSON 美化输出（带缩进）
来源：http://al.chemitech.net.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://or.bjjhwx.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ua.huanxung.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://mb.haigaiapp.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://at.bookmarksfly.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hk.bjjhwx.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nw.nszjky.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ko.huanxung.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ag.yuntaijiaju.cn

[K04] 读取 JSON 文件
来源：http://pj.shxzskj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nh.chemitech.net.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sv.huixinmuqiang.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zj.colortex.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tq.shxzukj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ev.shxzukj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ec.newstarts.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://lw.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mn.asd995.cn

[K05] 深拷贝对象
来源：http://vu.huanxung.cn

Py:   copy.deepcopy(obj)
来源：http://zp.chemitech.net.cn

PHP:  unserialize(serialize($obj));
来源：http://ao.huixiangedu.cn

JS:   structuredClone(obj)
来源：http://oz.jctech888.com.cn

TS:   structuredClone(obj)
来源：http://bq.bjjhwx.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rx.panjiajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mj.muxihuayi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zl.lnxyls.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xp.jctech888.com.cn

[K06] 解析 URL 查询串
来源：http://rt.newstarts.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zu.nicolike.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://to.yuexingan06.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xi.shtwfgs.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dc.9csxet.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mw.nicolike.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mu.hahajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oc.lnxyls.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nq.nszjky.cn

[K07] 进制转换
来源：http://cg.9csxet.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ja.hnjuh.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ok.asd995.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://us.nicolike.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://oe.yuntaijiaju.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://id.nszjky.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nl.shxzskj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mj.yuexingan06.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vp.jctech888.com.cn

[K08] 二进制序列化（非 JSON）
来源：http://vs.lnxyls.cn

Py:   pickle.dumps(obj)
来源：http://am.haigaiapp.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://jd.huixinmuqiang.cn

JS:   v8.serialize(obj)        // Node
来源：http://ik.lnxyls.cn

TS:   v8.serialize(obj)        // Node
来源：http://wh.wgjwhj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kl.newstarts.cn

Go:   encoding/gob
来源：http://tp.newstarts.cn

Ruby: Marshal.dump(obj)
来源：http://jn.asd995.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zq.lnxyls.cn

================================================================================
来源：http://gc.shtwfgs.cn

L. 网络请求
来源：http://zc.colortex.cn

================================================================================
来源：http://rd.jianghongdianzi.cn

[L01] 发送 GET 请求
来源：http://ux.521024.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://de.chemitech.net.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://js.yuexingan06.cn

JS:   await fetch(url)
来源：http://uu.bjjhwx.cn

TS:   await fetch(url)
来源：http://dc.bookmarksfly.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kt.asd995.cn

Go:   resp, err := http.Get(url)
来源：http://eg.szxytkj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gv.gzmigu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jk.nszjky.cn

[L02] 发送 POST JSON
来源：http://rq.521024.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vy.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://va.521024.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bk.asd995.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zy.colortex.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fy.yuexingan06.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pu.hnjuh.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sp.shtwfgs.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rd.jctech888.com.cn

[L03] 设置自定义请求头
来源：http://vp.wgjwhj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mv.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dw.huixinmuqiang.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ro.521024.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zd.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jo.szxytkj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rs.szxytkj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ho.szxytkj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jo.shxzukj.cn

[L04] 设置超时
来源：http://lf.gzmigu.cn

Py:   requests.get(url, timeout=5)
来源：http://lj.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gf.muxihuayi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rd.521024.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://si.newstarts.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://of.shtwfgs.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://io.shxzukj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ug.gzmigu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://py.shtwfgs.cn

[L05] 上传文件（multipart）
来源：http://lf.521024.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xz.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xo.jctech888.com.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hn.haigaiapp.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ps.haigaiapp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://df.bookmarksfly.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uw.nszjky.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bs.huanxung.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://go.shtwfgs.cn

[L06] 解析响应为 JSON
来源：http://ru.gzmigu.cn

Py:   resp.json()
来源：http://sv.newstarts.cn

PHP:  json_decode($body, true);
来源：http://ms.asd995.cn

JS:   await resp.json()
来源：http://lb.gzmigu.cn

TS:   await resp.json()
来源：http://zp.bookmarksfly.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rw.huixiangedu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tm.bookmarksfly.cn

Ruby: JSON.parse(resp.body)
来源：http://km.haigaiapp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ub.huanxung.cn

[L07] 处理 HTTP 状态码
来源：http://la.muxihuayi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://et.nicolike.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ch.panjiajie.cn

JS:   resp.ok;  resp.status
来源：http://ab.shxzskj.cn

TS:   resp.ok;  resp.status
来源：http://cq.hahajie.cn

Java: resp.statusCode()
来源：http://zr.newstarts.cn

Go:   resp.StatusCode
来源：http://zq.szsharing.cn

Ruby: resp.code.to_i
来源：http://uu.newstarts.cn

C#:   (int)resp.StatusCode
来源：http://jz.panjiajie.cn

[L08] 并发请求多个地址
来源：http://ys.hahajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kg.hnjuh.cn

PHP:  curl_multi_init() 系列
来源：http://oz.huanxung.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hm.nszjky.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bc.shtwfgs.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dm.jctech888.com.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tg.9csxet.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cd.bookmarksfly.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ew.szsharing.cn

================================================================================
来源：http://ur.hahajie.cn

M. 命令行 / 进程 / 环境
来源：http://vd.newstarts.cn

================================================================================
来源：http://os.szsharing.cn

[M01] 读取命令行参数
来源：http://lk.nszjky.cn

Py:   sys.argv[1:]
来源：http://qk.muxihuayi.cn

PHP:  $argv;  $argc;
来源：http://nv.szxytkj.cn

JS:   process.argv.slice(2)
来源：http://fo.9csxet.cn

TS:   process.argv.slice(2)
来源：http://py.shxzukj.cn

Java: args 数组（main 方法参数）
来源：http://fb.huixinmuqiang.cn

Go:   os.Args[1:]
来源：http://ts.hnjuh.cn

Ruby: ARGV
来源：http://zf.szxytkj.cn

C#:   args 数组（Main 方法参数）
来源：http://tk.haigaiapp.cn

[M02] 读取环境变量
来源：http://cv.521024.cn

Py:   os.environ.get("HOME")
来源：http://zz.wgjwhj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ha.jctech888.com.cn

JS:   process.env.HOME
来源：http://py.hnjuh.cn

TS:   process.env.HOME
来源：http://in.nszjky.cn

Java: System.getenv("HOME")
来源：http://fu.muxihuayi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bo.bookmarksfly.cn

Ruby: ENV["HOME"]
来源：http://hc.521024.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zj.nszjky.cn

[M03] 执行外部命令
来源：http://kg.shtwfgs.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dx.hahajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qa.shtwfgs.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ij.yuntaijiaju.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tn.chemitech.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ha.huanxung.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://sf.bookmarksfly.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xe.haigaiapp.cn

C#:   Process.Start("ls", "-l");
来源：http://wp.nicolike.cn


<!-- 参考信息 -->