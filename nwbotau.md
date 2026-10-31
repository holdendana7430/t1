代发 wailian999

Ruby: s.scan(/error/i)
来源：http://lr.9csxet.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ir.shxzskj.cn

[I08] 贪婪与非贪婪匹配
来源：http://ni.chemitech.net.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ci.hahajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wr.shxzukj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rt.shxzukj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oj.chemitech.net.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lj.huixinmuqiang.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ij.yuexingan06.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oo.jianghongdianzi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tw.521024.cn

================================================================================
来源：http://ys.szsharing.cn

J. 日期与时间
来源：http://rf.shtwfgs.cn

================================================================================
来源：http://vg.chemitech.net.cn

[J01] 获取当前时间
来源：http://gp.haigaiapp.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cf.shxzukj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://il.nicolike.cn

JS:   new Date();  Date.now()
来源：http://yu.yuexingan06.cn

TS:   new Date();  Date.now()
来源：http://gq.bookmarksfly.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://cy.9csxet.cn

Go:   time.Now()
来源：http://an.chemitech.net.cn

Ruby: Time.now
来源：http://lo.shxzukj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lp.9csxet.cn

[J02] 格式化输出
来源：http://vb.huixiangedu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hd.lnxyls.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://om.521024.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vv.lnxyls.cn

TS:   d.toISOString()
来源：http://sr.shxzukj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://up.jianghongdianzi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jj.bjjhwx.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gn.lnxyls.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sj.lnxyls.cn

[J03] 字符串解析为日期
来源：http://sb.gzmigu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wh.huixiangedu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xf.bjjhwx.cn

JS:   new Date("2024-01-02")
来源：http://vp.bookmarksfly.cn

TS:   new Date("2024-01-02")
来源：http://dr.shxzukj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ip.nszjky.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://py.bjjhwx.cn

Ruby: Date.parse("2024-01-02")
来源：http://ds.muxihuayi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jk.bjjhwx.cn

[J04] 时间戳与日期互转
来源：http://yh.gzmigu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fk.colortex.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://st.521024.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ob.yuntaijiaju.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ae.huixiangedu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vu.huixiangedu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mj.colortex.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rm.yuexingan06.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qr.bjjhwx.cn

[J05] 时间加减（加 7 天）
来源：http://qj.nszjky.cn

Py:   now + timedelta(days=7)
来源：http://ny.haigaiapp.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://on.chemitech.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mn.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lj.colortex.cn

Java: LocalDate.now().plusDays(7)
来源：http://wo.szsharing.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://we.huanxung.cn

Ruby: Time.now + 7 * 86400
来源：http://ft.bookmarksfly.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xk.szsharing.cn

[J06] 计算两时间之差
来源：http://mj.shtwfgs.cn

Py:   (end - start).total_seconds()
来源：http://tn.wgjwhj.cn

PHP:  $end->diff($start)->days;
来源：http://ww.521024.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qs.bookmarksfly.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lf.chemitech.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bj.jctech888.com.cn

Go:   end.Sub(start).Hours()
来源：http://pa.jctech888.com.cn

Ruby: end - start                 # 返回秒数
来源：http://lo.newstarts.cn

C#:   (end - start).TotalSeconds
来源：http://dy.521024.cn

[J07] 比较两个日期
来源：http://qh.huixiangedu.cn

Py:   d1 < d2;  d1 == d2
来源：http://pc.newstarts.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yn.gzmigu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ax.bjjhwx.cn

TS:   d1.getTime() < d2.getTime()
来源：http://oi.haigaiapp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lm.szsharing.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yh.huanxung.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ep.nszjky.cn

C#:   d1 < d2;  d1 == d2
来源：http://qu.nicolike.cn

[J08] 提取年月日与星期
来源：http://kn.jianghongdianzi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jd.bjjhwx.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kg.shtwfgs.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mv.jianghongdianzi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kh.shtwfgs.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kj.shtwfgs.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wy.muxihuayi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://on.panjiajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ys.hahajie.cn

[J09] 时区处理
来源：http://wx.shxzskj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pc.hnjuh.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wu.jianghongdianzi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fe.nicolike.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eo.hnjuh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wx.hahajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://at.hnjuh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fx.lnxyls.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://aq.szxytkj.cn

[J10] 取今天 / 本月第一天
来源：http://wo.521024.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://it.nszjky.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://re.hnjuh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zu.asd995.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://eh.szxytkj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ls.lnxyls.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rs.wgjwhj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vu.nszjky.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jd.asd995.cn

================================================================================
来源：http://uw.szsharing.cn

K. JSON 与序列化
来源：http://ie.haigaiapp.cn

================================================================================
来源：http://gu.wgjwhj.cn

