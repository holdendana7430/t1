代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sk.521024.cn

[I07] 忽略大小写与多行模式
来源：http://ey.521024.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ga.muxihuayi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vd.lnxyls.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lf.chemitech.net.cn

TS:   /error/gim
来源：http://xj.jianghongdianzi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lj.bjjhwx.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vu.chemitech.net.cn

Ruby: s.scan(/error/i)
来源：http://ao.bjjhwx.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pk.muxihuayi.cn

[I08] 贪婪与非贪婪匹配
来源：http://ku.szxytkj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yf.colortex.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ye.gzmigu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ae.jianghongdianzi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fg.hahajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://rl.chemitech.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hn.yuexingan06.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vo.shtwfgs.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fk.shxzskj.cn

================================================================================
来源：http://ip.bookmarksfly.cn

J. 日期与时间
来源：http://jp.521024.cn

================================================================================
来源：http://xn.szxytkj.cn

[J01] 获取当前时间
来源：http://sy.shxzukj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://tg.colortex.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zj.huixinmuqiang.cn

JS:   new Date();  Date.now()
来源：http://vy.szxytkj.cn

TS:   new Date();  Date.now()
来源：http://qo.yuntaijiaju.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fn.nicolike.cn

Go:   time.Now()
来源：http://ni.jianghongdianzi.cn

Ruby: Time.now
来源：http://df.wgjwhj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xg.nicolike.cn

[J02] 格式化输出
来源：http://js.huanxung.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wu.nicolike.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ah.hahajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fe.yuntaijiaju.cn

TS:   d.toISOString()
来源：http://af.panjiajie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qx.panjiajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kh.newstarts.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wk.jctech888.com.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://og.jctech888.com.cn

[J03] 字符串解析为日期
来源：http://rk.hnjuh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ks.bookmarksfly.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rh.9csxet.cn

JS:   new Date("2024-01-02")
来源：http://ye.newstarts.cn

TS:   new Date("2024-01-02")
来源：http://vf.panjiajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ly.colortex.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://be.asd995.cn

Ruby: Date.parse("2024-01-02")
来源：http://ns.shtwfgs.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cp.szxytkj.cn

[J04] 时间戳与日期互转
来源：http://fv.shxzskj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xc.shxzskj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lo.huixinmuqiang.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qw.shxzskj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xg.jianghongdianzi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nt.muxihuayi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jx.shxzukj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pw.szxytkj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hf.yuntaijiaju.cn

[J05] 时间加减（加 7 天）
来源：http://zl.bookmarksfly.cn

Py:   now + timedelta(days=7)
来源：http://ya.9csxet.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qn.huixinmuqiang.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://if.yuntaijiaju.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dq.shxzskj.cn

Java: LocalDate.now().plusDays(7)
来源：http://vh.shtwfgs.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lf.lnxyls.cn

Ruby: Time.now + 7 * 86400
来源：http://ly.nicolike.cn

C#:   DateTime.Now.AddDays(7)
来源：http://lq.huixinmuqiang.cn

[J06] 计算两时间之差
来源：http://eo.shxzskj.cn

Py:   (end - start).total_seconds()
来源：http://tk.wgjwhj.cn

PHP:  $end->diff($start)->days;
来源：http://mi.jianghongdianzi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ku.shxzskj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qv.lnxyls.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jq.huanxung.cn

Go:   end.Sub(start).Hours()
来源：http://kl.panjiajie.cn

Ruby: end - start                 # 返回秒数
来源：http://ig.szxytkj.cn

C#:   (end - start).TotalSeconds
来源：http://yz.nicolike.cn

[J07] 比较两个日期
来源：http://lm.jianghongdianzi.cn

Py:   d1 < d2;  d1 == d2
来源：http://tr.yuexingan06.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cf.yuexingan06.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gz.nicolike.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ty.szsharing.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://at.lnxyls.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zl.chemitech.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pl.wgjwhj.cn

C#:   d1 < d2;  d1 == d2
来源：http://id.gzmigu.cn

[J08] 提取年月日与星期
来源：http://ij.panjiajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wg.hahajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uq.asd995.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vl.shtwfgs.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dl.shxzskj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hn.asd995.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://my.hnjuh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vq.nszjky.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bu.yuntaijiaju.cn

[J09] 时区处理
来源：http://rv.jctech888.com.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dg.szsharing.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ep.shtwfgs.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zq.szxytkj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vr.9csxet.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qo.szsharing.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nn.hahajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cp.hnjuh.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bh.haigaiapp.cn

