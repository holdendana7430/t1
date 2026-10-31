代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://fq.huanxung.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ay.wgjwhj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nf.bookmarksfly.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xq.newstarts.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://te.nicolike.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://af.huanxung.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yi.shxzukj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xa.shxzskj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ls.lnxyls.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jv.bookmarksfly.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tx.chemitech.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wt.huixinmuqiang.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yb.nszjky.cn

[I07] 忽略大小写与多行模式
来源：http://if.hnjuh.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rv.newstarts.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://an.huanxung.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ql.szxytkj.cn

TS:   /error/gim
来源：http://gh.9csxet.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uq.huixiangedu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xo.panjiajie.cn

Ruby: s.scan(/error/i)
来源：http://ys.nszjky.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bn.hnjuh.cn

[I08] 贪婪与非贪婪匹配
来源：http://kl.yuntaijiaju.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jm.haigaiapp.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ln.bookmarksfly.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cp.huixinmuqiang.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://un.yuexingan06.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wo.521024.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gf.szsharing.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uz.chemitech.net.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qc.yuexingan06.cn

================================================================================
来源：http://mv.panjiajie.cn

J. 日期与时间
来源：http://jy.haigaiapp.cn

================================================================================
来源：http://vz.hnjuh.cn

[J01] 获取当前时间
来源：http://bl.yuexingan06.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://dq.lnxyls.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fz.panjiajie.cn

JS:   new Date();  Date.now()
来源：http://ps.shtwfgs.cn

TS:   new Date();  Date.now()
来源：http://gx.colortex.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://cr.colortex.cn

Go:   time.Now()
来源：http://ea.huixiangedu.cn

Ruby: Time.now
来源：http://pv.huanxung.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ya.muxihuayi.cn

[J02] 格式化输出
来源：http://vr.szxytkj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ss.521024.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tq.szxytkj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ux.nszjky.cn

TS:   d.toISOString()
来源：http://cw.bjjhwx.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ux.szsharing.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rn.yuexingan06.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://od.hnjuh.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xp.colortex.cn

[J03] 字符串解析为日期
来源：http://tu.nszjky.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yr.chemitech.net.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pm.panjiajie.cn

JS:   new Date("2024-01-02")
来源：http://dq.bjjhwx.cn

TS:   new Date("2024-01-02")
来源：http://zo.huanxung.cn

Java: LocalDate.parse("2024-01-02")
来源：http://di.yuexingan06.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vy.yuntaijiaju.cn

Ruby: Date.parse("2024-01-02")
来源：http://nx.huanxung.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cr.9csxet.cn

[J04] 时间戳与日期互转
来源：http://cz.nszjky.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lm.huixiangedu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://im.szsharing.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ic.muxihuayi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://yn.haigaiapp.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xy.shxzskj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lj.shtwfgs.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vo.szsharing.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lu.jctech888.com.cn

[J05] 时间加减（加 7 天）
来源：http://om.szsharing.cn

Py:   now + timedelta(days=7)
来源：http://sh.panjiajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://gd.hnjuh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://oc.newstarts.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pm.shxzukj.cn

Java: LocalDate.now().plusDays(7)
来源：http://cy.shtwfgs.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kb.shtwfgs.cn

Ruby: Time.now + 7 * 86400
来源：http://kr.bookmarksfly.cn

C#:   DateTime.Now.AddDays(7)
来源：http://lt.yuexingan06.cn

[J06] 计算两时间之差
来源：http://mk.panjiajie.cn

Py:   (end - start).total_seconds()
来源：http://pd.yuntaijiaju.cn

PHP:  $end->diff($start)->days;
来源：http://uh.panjiajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kk.gzmigu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yo.colortex.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ic.bjjhwx.cn

Go:   end.Sub(start).Hours()
来源：http://ah.szxytkj.cn

Ruby: end - start                 # 返回秒数
来源：http://ep.bookmarksfly.cn

C#:   (end - start).TotalSeconds
来源：http://xd.huanxung.cn

[J07] 比较两个日期
来源：http://yd.haigaiapp.cn

Py:   d1 < d2;  d1 == d2
来源：http://kb.szsharing.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ua.nicolike.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ci.colortex.cn

TS:   d1.getTime() < d2.getTime()
来源：http://nd.panjiajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cb.bjjhwx.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gw.chemitech.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ff.colortex.cn

C#:   d1 < d2;  d1 == d2
来源：http://um.gzmigu.cn