[K01] 对象转 JSON 字符串
来源：http://qb.9csxet.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qq.bjjhwx.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ha.nszjky.cn

JS:   JSON.stringify(obj)
来源：http://tp.haigaiapp.cn

TS:   JSON.stringify(obj)
来源：http://ua.wgjwhj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kw.nicolike.cn

Go:   json.Marshal(obj)
来源：http://lv.lnxyls.cn

Ruby: obj.to_json                                     // require "json"
来源：http://km.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yl.jianghongdianzi.cn

[K02] JSON 字符串转对象
来源：http://fu.jianghongdianzi.cn

Py:   json.loads(s)
来源：http://iv.panjiajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://am.jianghongdianzi.cn

JS:   JSON.parse(s)
来源：http://lg.nszjky.cn

TS:   JSON.parse(s)
来源：http://dw.hnjuh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pa.gzmigu.cn

Go:   json.Unmarshal(data, &v)
来源：http://fu.newstarts.cn

Ruby: JSON.parse(s)
来源：http://xg.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://eo.9csxet.cn

[K03] JSON 美化输出（带缩进）
来源：http://vv.bjjhwx.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://py.lnxyls.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lp.newstarts.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jz.yuntaijiaju.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vv.bookmarksfly.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pz.hnjuh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wn.9csxet.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rw.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lm.huanxung.cn

[K04] 读取 JSON 文件
来源：http://co.jctech888.com.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qr.bjjhwx.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://da.521024.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kg.jianghongdianzi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hy.huanxung.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kp.nicolike.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nz.huanxung.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xm.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://to.bjjhwx.cn

[K05] 深拷贝对象
来源：http://ec.shxzukj.cn

Py:   copy.deepcopy(obj)
来源：http://zz.huanxung.cn

PHP:  unserialize(serialize($obj));
来源：http://ak.jianghongdianzi.cn

JS:   structuredClone(obj)
来源：http://du.nicolike.cn

TS:   structuredClone(obj)
来源：http://sm.shxzskj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://oa.huanxung.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wg.asd995.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mc.bjjhwx.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ew.521024.cn

[K06] 解析 URL 查询串
来源：http://oo.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hf.shxzskj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hx.chemitech.net.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kr.panjiajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xl.newstarts.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://va.nszjky.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://he.muxihuayi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nd.huixinmuqiang.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yv.muxihuayi.cn

[K07] 进制转换
来源：http://td.szxytkj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dy.szsharing.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bg.shtwfgs.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xy.asd995.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hx.chemitech.net.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://px.yuntaijiaju.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://if.shtwfgs.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jh.jctech888.com.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nx.bookmarksfly.cn

[K08] 二进制序列化（非 JSON）
来源：http://pk.9csxet.cn

Py:   pickle.dumps(obj)
来源：http://wx.asd995.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mb.gzmigu.cn

JS:   v8.serialize(obj)        // Node
来源：http://st.colortex.cn

TS:   v8.serialize(obj)        // Node
来源：http://ec.chemitech.net.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ix.colortex.cn

Go:   encoding/gob
来源：http://pk.chemitech.net.cn

Ruby: Marshal.dump(obj)
来源：http://zd.lnxyls.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qf.haigaiapp.cn

================================================================================
来源：http://rh.shxzukj.cn

L. 网络请求
来源：http://mb.yuntaijiaju.cn

================================================================================
来源：http://cf.huixinmuqiang.cn

[L01] 发送 GET 请求
来源：http://yu.hnjuh.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zl.panjiajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ki.huanxung.cn

JS:   await fetch(url)
来源：http://kp.521024.cn

TS:   await fetch(url)
来源：http://yd.521024.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bq.szsharing.cn

Go:   resp, err := http.Get(url)
来源：http://pa.9csxet.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ms.521024.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hh.shxzskj.cn

[L02] 发送 POST JSON
来源：http://og.yuexingan06.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ps.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ig.shxzukj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://np.chemitech.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ia.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ci.huixinmuqiang.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ew.hnjuh.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ul.colortex.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://eo.shtwfgs.cn

[L03] 设置自定义请求头
来源：http://xa.hahajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zo.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wl.huixinmuqiang.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gm.huixinmuqiang.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://la.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lq.colortex.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fe.shxzskj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wb.asd995.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pr.lnxyls.cn

[L04] 设置超时
来源：http://fq.shtwfgs.cn

Py:   requests.get(url, timeout=5)
来源：http://on.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://da.shxzskj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gu.gzmigu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fj.szxytkj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fu.shxzskj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ug.hahajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wk.gzmigu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nx.gzmigu.cn

