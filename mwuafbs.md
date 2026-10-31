代发 wailian999

Ruby: s.scan(/error/i)
来源：http://pg.yuexingan06.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mu.shxzukj.cn

[I08] 贪婪与非贪婪匹配
来源：http://dl.jianghongdianzi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zx.yuexingan06.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xk.jctech888.com.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jc.hnjuh.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pc.9csxet.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ag.wgjwhj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ad.chemitech.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dq.huixinmuqiang.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ki.jianghongdianzi.cn

================================================================================
来源：http://rn.wgjwhj.cn

J. 日期与时间
来源：http://kd.newstarts.cn

================================================================================
来源：http://jg.shtwfgs.cn

[J01] 获取当前时间
来源：http://gu.shxzukj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://tw.gzmigu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lp.gzmigu.cn

JS:   new Date();  Date.now()
来源：http://pv.jctech888.com.cn

TS:   new Date();  Date.now()
来源：http://qg.huanxung.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://uq.szxytkj.cn

Go:   time.Now()
来源：http://rp.nicolike.cn

Ruby: Time.now
来源：http://dx.huixinmuqiang.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qj.colortex.cn

[J02] 格式化输出
来源：http://wq.huixinmuqiang.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fn.shtwfgs.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cc.9csxet.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yc.chemitech.net.cn

TS:   d.toISOString()
来源：http://wh.9csxet.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rj.521024.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tf.asd995.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ua.hnjuh.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ze.shtwfgs.cn

[J03] 字符串解析为日期
来源：http://zc.haigaiapp.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gw.wgjwhj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://my.szsharing.cn

JS:   new Date("2024-01-02")
来源：http://nt.nicolike.cn

TS:   new Date("2024-01-02")
来源：http://op.bjjhwx.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bb.gzmigu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tp.huanxung.cn

Ruby: Date.parse("2024-01-02")
来源：http://ef.521024.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://je.jctech888.com.cn

[J04] 时间戳与日期互转
来源：http://ef.shxzukj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vj.panjiajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nx.shtwfgs.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cr.muxihuayi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fy.nszjky.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mh.lnxyls.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lt.shxzukj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://md.bookmarksfly.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pt.huixiangedu.cn

[J05] 时间加减（加 7 天）
来源：http://wu.bjjhwx.cn

Py:   now + timedelta(days=7)
来源：http://we.521024.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ah.hnjuh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dd.nszjky.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rc.panjiajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://un.huanxung.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ah.newstarts.cn

Ruby: Time.now + 7 * 86400
来源：http://fc.shxzukj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ea.nszjky.cn

[J06] 计算两时间之差
来源：http://bk.lnxyls.cn

Py:   (end - start).total_seconds()
来源：http://nt.shxzukj.cn

PHP:  $end->diff($start)->days;
来源：http://vx.shxzukj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://us.shxzskj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qw.panjiajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fj.colortex.cn

Go:   end.Sub(start).Hours()
来源：http://az.muxihuayi.cn

Ruby: end - start                 # 返回秒数
来源：http://mk.szxytkj.cn

C#:   (end - start).TotalSeconds
来源：http://rz.jianghongdianzi.cn

[J07] 比较两个日期
来源：http://tp.yuntaijiaju.cn

Py:   d1 < d2;  d1 == d2
来源：http://vy.huanxung.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ql.huixiangedu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qg.yuexingan06.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ma.bookmarksfly.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jw.nicolike.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ya.lnxyls.cn

Ruby: d1 < d2;  d1 == d2
来源：http://my.shtwfgs.cn

C#:   d1 < d2;  d1 == d2
来源：http://ci.lnxyls.cn

[J08] 提取年月日与星期
来源：http://qt.hnjuh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zj.hnjuh.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zc.haigaiapp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xs.hahajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mu.colortex.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nk.huanxung.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sg.newstarts.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fg.9csxet.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qq.chemitech.net.cn

[J09] 时区处理
来源：http://zm.chemitech.net.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ea.9csxet.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vf.hahajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qf.chemitech.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ln.huanxung.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tr.lnxyls.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fm.nszjky.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://md.hnjuh.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://in.shxzukj.cn

[J10] 取今天 / 本月第一天
来源：http://jj.gzmigu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rd.szsharing.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ea.shtwfgs.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://je.haigaiapp.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mv.wgjwhj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://oz.jianghongdianzi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ef.haigaiapp.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mk.nszjky.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qf.lnxyls.cn

================================================================================
来源：http://lh.9csxet.cn

K. JSON 与序列化
来源：http://pj.9csxet.cn

================================================================================
来源：http://xc.chemitech.net.cn