[J10] 取今天 / 本月第一天
来源：http://vf.bookmarksfly.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://dg.gzmigu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sn.yuexingan06.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ut.szsharing.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vp.yuexingan06.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mp.colortex.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sq.huixinmuqiang.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vl.szsharing.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ou.panjiajie.cn

================================================================================
来源：http://gp.jianghongdianzi.cn

K. JSON 与序列化
来源：http://fy.yuntaijiaju.cn

================================================================================
来源：http://ww.shtwfgs.cn

[K01] 对象转 JSON 字符串
来源：http://om.hnjuh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://au.asd995.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bk.szxytkj.cn

JS:   JSON.stringify(obj)
来源：http://ay.szsharing.cn

TS:   JSON.stringify(obj)
来源：http://lj.huixinmuqiang.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qj.bjjhwx.cn

Go:   json.Marshal(obj)
来源：http://gm.newstarts.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qq.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ts.huanxung.cn

[K02] JSON 字符串转对象
来源：http://tq.bookmarksfly.cn

Py:   json.loads(s)
来源：http://on.wgjwhj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nh.gzmigu.cn

JS:   JSON.parse(s)
来源：http://ui.chemitech.net.cn

TS:   JSON.parse(s)
来源：http://nt.nicolike.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sm.521024.cn

Go:   json.Unmarshal(data, &v)
来源：http://gp.asd995.cn

Ruby: JSON.parse(s)
来源：http://un.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pw.jctech888.com.cn

[K03] JSON 美化输出（带缩进）
来源：http://qt.yuexingan06.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mq.521024.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ht.wgjwhj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ih.nszjky.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yh.bjjhwx.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ji.shxzskj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vk.szsharing.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ek.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ud.nszjky.cn

[K04] 读取 JSON 文件
来源：http://ig.wgjwhj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qo.nicolike.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://eh.yuexingan06.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tk.haigaiapp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uh.newstarts.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://os.huanxung.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tc.lnxyls.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://nl.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kq.9csxet.cn

[K05] 深拷贝对象
来源：http://ou.newstarts.cn

Py:   copy.deepcopy(obj)
来源：http://mz.muxihuayi.cn

PHP:  unserialize(serialize($obj));
来源：http://ch.nszjky.cn

JS:   structuredClone(obj)
来源：http://ft.szxytkj.cn

TS:   structuredClone(obj)
来源：http://ay.szxytkj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://yz.jctech888.com.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pw.gzmigu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jo.haigaiapp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mo.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://ig.9csxet.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://db.chemitech.net.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://we.haigaiapp.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qe.nszjky.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sm.9csxet.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fj.panjiajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://yv.jianghongdianzi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pm.shxzskj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bm.huixinmuqiang.cn

[K07] 进制转换
来源：http://gk.huanxung.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://in.bjjhwx.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tl.shxzukj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dr.yuntaijiaju.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://do.yuexingan06.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tq.bookmarksfly.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vl.shtwfgs.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rd.huanxung.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wz.gzmigu.cn

[K08] 二进制序列化（非 JSON）
来源：http://ia.hahajie.cn

Py:   pickle.dumps(obj)
来源：http://xb.panjiajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://em.asd995.cn

JS:   v8.serialize(obj)        // Node
来源：http://jw.lnxyls.cn

TS:   v8.serialize(obj)        // Node
来源：http://au.shxzukj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ub.521024.cn

Go:   encoding/gob
来源：http://jf.yuexingan06.cn

Ruby: Marshal.dump(obj)
来源：http://xe.gzmigu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dc.bjjhwx.cn

================================================================================
来源：http://nc.yuexingan06.cn

L. 网络请求
来源：http://oj.huixiangedu.cn

================================================================================
来源：http://np.shxzskj.cn

[L01] 发送 GET 请求
来源：http://lv.gzmigu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://iu.huanxung.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jv.521024.cn

JS:   await fetch(url)
来源：http://ne.wgjwhj.cn

TS:   await fetch(url)
来源：http://hj.asd995.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rw.szsharing.cn

Go:   resp, err := http.Get(url)
来源：http://zd.nszjky.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wg.huanxung.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bk.nicolike.cn

[L02] 发送 POST JSON
来源：http://ad.wgjwhj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vz.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ln.9csxet.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ip.9csxet.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mh.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jt.lnxyls.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zk.hahajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mt.huixiangedu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zk.huixinmuqiang.cn

[L03] 设置自定义请求头
来源：http://vt.huanxung.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lp.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wc.muxihuayi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nr.nicolike.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ty.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://au.muxihuayi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vt.jianghongdianzi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cc.nicolike.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://io.hnjuh.cn

