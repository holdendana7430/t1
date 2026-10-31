代发 wailian999

Ruby: s.scan(/error/i)
来源：http://ew.colortex.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ao.hnjuh.cn

[I08] 贪婪与非贪婪匹配
来源：http://ye.521024.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://so.panjiajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lm.shtwfgs.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pm.newstarts.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xw.shxzskj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ak.shtwfgs.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cv.bjjhwx.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jh.shxzskj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rm.yuntaijiaju.cn

================================================================================
来源：http://he.521024.cn

J. 日期与时间
来源：http://vh.chemitech.net.cn

================================================================================
来源：http://xp.huixiangedu.cn

[J01] 获取当前时间
来源：http://wj.colortex.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cg.shxzukj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xw.nicolike.cn

JS:   new Date();  Date.now()
来源：http://br.huixinmuqiang.cn

TS:   new Date();  Date.now()
来源：http://pl.asd995.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://sm.szxytkj.cn

Go:   time.Now()
来源：http://aw.chemitech.net.cn

Ruby: Time.now
来源：http://vf.hahajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://su.szsharing.cn

[J02] 格式化输出
来源：http://iy.lnxyls.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sa.newstarts.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://be.haigaiapp.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ja.jctech888.com.cn

TS:   d.toISOString()
来源：http://fp.szxytkj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ri.szsharing.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://se.chemitech.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eo.colortex.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.huanxung.cn

[J03] 字符串解析为日期
来源：http://ea.lnxyls.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xm.521024.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dh.jctech888.com.cn

JS:   new Date("2024-01-02")
来源：http://ht.yuntaijiaju.cn

TS:   new Date("2024-01-02")
来源：http://bx.huixiangedu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://lk.bjjhwx.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rf.yuntaijiaju.cn

Ruby: Date.parse("2024-01-02")
来源：http://xf.yuntaijiaju.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ji.gzmigu.cn

[J04] 时间戳与日期互转
来源：http://tp.huanxung.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rw.colortex.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://re.bookmarksfly.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cg.panjiajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hm.huanxung.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wq.bjjhwx.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://on.panjiajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uo.huixinmuqiang.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fk.hahajie.cn

[J05] 时间加减（加 7 天）
来源：http://ed.hahajie.cn

Py:   now + timedelta(days=7)
来源：http://wo.hahajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lv.gzmigu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qx.shxzukj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ts.szxytkj.cn

Java: LocalDate.now().plusDays(7)
来源：http://ka.shxzukj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://eu.521024.cn

Ruby: Time.now + 7 * 86400
来源：http://lb.nicolike.cn

C#:   DateTime.Now.AddDays(7)
来源：http://sp.panjiajie.cn

[J06] 计算两时间之差
来源：http://rl.9csxet.cn

Py:   (end - start).total_seconds()
来源：http://sx.bookmarksfly.cn

PHP:  $end->diff($start)->days;
来源：http://ot.panjiajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xi.hnjuh.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ft.yuexingan06.cn

Java: Duration.between(start, end).toSeconds()
来源：http://cb.szxytkj.cn

Go:   end.Sub(start).Hours()
来源：http://mg.nszjky.cn

Ruby: end - start                 # 返回秒数
来源：http://ad.lnxyls.cn

C#:   (end - start).TotalSeconds
来源：http://mi.haigaiapp.cn

[J07] 比较两个日期
来源：http://pe.haigaiapp.cn

Py:   d1 < d2;  d1 == d2
来源：http://kl.huixiangedu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bx.panjiajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://em.9csxet.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gr.newstarts.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uc.muxihuayi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ma.shtwfgs.cn

Ruby: d1 < d2;  d1 == d2
来源：http://an.yuntaijiaju.cn

C#:   d1 < d2;  d1 == d2
来源：http://na.bookmarksfly.cn

[J08] 提取年月日与星期
来源：http://ym.szsharing.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kc.szsharing.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jx.yuntaijiaju.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fx.lnxyls.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lo.bookmarksfly.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fh.9csxet.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zp.chemitech.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://go.nszjky.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xs.huanxung.cn

[J09] 时区处理
来源：http://tb.bjjhwx.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jx.9csxet.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://az.gzmigu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dp.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uv.jianghongdianzi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xf.jianghongdianzi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tr.asd995.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vp.nszjky.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ew.szsharing.cn

[J10] 取今天 / 本月第一天
来源：http://en.huanxung.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gk.szsharing.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rt.szxytkj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ri.9csxet.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zg.huanxung.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ob.szxytkj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ic.hahajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vh.jianghongdianzi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zd.asd995.cn

================================================================================
来源：http://up.hnjuh.cn

K. JSON 与序列化
来源：http://gh.huanxung.cn

