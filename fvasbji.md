代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ld.yuexingan06.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pw.bookmarksfly.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://eb.hnjuh.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://td.chemitech.net.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wd.huixiangedu.cn

[I07] 忽略大小写与多行模式
来源：http://fz.panjiajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xs.muxihuayi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lu.hnjuh.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rx.huixinmuqiang.cn

TS:   /error/gim
来源：http://mw.nszjky.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ri.nicolike.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ru.nicolike.cn

Ruby: s.scan(/error/i)
来源：http://di.shxzskj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nb.chemitech.net.cn

[I08] 贪婪与非贪婪匹配
来源：http://kj.huanxung.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://oq.newstarts.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qr.hnjuh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://el.hnjuh.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qi.huixiangedu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bm.huixiangedu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pp.nicolike.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qn.shxzukj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qq.muxihuayi.cn

================================================================================
来源：http://mz.haigaiapp.cn

J. 日期与时间
来源：http://mw.521024.cn

================================================================================
来源：http://ey.huixiangedu.cn

[J01] 获取当前时间
来源：http://ms.newstarts.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://nh.nicolike.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yu.bjjhwx.cn

JS:   new Date();  Date.now()
来源：http://kv.bjjhwx.cn

TS:   new Date();  Date.now()
来源：http://vf.hahajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ul.521024.cn

Go:   time.Now()
来源：http://qb.huanxung.cn

Ruby: Time.now
来源：http://nh.szsharing.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kd.muxihuayi.cn

[J02] 格式化输出
来源：http://vn.huixiangedu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://av.521024.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fg.huixiangedu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://av.newstarts.cn

TS:   d.toISOString()
来源：http://yx.shxzskj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lq.colortex.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qt.panjiajie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zs.asd995.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vo.colortex.cn

[J03] 字符串解析为日期
来源：http://ck.panjiajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wr.shxzskj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ew.shtwfgs.cn

JS:   new Date("2024-01-02")
来源：http://db.szsharing.cn

TS:   new Date("2024-01-02")
来源：http://rb.nicolike.cn

Java: LocalDate.parse("2024-01-02")
来源：http://eo.haigaiapp.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nh.haigaiapp.cn

Ruby: Date.parse("2024-01-02")
来源：http://oq.9csxet.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tg.huixinmuqiang.cn

[J04] 时间戳与日期互转
来源：http://pr.panjiajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qo.lnxyls.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kn.nicolike.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tc.521024.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vx.panjiajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mk.asd995.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lj.huixinmuqiang.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://et.haigaiapp.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://eo.gzmigu.cn

[J05] 时间加减（加 7 天）
来源：http://mj.muxihuayi.cn

Py:   now + timedelta(days=7)
来源：http://ih.shxzskj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wv.wgjwhj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://od.shxzskj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lc.nicolike.cn

Java: LocalDate.now().plusDays(7)
来源：http://ls.nszjky.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://my.521024.cn

Ruby: Time.now + 7 * 86400
来源：http://ft.jctech888.com.cn

C#:   DateTime.Now.AddDays(7)
来源：http://dk.gzmigu.cn

[J06] 计算两时间之差
来源：http://nf.shxzukj.cn

Py:   (end - start).total_seconds()
来源：http://yh.shtwfgs.cn

PHP:  $end->diff($start)->days;
来源：http://ay.nicolike.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ib.bjjhwx.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gk.yuntaijiaju.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ii.shxzukj.cn

Go:   end.Sub(start).Hours()
来源：http://yd.newstarts.cn

Ruby: end - start                 # 返回秒数
来源：http://ei.hnjuh.cn

C#:   (end - start).TotalSeconds
来源：http://qa.521024.cn

[J07] 比较两个日期
来源：http://mh.yuntaijiaju.cn

Py:   d1 < d2;  d1 == d2
来源：http://pw.muxihuayi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gz.yuexingan06.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gg.asd995.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jr.bookmarksfly.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sg.hnjuh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ej.nszjky.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zj.szxytkj.cn

C#:   d1 < d2;  d1 == d2
来源：http://le.yuexingan06.cn

[J08] 提取年月日与星期
来源：http://zu.newstarts.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://va.newstarts.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rv.shtwfgs.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ac.bjjhwx.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yo.nicolike.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tm.bookmarksfly.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fm.huixiangedu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qn.521024.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ct.asd995.cn

[J09] 时区处理
来源：http://zj.hahajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ek.panjiajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ps.bookmarksfly.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fc.jianghongdianzi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ox.newstarts.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ab.lnxyls.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://se.9csxet.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://re.chemitech.net.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rj.nicolike.cn