[L04] 设置超时
来源：http://tc.gzmigu.cn

Py:   requests.get(url, timeout=5)
来源：http://og.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dz.jianghongdianzi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lc.gzmigu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mv.shxzskj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xc.chemitech.net.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dk.asd995.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sl.haigaiapp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ma.bookmarksfly.cn

[L05] 上传文件（multipart）
来源：http://kk.jianghongdianzi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gc.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hk.hnjuh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://aq.wgjwhj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://oi.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ar.wgjwhj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pq.szsharing.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vn.jianghongdianzi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tg.yuntaijiaju.cn

[L06] 解析响应为 JSON
来源：http://un.muxihuayi.cn

Py:   resp.json()
来源：http://ds.bookmarksfly.cn

PHP:  json_decode($body, true);
来源：http://ui.nszjky.cn

JS:   await resp.json()
来源：http://ig.shtwfgs.cn

TS:   await resp.json()
来源：http://vh.panjiajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jj.asd995.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pe.nszjky.cn

Ruby: JSON.parse(resp.body)
来源：http://bv.yuntaijiaju.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sa.panjiajie.cn

[L07] 处理 HTTP 状态码
来源：http://uf.hahajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gd.wgjwhj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lh.bookmarksfly.cn

JS:   resp.ok;  resp.status
来源：http://lt.muxihuayi.cn

TS:   resp.ok;  resp.status
来源：http://nr.szsharing.cn

Java: resp.statusCode()
来源：http://en.huixinmuqiang.cn

Go:   resp.StatusCode
来源：http://nn.hnjuh.cn

Ruby: resp.code.to_i
来源：http://am.521024.cn

C#:   (int)resp.StatusCode
来源：http://nq.hahajie.cn

[L08] 并发请求多个地址
来源：http://qu.shtwfgs.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sw.muxihuayi.cn

PHP:  curl_multi_init() 系列
来源：http://qk.szxytkj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tf.521024.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xv.muxihuayi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://in.shxzukj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bp.haigaiapp.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sw.9csxet.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://eh.gzmigu.cn

================================================================================
来源：http://am.lnxyls.cn

M. 命令行 / 进程 / 环境
来源：http://lt.bookmarksfly.cn

================================================================================
来源：http://xx.panjiajie.cn

[M01] 读取命令行参数
来源：http://er.jctech888.com.cn

Py:   sys.argv[1:]
来源：http://zq.hnjuh.cn

PHP:  $argv;  $argc;
来源：http://eg.hnjuh.cn

JS:   process.argv.slice(2)
来源：http://za.huixiangedu.cn

TS:   process.argv.slice(2)
来源：http://ot.asd995.cn

Java: args 数组（main 方法参数）
来源：http://qj.yuntaijiaju.cn

Go:   os.Args[1:]
来源：http://py.panjiajie.cn

Ruby: ARGV
来源：http://nh.huanxung.cn

C#:   args 数组（Main 方法参数）
来源：http://fz.szxytkj.cn

[M02] 读取环境变量
来源：http://ij.jianghongdianzi.cn

Py:   os.environ.get("HOME")
来源：http://ln.huanxung.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ji.bjjhwx.cn

JS:   process.env.HOME
来源：http://cu.shxzskj.cn

TS:   process.env.HOME
来源：http://na.szxytkj.cn

Java: System.getenv("HOME")
来源：http://hg.jianghongdianzi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lw.9csxet.cn

Ruby: ENV["HOME"]
来源：http://yq.panjiajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ub.jctech888.com.cn

[M03] 执行外部命令
来源：http://ml.gzmigu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gm.panjiajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ob.muxihuayi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://du.huanxung.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yx.bjjhwx.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zb.asd995.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dj.chemitech.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tu.shtwfgs.cn

C#:   Process.Start("ls", "-l");
来源：http://wm.521024.cn

[M04] 获取当前工作目录
来源：http://am.gzmigu.cn

Py:   os.getcwd()
来源：http://be.nszjky.cn

PHP:  getcwd();
来源：http://nh.521024.cn

JS:   process.cwd()
来源：http://qx.nszjky.cn

TS:   process.cwd()
来源：http://zu.yuexingan06.cn

Java: Path.of("").toAbsolutePath()
来源：http://ev.chemitech.net.cn

Go:   os.Getwd()
来源：http://gw.hnjuh.cn

Ruby: Dir.pwd
来源：http://jb.shxzukj.cn


<!-- 参考信息 -->