[K01] 对象转 JSON 字符串
来源：http://dp.newstarts.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gz.nicolike.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gc.bjjhwx.cn

JS:   JSON.stringify(obj)
来源：http://pr.wgjwhj.cn

TS:   JSON.stringify(obj)
来源：http://rr.newstarts.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gx.yuexingan06.cn

Go:   json.Marshal(obj)
来源：http://ri.chemitech.net.cn

Ruby: obj.to_json                                     // require "json"
来源：http://yp.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://kt.huixinmuqiang.cn

[K02] JSON 字符串转对象
来源：http://sp.shxzukj.cn

Py:   json.loads(s)
来源：http://ju.lnxyls.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lv.9csxet.cn

JS:   JSON.parse(s)
来源：http://dn.bjjhwx.cn

TS:   JSON.parse(s)
来源：http://ii.huanxung.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qt.yuntaijiaju.cn

Go:   json.Unmarshal(data, &v)
来源：http://vy.newstarts.cn

Ruby: JSON.parse(s)
来源：http://bu.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://en.huanxung.cn

[K03] JSON 美化输出（带缩进）
来源：http://ij.panjiajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://or.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://um.shxzukj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://yt.asd995.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://hl.bookmarksfly.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zr.nszjky.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://be.yuntaijiaju.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jn.newstarts.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lk.gzmigu.cn

[K04] 读取 JSON 文件
来源：http://wa.nszjky.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hl.hahajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xf.521024.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jl.wgjwhj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tg.shxzskj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ca.shxzukj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ft.hnjuh.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rs.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ca.huixinmuqiang.cn

[K05] 深拷贝对象
来源：http://cg.chemitech.net.cn

Py:   copy.deepcopy(obj)
来源：http://mj.yuexingan06.cn

PHP:  unserialize(serialize($obj));
来源：http://yb.shxzskj.cn

JS:   structuredClone(obj)
来源：http://yh.newstarts.cn

TS:   structuredClone(obj)
来源：http://qu.shxzskj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rr.hnjuh.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://iw.chemitech.net.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mb.huanxung.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dr.nicolike.cn

[K06] 解析 URL 查询串
来源：http://dr.hahajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://et.shtwfgs.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hi.panjiajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xt.huixiangedu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ax.haigaiapp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sw.huanxung.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qa.shxzskj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fn.haigaiapp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qt.bookmarksfly.cn

[K07] 进制转换
来源：http://vm.jctech888.com.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://oi.521024.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fr.newstarts.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lg.jianghongdianzi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mw.newstarts.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hi.yuntaijiaju.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rq.shxzukj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xr.521024.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wr.bjjhwx.cn

[K08] 二进制序列化（非 JSON）
来源：http://pk.nicolike.cn

Py:   pickle.dumps(obj)
来源：http://ox.huanxung.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zb.chemitech.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://ao.nicolike.cn

TS:   v8.serialize(obj)        // Node
来源：http://ge.hahajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jz.szsharing.cn

Go:   encoding/gob
来源：http://dr.huixinmuqiang.cn

Ruby: Marshal.dump(obj)
来源：http://ia.huixiangedu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cj.chemitech.net.cn

================================================================================
来源：http://qk.hnjuh.cn

L. 网络请求
来源：http://vg.yuexingan06.cn

================================================================================
来源：http://sh.gzmigu.cn

[L01] 发送 GET 请求
来源：http://us.nicolike.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ja.hahajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gv.wgjwhj.cn

JS:   await fetch(url)
来源：http://jc.newstarts.cn

TS:   await fetch(url)
来源：http://nf.yuexingan06.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://au.hnjuh.cn

Go:   resp, err := http.Get(url)
来源：http://fg.haigaiapp.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ht.yuntaijiaju.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yn.haigaiapp.cn

[L02] 发送 POST JSON
来源：http://qj.9csxet.cn

Py:   requests.post(url, json={"a": 1})
来源：http://tl.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kc.muxihuayi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ri.chemitech.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vk.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cp.nicolike.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ml.jianghongdianzi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ae.colortex.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gf.bookmarksfly.cn

[L03] 设置自定义请求头
来源：http://wr.colortex.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cp.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vf.gzmigu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://in.jianghongdianzi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bw.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ft.nicolike.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://be.yuntaijiaju.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hu.hnjuh.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mv.gzmigu.cn

[L04] 设置超时
来源：http://mu.shxzskj.cn

Py:   requests.get(url, timeout=5)
来源：http://sa.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hq.nicolike.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kb.panjiajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shtwfgs.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pz.yuexingan06.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cl.szxytkj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fe.newstarts.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hu.huixiangedu.cn