[J08] 提取年月日与星期
来源：http://ad.huixiangedu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dh.bjjhwx.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ze.wgjwhj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wu.wgjwhj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cg.asd995.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://et.colortex.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nh.bjjhwx.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zg.lnxyls.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bd.szsharing.cn

[J09] 时区处理
来源：http://oc.huanxung.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://aj.asd995.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fh.szxytkj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aq.yuntaijiaju.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tn.panjiajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fv.gzmigu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cr.shxzukj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://nx.panjiajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xg.wgjwhj.cn

[J10] 取今天 / 本月第一天
来源：http://hh.huixinmuqiang.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fa.hnjuh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://an.jianghongdianzi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xa.shxzukj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zq.jianghongdianzi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hq.nszjky.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qp.hahajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://in.yuntaijiaju.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lo.szsharing.cn

================================================================================
来源：http://az.9csxet.cn

K. JSON 与序列化
来源：http://di.szsharing.cn

================================================================================
来源：http://lf.huanxung.cn

[K01] 对象转 JSON 字符串
来源：http://zu.wgjwhj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mf.colortex.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ng.huixinmuqiang.cn

JS:   JSON.stringify(obj)
来源：http://ln.gzmigu.cn

TS:   JSON.stringify(obj)
来源：http://qh.9csxet.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kj.szxytkj.cn

Go:   json.Marshal(obj)
来源：http://xo.9csxet.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bq.szsharing.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fz.hahajie.cn

[K02] JSON 字符串转对象
来源：http://wh.szsharing.cn

Py:   json.loads(s)
来源：http://ro.nicolike.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://et.colortex.cn

JS:   JSON.parse(s)
来源：http://ir.shxzukj.cn

TS:   JSON.parse(s)
来源：http://nl.huixinmuqiang.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ev.nszjky.cn

Go:   json.Unmarshal(data, &v)
来源：http://ui.yuexingan06.cn

Ruby: JSON.parse(s)
来源：http://gj.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rn.nicolike.cn

[K03] JSON 美化输出（带缩进）
来源：http://yo.hnjuh.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yv.haigaiapp.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hg.asd995.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hi.hahajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wt.lnxyls.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ya.bookmarksfly.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dr.szsharing.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qm.9csxet.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ra.huixinmuqiang.cn

[K04] 读取 JSON 文件
来源：http://xj.nszjky.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://us.hnjuh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://em.gzmigu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://va.jctech888.com.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ar.bookmarksfly.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://en.asd995.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ue.nszjky.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gd.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tf.gzmigu.cn

[K05] 深拷贝对象
来源：http://jn.nszjky.cn

Py:   copy.deepcopy(obj)
来源：http://et.haigaiapp.cn

PHP:  unserialize(serialize($obj));
来源：http://qv.yuntaijiaju.cn

JS:   structuredClone(obj)
来源：http://us.shxzukj.cn

TS:   structuredClone(obj)
来源：http://da.shxzskj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ln.yuntaijiaju.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nj.colortex.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yc.nicolike.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ai.shxzskj.cn

[K06] 解析 URL 查询串
来源：http://dm.shxzukj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mf.nicolike.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wk.hahajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ef.gzmigu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://da.szsharing.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ok.shxzskj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sw.wgjwhj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fr.newstarts.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ta.panjiajie.cn

[K07] 进制转换
来源：http://jl.chemitech.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vh.shtwfgs.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sa.521024.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ge.colortex.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rt.jianghongdianzi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://du.haigaiapp.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ne.hahajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mw.wgjwhj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nr.szsharing.cn

[K08] 二进制序列化（非 JSON）
来源：http://in.shtwfgs.cn

Py:   pickle.dumps(obj)
来源：http://wi.szxytkj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ef.huixinmuqiang.cn

JS:   v8.serialize(obj)        // Node
来源：http://ew.huixinmuqiang.cn

TS:   v8.serialize(obj)        // Node
来源：http://zz.bookmarksfly.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cm.bjjhwx.cn

Go:   encoding/gob
来源：http://kw.gzmigu.cn

Ruby: Marshal.dump(obj)
来源：http://tm.yuntaijiaju.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ki.shxzskj.cn

================================================================================
来源：http://fo.huixiangedu.cn

L. 网络请求
来源：http://hw.muxihuayi.cn

================================================================================
来源：http://si.asd995.cn

[L01] 发送 GET 请求
来源：http://mi.yuexingan06.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xn.asd995.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hl.yuexingan06.cn