================================================================================
来源：http://wx.bjjhwx.cn

[K01] 对象转 JSON 字符串
来源：http://ha.shxzukj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ew.hahajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ob.colortex.cn

JS:   JSON.stringify(obj)
来源：http://et.chemitech.net.cn

TS:   JSON.stringify(obj)
来源：http://ec.gzmigu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ge.chemitech.net.cn

Go:   json.Marshal(obj)
来源：http://pj.hnjuh.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ip.szxytkj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ac.shxzukj.cn

[K02] JSON 字符串转对象
来源：http://jv.nicolike.cn

Py:   json.loads(s)
来源：http://cb.521024.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lz.colortex.cn

JS:   JSON.parse(s)
来源：http://gi.colortex.cn

TS:   JSON.parse(s)
来源：http://sj.bjjhwx.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wh.huixinmuqiang.cn

Go:   json.Unmarshal(data, &v)
来源：http://cn.huixinmuqiang.cn

Ruby: JSON.parse(s)
来源：http://dg.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qf.nicolike.cn

[K03] JSON 美化输出（带缩进）
来源：http://ok.huixiangedu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://je.asd995.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ig.huanxung.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qm.colortex.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ka.hnjuh.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://so.bjjhwx.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mt.asd995.cn

Ruby: JSON.pretty_generate(obj)
来源：http://em.gzmigu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ci.hnjuh.cn

[K04] 读取 JSON 文件
来源：http://ep.yuexingan06.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uf.jctech888.com.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://an.panjiajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ag.yuexingan06.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fz.hahajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bc.szsharing.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ll.shtwfgs.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rz.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ff.huixinmuqiang.cn

[K05] 深拷贝对象
来源：http://ya.chemitech.net.cn

Py:   copy.deepcopy(obj)
来源：http://lv.huanxung.cn

PHP:  unserialize(serialize($obj));
来源：http://cc.nicolike.cn

JS:   structuredClone(obj)
来源：http://eb.chemitech.net.cn

TS:   structuredClone(obj)
来源：http://tn.huanxung.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ju.lnxyls.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://by.bjjhwx.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ty.gzmigu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ro.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://dq.nszjky.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gz.yuntaijiaju.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hd.newstarts.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xm.shxzskj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qr.bookmarksfly.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hl.lnxyls.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cy.muxihuayi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zo.yuntaijiaju.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xx.gzmigu.cn

[K07] 进制转换
来源：http://io.nszjky.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wx.lnxyls.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://eo.jctech888.com.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ge.szxytkj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rb.521024.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xz.shxzukj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mg.panjiajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zn.haigaiapp.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ot.yuntaijiaju.cn

[K08] 二进制序列化（非 JSON）
来源：http://ms.shxzskj.cn

Py:   pickle.dumps(obj)
来源：http://hy.shtwfgs.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.huixinmuqiang.cn

JS:   v8.serialize(obj)        // Node
来源：http://xg.hnjuh.cn

TS:   v8.serialize(obj)        // Node
来源：http://ik.shxzukj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ri.nicolike.cn

Go:   encoding/gob
来源：http://cc.hnjuh.cn

Ruby: Marshal.dump(obj)
来源：http://ah.jianghongdianzi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://di.colortex.cn

================================================================================
来源：http://tc.yuexingan06.cn

L. 网络请求
来源：http://dr.wgjwhj.cn

================================================================================
来源：http://ok.jianghongdianzi.cn

[L01] 发送 GET 请求
来源：http://xc.panjiajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ko.panjiajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://px.jianghongdianzi.cn

JS:   await fetch(url)
来源：http://kq.521024.cn

TS:   await fetch(url)
来源：http://nk.jctech888.com.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ap.hnjuh.cn

Go:   resp, err := http.Get(url)
来源：http://xd.jianghongdianzi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://il.hnjuh.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://md.yuntaijiaju.cn

[L02] 发送 POST JSON
来源：http://as.newstarts.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wv.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rp.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zd.szsharing.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jn.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://an.9csxet.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ah.huanxung.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nx.huanxung.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kd.lnxyls.cn

[L03] 设置自定义请求头
来源：http://bo.hnjuh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kv.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tq.newstarts.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yq.9csxet.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fi.colortex.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jg.9csxet.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mi.shtwfgs.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pl.bookmarksfly.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wf.9csxet.cn

[L04] 设置超时
来源：http://ci.huixiangedu.cn

Py:   requests.get(url, timeout=5)
来源：http://ns.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jp.chemitech.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://on.muxihuayi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pa.shxzskj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gi.521024.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://du.jianghongdianzi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tn.huanxung.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bz.lnxyls.cn