[J10] 取今天 / 本月第一天
来源：http://gu.huixinmuqiang.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://os.haigaiapp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lz.jianghongdianzi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yi.panjiajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tc.panjiajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ni.jianghongdianzi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vu.haigaiapp.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cb.colortex.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xb.jctech888.com.cn

================================================================================
来源：http://tp.huixinmuqiang.cn

K. JSON 与序列化
来源：http://fj.wgjwhj.cn

================================================================================
来源：http://je.hnjuh.cn

[K01] 对象转 JSON 字符串
来源：http://pe.jianghongdianzi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ub.521024.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://or.9csxet.cn

JS:   JSON.stringify(obj)
来源：http://tb.huixinmuqiang.cn

TS:   JSON.stringify(obj)
来源：http://wu.yuntaijiaju.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ag.yuntaijiaju.cn

Go:   json.Marshal(obj)
来源：http://wa.lnxyls.cn

Ruby: obj.to_json                                     // require "json"
来源：http://up.9csxet.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://oq.bookmarksfly.cn

[K02] JSON 字符串转对象
来源：http://ql.muxihuayi.cn

Py:   json.loads(s)
来源：http://gj.wgjwhj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://si.huixiangedu.cn

JS:   JSON.parse(s)
来源：http://kc.nszjky.cn

TS:   JSON.parse(s)
来源：http://vb.asd995.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uv.bookmarksfly.cn

Go:   json.Unmarshal(data, &v)
来源：http://qj.szxytkj.cn

Ruby: JSON.parse(s)
来源：http://qo.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kk.newstarts.cn

[K03] JSON 美化输出（带缩进）
来源：http://xk.hahajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://el.9csxet.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fl.yuntaijiaju.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kb.newstarts.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://te.9csxet.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pk.shxzukj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gg.yuntaijiaju.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pf.hahajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gl.colortex.cn

[K04] 读取 JSON 文件
来源：http://pt.szxytkj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ho.bjjhwx.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://un.shxzukj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://su.muxihuayi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fn.nicolike.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qk.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ow.muxihuayi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fn.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://aa.yuntaijiaju.cn

[K05] 深拷贝对象
来源：http://qu.shxzskj.cn

Py:   copy.deepcopy(obj)
来源：http://gy.jianghongdianzi.cn

PHP:  unserialize(serialize($obj));
来源：http://zh.panjiajie.cn

JS:   structuredClone(obj)
来源：http://xh.newstarts.cn

TS:   structuredClone(obj)
来源：http://mo.newstarts.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://an.shxzukj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rl.jctech888.com.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zz.asd995.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ra.panjiajie.cn

[K06] 解析 URL 查询串
来源：http://vs.muxihuayi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lx.shtwfgs.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jd.huixiangedu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vm.chemitech.net.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yj.muxihuayi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ay.szxytkj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://co.wgjwhj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ow.shtwfgs.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ez.szxytkj.cn

[K07] 进制转换
来源：http://xd.chemitech.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mg.panjiajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mv.panjiajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bj.newstarts.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qf.shtwfgs.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tz.nicolike.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qb.jctech888.com.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vd.szxytkj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zv.hnjuh.cn

[K08] 二进制序列化（非 JSON）
来源：http://ah.colortex.cn

Py:   pickle.dumps(obj)
来源：http://kx.jianghongdianzi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ys.wgjwhj.cn

JS:   v8.serialize(obj)        // Node
来源：http://wt.521024.cn

TS:   v8.serialize(obj)        // Node
来源：http://yk.newstarts.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://iq.huanxung.cn

Go:   encoding/gob
来源：http://tq.yuntaijiaju.cn

Ruby: Marshal.dump(obj)
来源：http://ju.asd995.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vc.nszjky.cn

================================================================================
来源：http://yl.asd995.cn

L. 网络请求
来源：http://zi.shtwfgs.cn

================================================================================
来源：http://sp.bookmarksfly.cn

[L01] 发送 GET 请求
来源：http://xw.colortex.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bg.9csxet.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://eb.shtwfgs.cn

JS:   await fetch(url)
来源：http://aq.huanxung.cn

TS:   await fetch(url)
来源：http://ox.bjjhwx.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ch.asd995.cn

Go:   resp, err := http.Get(url)
来源：http://ql.shxzskj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://na.newstarts.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://br.shxzskj.cn