JS:   await fetch(url)
来源：http://px.gzmigu.cn

TS:   await fetch(url)
来源：http://rf.panjiajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://if.newstarts.cn

Go:   resp, err := http.Get(url)
来源：http://oc.asd995.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://om.9csxet.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rx.521024.cn

[L02] 发送 POST JSON
来源：http://tr.shxzukj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://si.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bq.521024.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://td.jianghongdianzi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hh.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ov.wgjwhj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sl.haigaiapp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xk.jctech888.com.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yq.shtwfgs.cn

[L03] 设置自定义请求头
来源：http://gg.huanxung.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ie.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uh.shxzskj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fk.szsharing.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://su.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lq.panjiajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jl.shxzukj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gb.colortex.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fo.colortex.cn

[L04] 设置超时
来源：http://mw.huixiangedu.cn

Py:   requests.get(url, timeout=5)
来源：http://dy.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ai.huixiangedu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://um.521024.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zx.gzmigu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jh.hnjuh.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hj.jctech888.com.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sy.asd995.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xg.wgjwhj.cn

[L05] 上传文件（multipart）
来源：http://fe.huixiangedu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ul.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hx.haigaiapp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xb.colortex.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qv.bjjhwx.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://la.colortex.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mu.panjiajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nd.shxzskj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jq.lnxyls.cn

[L06] 解析响应为 JSON
来源：http://to.szsharing.cn

Py:   resp.json()
来源：http://ax.wgjwhj.cn

PHP:  json_decode($body, true);
来源：http://jk.lnxyls.cn

JS:   await resp.json()
来源：http://yz.asd995.cn

TS:   await resp.json()
来源：http://fn.asd995.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://go.yuntaijiaju.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ct.hnjuh.cn

Ruby: JSON.parse(resp.body)
来源：http://if.colortex.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lb.panjiajie.cn

[L07] 处理 HTTP 状态码
来源：http://yq.shxzskj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ty.lnxyls.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fk.huanxung.cn

JS:   resp.ok;  resp.status
来源：http://qs.bookmarksfly.cn

TS:   resp.ok;  resp.status
来源：http://rl.huanxung.cn

Java: resp.statusCode()
来源：http://qn.asd995.cn

Go:   resp.StatusCode
来源：http://pg.wgjwhj.cn

Ruby: resp.code.to_i
来源：http://ei.shxzukj.cn

C#:   (int)resp.StatusCode
来源：http://hr.szsharing.cn

[L08] 并发请求多个地址
来源：http://ll.newstarts.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hd.shtwfgs.cn

PHP:  curl_multi_init() 系列
来源：http://mr.jctech888.com.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dl.jctech888.com.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sm.muxihuayi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bk.jctech888.com.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://um.shxzukj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://re.jianghongdianzi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dk.szsharing.cn

================================================================================
来源：http://jw.jianghongdianzi.cn

M. 命令行 / 进程 / 环境
来源：http://gt.huixiangedu.cn

================================================================================
来源：http://xw.muxihuayi.cn

[M01] 读取命令行参数
来源：http://ge.newstarts.cn

Py:   sys.argv[1:]
来源：http://gs.haigaiapp.cn

PHP:  $argv;  $argc;
来源：http://xw.hahajie.cn

JS:   process.argv.slice(2)
来源：http://fb.panjiajie.cn

TS:   process.argv.slice(2)
来源：http://yu.muxihuayi.cn

Java: args 数组（main 方法参数）
来源：http://bi.huixiangedu.cn

Go:   os.Args[1:]
来源：http://gp.bookmarksfly.cn

Ruby: ARGV
来源：http://jw.panjiajie.cn

C#:   args 数组（Main 方法参数）
来源：http://lm.shxzukj.cn

[M02] 读取环境变量
来源：http://bg.huanxung.cn

Py:   os.environ.get("HOME")
来源：http://gy.huixinmuqiang.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rx.newstarts.cn

JS:   process.env.HOME
来源：http://bj.nszjky.cn

TS:   process.env.HOME
来源：http://lk.hnjuh.cn

Java: System.getenv("HOME")
来源：http://la.jctech888.com.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qo.panjiajie.cn

Ruby: ENV["HOME"]
来源：http://vp.chemitech.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gb.wgjwhj.cn

[M03] 执行外部命令
来源：http://dv.panjiajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tq.hnjuh.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bf.asd995.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://mk.hnjuh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yx.9csxet.cn


<!-- 参考信息 -->