[L05] 上传文件（multipart）
来源：http://hu.colortex.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zu.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pq.shxzukj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://iu.521024.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://of.521024.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ih.newstarts.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zy.huanxung.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wd.bookmarksfly.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://en.szxytkj.cn

[L06] 解析响应为 JSON
来源：http://ba.huixiangedu.cn

Py:   resp.json()
来源：http://ip.lnxyls.cn

PHP:  json_decode($body, true);
来源：http://bp.jctech888.com.cn

JS:   await resp.json()
来源：http://dc.yuexingan06.cn

TS:   await resp.json()
来源：http://cs.9csxet.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://iy.nicolike.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pk.huixinmuqiang.cn

Ruby: JSON.parse(resp.body)
来源：http://xs.shxzukj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://du.colortex.cn

[L07] 处理 HTTP 状态码
来源：http://ll.wgjwhj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://eq.szsharing.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kh.bookmarksfly.cn

JS:   resp.ok;  resp.status
来源：http://wt.huixiangedu.cn

TS:   resp.ok;  resp.status
来源：http://fu.huixinmuqiang.cn

Java: resp.statusCode()
来源：http://fp.bjjhwx.cn

Go:   resp.StatusCode
来源：http://mf.wgjwhj.cn

Ruby: resp.code.to_i
来源：http://hr.wgjwhj.cn

C#:   (int)resp.StatusCode
来源：http://wj.huixinmuqiang.cn

[L08] 并发请求多个地址
来源：http://oi.muxihuayi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nx.bookmarksfly.cn

PHP:  curl_multi_init() 系列
来源：http://hi.jctech888.com.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zk.jianghongdianzi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yw.lnxyls.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rz.muxihuayi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ed.bookmarksfly.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fe.huixinmuqiang.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://aw.shxzukj.cn

================================================================================
来源：http://ai.asd995.cn

M. 命令行 / 进程 / 环境
来源：http://ez.colortex.cn

================================================================================
来源：http://ej.bjjhwx.cn

[M01] 读取命令行参数
来源：http://ai.jctech888.com.cn

Py:   sys.argv[1:]
来源：http://wr.lnxyls.cn

PHP:  $argv;  $argc;
来源：http://dg.newstarts.cn

JS:   process.argv.slice(2)
来源：http://bh.shxzukj.cn

TS:   process.argv.slice(2)
来源：http://zi.huixiangedu.cn

Java: args 数组（main 方法参数）
来源：http://oh.huixiangedu.cn

Go:   os.Args[1:]
来源：http://vc.9csxet.cn

Ruby: ARGV
来源：http://aw.lnxyls.cn

C#:   args 数组（Main 方法参数）
来源：http://ec.gzmigu.cn

[M02] 读取环境变量
来源：http://rc.jianghongdianzi.cn

Py:   os.environ.get("HOME")
来源：http://jh.shxzukj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gp.hnjuh.cn

JS:   process.env.HOME
来源：http://li.szxytkj.cn

TS:   process.env.HOME
来源：http://ep.shxzukj.cn

Java: System.getenv("HOME")
来源：http://mj.wgjwhj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ok.shxzukj.cn

Ruby: ENV["HOME"]
来源：http://bl.muxihuayi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ka.yuntaijiaju.cn

[M03] 执行外部命令
来源：http://ok.bookmarksfly.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://oc.huixiangedu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lw.jctech888.com.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jo.asd995.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pi.521024.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vp.colortex.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://az.huanxung.cn

Ruby: system("ls -l");  `ls -l`
来源：http://br.shxzskj.cn

C#:   Process.Start("ls", "-l");
来源：http://ee.9csxet.cn

[M04] 获取当前工作目录
来源：http://js.jianghongdianzi.cn

Py:   os.getcwd()
来源：http://zv.bookmarksfly.cn

PHP:  getcwd();
来源：http://fo.asd995.cn

JS:   process.cwd()
来源：http://zk.panjiajie.cn

TS:   process.cwd()
来源：http://jl.nicolike.cn

Java: Path.of("").toAbsolutePath()
来源：http://ya.shtwfgs.cn

Go:   os.Getwd()
来源：http://tt.lnxyls.cn

Ruby: Dir.pwd
来源：http://pm.huixiangedu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://en.nszjky.cn

[M05] 设置退出码
来源：http://ts.chemitech.net.cn

Py:   sys.exit(1)
来源：http://br.shxzukj.cn

PHP:  exit(1);
来源：http://qo.nszjky.cn

JS:   process.exit(1)
来源：http://sk.huixinmuqiang.cn

TS:   process.exit(1)
来源：http://sq.shxzskj.cn

Java: System.exit(1)
来源：http://dp.muxihuayi.cn

Go:   os.Exit(1)
来源：http://bh.nicolike.cn


<!-- 参考信息 -->