[L05] 上传文件（multipart）
来源：http://hh.huixinmuqiang.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zs.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yu.9csxet.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ie.haigaiapp.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vf.hahajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dn.yuexingan06.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yi.chemitech.net.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tf.bjjhwx.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dw.jctech888.com.cn

[L06] 解析响应为 JSON
来源：http://od.panjiajie.cn

Py:   resp.json()
来源：http://dq.gzmigu.cn

PHP:  json_decode($body, true);
来源：http://db.colortex.cn

JS:   await resp.json()
来源：http://js.jctech888.com.cn

TS:   await resp.json()
来源：http://rg.yuexingan06.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ah.jianghongdianzi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://oa.wgjwhj.cn

Ruby: JSON.parse(resp.body)
来源：http://ik.gzmigu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://az.shxzskj.cn

[L07] 处理 HTTP 状态码
来源：http://ec.jianghongdianzi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ik.yuntaijiaju.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qo.huixinmuqiang.cn

JS:   resp.ok;  resp.status
来源：http://um.panjiajie.cn

TS:   resp.ok;  resp.status
来源：http://xl.panjiajie.cn

Java: resp.statusCode()
来源：http://di.colortex.cn

Go:   resp.StatusCode
来源：http://wc.lnxyls.cn

Ruby: resp.code.to_i
来源：http://at.muxihuayi.cn

C#:   (int)resp.StatusCode
来源：http://hx.bjjhwx.cn

[L08] 并发请求多个地址
来源：http://oq.szxytkj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fr.haigaiapp.cn

PHP:  curl_multi_init() 系列
来源：http://bu.9csxet.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fo.wgjwhj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nn.gzmigu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jz.colortex.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tn.asd995.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ab.yuexingan06.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://df.wgjwhj.cn

================================================================================
来源：http://bt.bookmarksfly.cn

M. 命令行 / 进程 / 环境
来源：http://dt.szxytkj.cn

================================================================================
来源：http://sh.huanxung.cn

[M01] 读取命令行参数
来源：http://fx.nicolike.cn

Py:   sys.argv[1:]
来源：http://ll.jianghongdianzi.cn

PHP:  $argv;  $argc;
来源：http://sj.yuexingan06.cn

JS:   process.argv.slice(2)
来源：http://ew.panjiajie.cn

TS:   process.argv.slice(2)
来源：http://yf.jctech888.com.cn

Java: args 数组（main 方法参数）
来源：http://zg.haigaiapp.cn

Go:   os.Args[1:]
来源：http://bb.lnxyls.cn

Ruby: ARGV
来源：http://us.szxytkj.cn

C#:   args 数组（Main 方法参数）
来源：http://ow.wgjwhj.cn

[M02] 读取环境变量
来源：http://jn.haigaiapp.cn

Py:   os.environ.get("HOME")
来源：http://vi.szxytkj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dk.shxzukj.cn

JS:   process.env.HOME
来源：http://cu.hahajie.cn

TS:   process.env.HOME
来源：http://ob.yuntaijiaju.cn

Java: System.getenv("HOME")
来源：http://fs.yuntaijiaju.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wx.bookmarksfly.cn

Ruby: ENV["HOME"]
来源：http://id.yuntaijiaju.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wa.colortex.cn

[M03] 执行外部命令
来源：http://bg.bjjhwx.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yo.szsharing.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gn.jctech888.com.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://em.hnjuh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ap.wgjwhj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lc.szsharing.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://sh.szxytkj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://al.jianghongdianzi.cn

C#:   Process.Start("ls", "-l");
来源：http://ik.newstarts.cn

[M04] 获取当前工作目录
来源：http://ft.colortex.cn

Py:   os.getcwd()
来源：http://ky.shtwfgs.cn

PHP:  getcwd();
来源：http://ha.nicolike.cn

JS:   process.cwd()
来源：http://yi.nszjky.cn

TS:   process.cwd()
来源：http://kg.chemitech.net.cn

Java: Path.of("").toAbsolutePath()
来源：http://ni.colortex.cn

Go:   os.Getwd()
来源：http://hx.colortex.cn

Ruby: Dir.pwd
来源：http://bu.newstarts.cn

C#:   Directory.GetCurrentDirectory()
来源：http://av.chemitech.net.cn

[M05] 设置退出码
来源：http://tl.jianghongdianzi.cn

Py:   sys.exit(1)
来源：http://zz.haigaiapp.cn

PHP:  exit(1);
来源：http://bx.huanxung.cn

JS:   process.exit(1)
来源：http://pu.jctech888.com.cn

TS:   process.exit(1)
来源：http://vj.shxzukj.cn

Java: System.exit(1)
来源：http://ep.wgjwhj.cn

Go:   os.Exit(1)
来源：http://gf.wgjwhj.cn


<!-- 参考信息 -->