[L05] 上传文件（multipart）
来源：http://jd.szxytkj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nf.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yv.yuexingan06.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xp.huixinmuqiang.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qr.nicolike.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qb.yuexingan06.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rx.huixiangedu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://eg.szxytkj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gs.bookmarksfly.cn

[L06] 解析响应为 JSON
来源：http://wo.szxytkj.cn

Py:   resp.json()
来源：http://zm.asd995.cn

PHP:  json_decode($body, true);
来源：http://qd.9csxet.cn

JS:   await resp.json()
来源：http://yl.wgjwhj.cn

TS:   await resp.json()
来源：http://ty.nszjky.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xl.521024.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mx.szsharing.cn

Ruby: JSON.parse(resp.body)
来源：http://ap.shxzukj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qw.shxzskj.cn

[L07] 处理 HTTP 状态码
来源：http://kh.huixiangedu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nr.yuntaijiaju.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yv.521024.cn

JS:   resp.ok;  resp.status
来源：http://wv.szxytkj.cn

TS:   resp.ok;  resp.status
来源：http://ac.huanxung.cn

Java: resp.statusCode()
来源：http://lq.bjjhwx.cn

Go:   resp.StatusCode
来源：http://nn.chemitech.net.cn

Ruby: resp.code.to_i
来源：http://ye.asd995.cn

C#:   (int)resp.StatusCode
来源：http://jy.szxytkj.cn

[L08] 并发请求多个地址
来源：http://fk.wgjwhj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ql.bjjhwx.cn

PHP:  curl_multi_init() 系列
来源：http://ba.hnjuh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tn.huixiangedu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bv.lnxyls.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fq.asd995.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mg.9csxet.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ag.szxytkj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wl.huixinmuqiang.cn

================================================================================
来源：http://zk.gzmigu.cn

M. 命令行 / 进程 / 环境
来源：http://gy.hahajie.cn

================================================================================
来源：http://bz.shxzukj.cn

[M01] 读取命令行参数
来源：http://uf.nszjky.cn

Py:   sys.argv[1:]
来源：http://uh.nszjky.cn

PHP:  $argv;  $argc;
来源：http://oq.jctech888.com.cn

JS:   process.argv.slice(2)
来源：http://fn.shxzskj.cn

TS:   process.argv.slice(2)
来源：http://qc.9csxet.cn

Java: args 数组（main 方法参数）
来源：http://bp.yuntaijiaju.cn

Go:   os.Args[1:]
来源：http://nu.jctech888.com.cn

Ruby: ARGV
来源：http://dp.jctech888.com.cn

C#:   args 数组（Main 方法参数）
来源：http://cd.chemitech.net.cn

[M02] 读取环境变量
来源：http://yj.huixiangedu.cn

Py:   os.environ.get("HOME")
来源：http://jj.jctech888.com.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cp.szsharing.cn

JS:   process.env.HOME
来源：http://zu.jctech888.com.cn

TS:   process.env.HOME
来源：http://qh.huanxung.cn

Java: System.getenv("HOME")
来源：http://kw.nicolike.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qt.9csxet.cn

Ruby: ENV["HOME"]
来源：http://th.chemitech.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bx.521024.cn

[M03] 执行外部命令
来源：http://xo.gzmigu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rb.szxytkj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cw.jctech888.com.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kz.panjiajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://lv.muxihuayi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://op.yuntaijiaju.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ev.lnxyls.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vb.huixiangedu.cn

C#:   Process.Start("ls", "-l");
来源：http://bv.shtwfgs.cn

[M04] 获取当前工作目录
来源：http://sr.nicolike.cn

Py:   os.getcwd()
来源：http://xc.wgjwhj.cn

PHP:  getcwd();
来源：http://sm.gzmigu.cn

JS:   process.cwd()
来源：http://hr.jctech888.com.cn

TS:   process.cwd()
来源：http://cr.hnjuh.cn

Java: Path.of("").toAbsolutePath()
来源：http://lq.hahajie.cn

Go:   os.Getwd()
来源：http://br.panjiajie.cn

Ruby: Dir.pwd
来源：http://jx.shxzukj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://oc.panjiajie.cn

[M05] 设置退出码
来源：http://yv.haigaiapp.cn

Py:   sys.exit(1)
来源：http://rx.jianghongdianzi.cn

PHP:  exit(1);
来源：http://ye.colortex.cn

JS:   process.exit(1)
来源：http://tw.hnjuh.cn

TS:   process.exit(1)
来源：http://je.nicolike.cn

Java: System.exit(1)
来源：http://du.nszjky.cn

Go:   os.Exit(1)
来源：http://jx.szsharing.cn


<!-- 参考信息 -->