[L02] 发送 POST JSON
来源：http://rr.lnxyls.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vj.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ql.521024.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fg.chemitech.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ze.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ar.muxihuayi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jk.huixiangedu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://od.chemitech.net.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.shtwfgs.cn

[L03] 设置自定义请求头
来源：http://sf.jianghongdianzi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sq.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qa.newstarts.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ap.yuexingan06.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wr.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qd.jianghongdianzi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rf.9csxet.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zd.huixiangedu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mc.yuexingan06.cn

[L04] 设置超时
来源：http://hq.wgjwhj.cn

Py:   requests.get(url, timeout=5)
来源：http://yq.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://te.asd995.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lc.szsharing.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ba.newstarts.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hm.huanxung.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ne.wgjwhj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ct.huanxung.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://to.haigaiapp.cn

[L05] 上传文件（multipart）
来源：http://cl.szxytkj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ot.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vq.9csxet.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yu.wgjwhj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sd.nicolike.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ia.asd995.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pe.chemitech.net.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qb.huixiangedu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fl.yuexingan06.cn

[L06] 解析响应为 JSON
来源：http://su.asd995.cn

Py:   resp.json()
来源：http://yg.bookmarksfly.cn

PHP:  json_decode($body, true);
来源：http://ym.huixiangedu.cn

JS:   await resp.json()
来源：http://zt.shtwfgs.cn

TS:   await resp.json()
来源：http://co.shxzskj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dq.lnxyls.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ci.nicolike.cn

Ruby: JSON.parse(resp.body)
来源：http://jd.panjiajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bu.colortex.cn

[L07] 处理 HTTP 状态码
来源：http://kp.huixinmuqiang.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lh.asd995.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mf.hnjuh.cn

JS:   resp.ok;  resp.status
来源：http://vf.shxzukj.cn

TS:   resp.ok;  resp.status
来源：http://bv.gzmigu.cn

Java: resp.statusCode()
来源：http://ro.521024.cn

Go:   resp.StatusCode
来源：http://mp.colortex.cn

Ruby: resp.code.to_i
来源：http://kb.nicolike.cn

C#:   (int)resp.StatusCode
来源：http://fq.muxihuayi.cn

[L08] 并发请求多个地址
来源：http://bv.wgjwhj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hs.huixiangedu.cn

PHP:  curl_multi_init() 系列
来源：http://ok.chemitech.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vh.szxytkj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nf.9csxet.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pr.nicolike.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mg.jianghongdianzi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yl.huixiangedu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ua.huanxung.cn

================================================================================
来源：http://bu.9csxet.cn

M. 命令行 / 进程 / 环境
来源：http://vs.nicolike.cn

================================================================================
来源：http://wv.shtwfgs.cn

[M01] 读取命令行参数
来源：http://cc.shtwfgs.cn

Py:   sys.argv[1:]
来源：http://do.bjjhwx.cn

PHP:  $argv;  $argc;
来源：http://cz.gzmigu.cn

JS:   process.argv.slice(2)
来源：http://bk.newstarts.cn

TS:   process.argv.slice(2)
来源：http://nz.jctech888.com.cn

Java: args 数组（main 方法参数）
来源：http://tb.huanxung.cn

Go:   os.Args[1:]
来源：http://zu.shxzukj.cn

Ruby: ARGV
来源：http://ww.nicolike.cn

C#:   args 数组（Main 方法参数）
来源：http://ty.hnjuh.cn

[M02] 读取环境变量
来源：http://mc.yuexingan06.cn

Py:   os.environ.get("HOME")
来源：http://bs.gzmigu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ru.hnjuh.cn

JS:   process.env.HOME
来源：http://ju.huixinmuqiang.cn

TS:   process.env.HOME
来源：http://oj.jianghongdianzi.cn

Java: System.getenv("HOME")
来源：http://mh.521024.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hv.muxihuayi.cn

Ruby: ENV["HOME"]
来源：http://jx.gzmigu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hx.bjjhwx.cn

[M03] 执行外部命令
来源：http://dz.lnxyls.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zi.huixinmuqiang.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zj.chemitech.net.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://aw.newstarts.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pn.haigaiapp.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tq.huanxung.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ia.wgjwhj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ft.521024.cn

C#:   Process.Start("ls", "-l");
来源：http://co.szsharing.cn

[M04] 获取当前工作目录
来源：http://xk.newstarts.cn

Py:   os.getcwd()
来源：http://mi.colortex.cn

PHP:  getcwd();
来源：http://zp.521024.cn

JS:   process.cwd()
来源：http://sq.szxytkj.cn


<!-- 参考信息 -->