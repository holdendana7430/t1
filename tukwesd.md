代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://li.panjiajie.cn

TS:   /error/gim
来源：http://vm.szsharing.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://at.huanxung.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lj.muxihuayi.cn

Ruby: s.scan(/error/i)
来源：http://te.wgjwhj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ut.haigaiapp.cn

[I08] 贪婪与非贪婪匹配
来源：http://mb.shxzskj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mf.shxzukj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bd.chemitech.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://oq.wgjwhj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oa.newstarts.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://mf.hnjuh.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yx.hahajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jk.panjiajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vw.521024.cn

================================================================================
来源：http://vh.haigaiapp.cn

J. 日期与时间
来源：http://bs.yuexingan06.cn

================================================================================
来源：http://oc.shtwfgs.cn

[J01] 获取当前时间
来源：http://rd.huanxung.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://mi.bjjhwx.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fc.shtwfgs.cn

JS:   new Date();  Date.now()
来源：http://xu.gzmigu.cn

TS:   new Date();  Date.now()
来源：http://tg.hnjuh.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ym.huanxung.cn

Go:   time.Now()
来源：http://go.huixiangedu.cn

Ruby: Time.now
来源：http://ny.panjiajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qv.yuexingan06.cn

[J02] 格式化输出
来源：http://gs.lnxyls.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dy.shxzukj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rk.lnxyls.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dp.wgjwhj.cn

TS:   d.toISOString()
来源：http://nz.yuntaijiaju.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://at.asd995.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://aw.yuntaijiaju.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qa.huixinmuqiang.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vo.asd995.cn

[J03] 字符串解析为日期
来源：http://ro.9csxet.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xc.nszjky.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bd.colortex.cn

JS:   new Date("2024-01-02")
来源：http://ck.521024.cn

TS:   new Date("2024-01-02")
来源：http://jm.bookmarksfly.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fd.bjjhwx.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bs.hnjuh.cn

Ruby: Date.parse("2024-01-02")
来源：http://es.hahajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hu.bjjhwx.cn

[J04] 时间戳与日期互转
来源：http://mk.gzmigu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xr.panjiajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wg.panjiajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tb.chemitech.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ib.lnxyls.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wm.haigaiapp.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fz.yuntaijiaju.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uz.szsharing.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://en.gzmigu.cn

[J05] 时间加减（加 7 天）
来源：http://jr.521024.cn

Py:   now + timedelta(days=7)
来源：http://eo.lnxyls.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://or.hnjuh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wl.newstarts.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rf.hahajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://ir.muxihuayi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ez.shtwfgs.cn

Ruby: Time.now + 7 * 86400
来源：http://xu.yuntaijiaju.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xc.huanxung.cn

[J06] 计算两时间之差
来源：http://gf.szsharing.cn

Py:   (end - start).total_seconds()
来源：http://ka.521024.cn

PHP:  $end->diff($start)->days;
来源：http://ab.nicolike.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yj.hahajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gl.colortex.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ev.hnjuh.cn

Go:   end.Sub(start).Hours()
来源：http://ue.panjiajie.cn

Ruby: end - start                 # 返回秒数
来源：http://sg.shtwfgs.cn

C#:   (end - start).TotalSeconds
来源：http://ly.bookmarksfly.cn

[J07] 比较两个日期
来源：http://lk.nicolike.cn

Py:   d1 < d2;  d1 == d2
来源：http://az.huixinmuqiang.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ci.yuexingan06.cn

JS:   d1.getTime() < d2.getTime()
来源：http://sd.szsharing.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rc.hnjuh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vx.521024.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://va.nszjky.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fg.huixinmuqiang.cn

C#:   d1 < d2;  d1 == d2
来源：http://ny.shtwfgs.cn

[J08] 提取年月日与星期
来源：http://xw.hnjuh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://av.jianghongdianzi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xm.bookmarksfly.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ha.colortex.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nn.jctech888.com.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kg.huixiangedu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vx.shxzukj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hy.asd995.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jj.lnxyls.cn

[J09] 时区处理
来源：http://dn.yuexingan06.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yu.nszjky.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://uz.panjiajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mo.shtwfgs.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mz.lnxyls.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ri.chemitech.net.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gi.szxytkj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://sc.bjjhwx.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ep.szsharing.cn

[J10] 取今天 / 本月第一天
来源：http://fb.panjiajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hb.chemitech.net.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qp.huixiangedu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://az.chemitech.net.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rc.9csxet.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ua.szxytkj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wm.nszjky.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lm.szxytkj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ls.wgjwhj.cn

================================================================================
来源：http://xm.shxzskj.cn

K. JSON 与序列化
来源：http://ue.wgjwhj.cn

================================================================================
来源：http://hg.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://bg.yuexingan06.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dl.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zw.yuexingan06.cn

JS:   JSON.stringify(obj)
来源：http://ef.huixinmuqiang.cn

TS:   JSON.stringify(obj)
来源：http://lj.jctech888.com.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yy.jctech888.com.cn

Go:   json.Marshal(obj)
来源：http://te.newstarts.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ut.shxzskj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wg.bjjhwx.cn

[K02] JSON 字符串转对象
来源：http://ie.shxzskj.cn

Py:   json.loads(s)
来源：http://uv.asd995.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://js.haigaiapp.cn

JS:   JSON.parse(s)
来源：http://my.nszjky.cn

TS:   JSON.parse(s)
来源：http://qi.bookmarksfly.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tj.bjjhwx.cn

Go:   json.Unmarshal(data, &v)
来源：http://xr.newstarts.cn

Ruby: JSON.parse(s)
来源：http://vc.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sk.chemitech.net.cn

[K03] JSON 美化输出（带缩进）
来源：http://lm.colortex.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pa.newstarts.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wd.9csxet.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zj.asd995.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tn.huixinmuqiang.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oe.haigaiapp.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hf.chemitech.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vg.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tb.9csxet.cn

[K04] 读取 JSON 文件
来源：http://kx.colortex.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zy.lnxyls.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jd.jctech888.com.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wc.jianghongdianzi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wj.haigaiapp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pe.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uy.shxzskj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ci.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jf.yuexingan06.cn

[K05] 深拷贝对象
来源：http://dv.muxihuayi.cn

Py:   copy.deepcopy(obj)
来源：http://aw.huixinmuqiang.cn

PHP:  unserialize(serialize($obj));
来源：http://yb.nszjky.cn

JS:   structuredClone(obj)
来源：http://pb.jianghongdianzi.cn

TS:   structuredClone(obj)
来源：http://qk.nicolike.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jk.szxytkj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://va.huixiangedu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yq.jianghongdianzi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lt.bjjhwx.cn

[K06] 解析 URL 查询串
来源：http://ky.yuexingan06.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wy.521024.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hj.yuntaijiaju.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ow.hahajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jm.yuexingan06.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tl.szsharing.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fz.521024.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ri.haigaiapp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yx.wgjwhj.cn

[K07] 进制转换
来源：http://kc.asd995.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vm.haigaiapp.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fn.chemitech.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jp.lnxyls.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ga.colortex.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uj.nicolike.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sz.huixinmuqiang.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ll.lnxyls.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://au.gzmigu.cn

[K08] 二进制序列化（非 JSON）
来源：http://vx.shxzskj.cn

Py:   pickle.dumps(obj)
来源：http://xt.hnjuh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://rh.9csxet.cn

JS:   v8.serialize(obj)        // Node
来源：http://fn.nicolike.cn

TS:   v8.serialize(obj)        // Node
来源：http://lj.bjjhwx.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://if.huanxung.cn

Go:   encoding/gob
来源：http://ex.huixiangedu.cn

Ruby: Marshal.dump(obj)
来源：http://ui.szsharing.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://km.huixiangedu.cn

================================================================================
来源：http://ka.shtwfgs.cn

L. 网络请求
来源：http://hs.yuexingan06.cn

================================================================================
来源：http://gu.colortex.cn

[L01] 发送 GET 请求
来源：http://ln.szsharing.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ac.colortex.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ug.521024.cn

JS:   await fetch(url)
来源：http://el.yuexingan06.cn

TS:   await fetch(url)
来源：http://sk.jianghongdianzi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gp.szxytkj.cn

Go:   resp, err := http.Get(url)
来源：http://wj.colortex.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zd.huanxung.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bd.huixiangedu.cn

[L02] 发送 POST JSON
来源：http://qk.szsharing.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qd.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dy.bjjhwx.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gb.yuntaijiaju.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://an.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://me.colortex.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qa.lnxyls.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ra.huixiangedu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bg.nicolike.cn

[L03] 设置自定义请求头
来源：http://ce.hnjuh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://au.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ce.lnxyls.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pj.9csxet.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xf.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qr.huanxung.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ct.nicolike.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://at.huixinmuqiang.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sz.yuexingan06.cn

[L04] 设置超时
来源：http://rt.wgjwhj.cn

Py:   requests.get(url, timeout=5)
来源：http://bg.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yf.chemitech.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xc.szxytkj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cq.gzmigu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qe.nicolike.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hj.jctech888.com.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vx.muxihuayi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qx.521024.cn

[L05] 上传文件（multipart）
来源：http://oy.shtwfgs.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rf.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rc.asd995.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lv.huixiangedu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vg.shtwfgs.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ex.colortex.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ah.bookmarksfly.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uq.shtwfgs.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jd.jctech888.com.cn

[L06] 解析响应为 JSON
来源：http://zn.szsharing.cn

Py:   resp.json()
来源：http://ay.szsharing.cn

PHP:  json_decode($body, true);
来源：http://fe.bjjhwx.cn

JS:   await resp.json()
来源：http://vr.haigaiapp.cn

TS:   await resp.json()
来源：http://rh.bookmarksfly.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dl.jctech888.com.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ke.chemitech.net.cn

Ruby: JSON.parse(resp.body)
来源：http://nm.yuntaijiaju.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vm.haigaiapp.cn

[L07] 处理 HTTP 状态码
来源：http://xn.chemitech.net.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qo.szxytkj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ra.szxytkj.cn

JS:   resp.ok;  resp.status
来源：http://lp.lnxyls.cn

TS:   resp.ok;  resp.status
来源：http://im.yuexingan06.cn

Java: resp.statusCode()
来源：http://oe.huanxung.cn

Go:   resp.StatusCode
来源：http://ll.colortex.cn

Ruby: resp.code.to_i
来源：http://nv.hahajie.cn

C#:   (int)resp.StatusCode
来源：http://il.colortex.cn

[L08] 并发请求多个地址
来源：http://md.yuexingan06.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vw.wgjwhj.cn

PHP:  curl_multi_init() 系列
来源：http://nc.chemitech.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://de.haigaiapp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yg.chemitech.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bc.jctech888.com.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://am.chemitech.net.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://of.shxzskj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://as.chemitech.net.cn

================================================================================
来源：http://rr.panjiajie.cn

M. 命令行 / 进程 / 环境
来源：http://wg.newstarts.cn

================================================================================
来源：http://yz.shxzukj.cn

[M01] 读取命令行参数
来源：http://ox.szsharing.cn

Py:   sys.argv[1:]
来源：http://ph.nicolike.cn

PHP:  $argv;  $argc;
来源：http://bv.szxytkj.cn

JS:   process.argv.slice(2)
来源：http://wr.jctech888.com.cn

TS:   process.argv.slice(2)
来源：http://xr.shxzskj.cn

Java: args 数组（main 方法参数）
来源：http://oj.haigaiapp.cn

Go:   os.Args[1:]
来源：http://yx.newstarts.cn

Ruby: ARGV
来源：http://gy.szxytkj.cn

C#:   args 数组（Main 方法参数）
来源：http://yk.bjjhwx.cn

[M02] 读取环境变量
来源：http://tc.lnxyls.cn

Py:   os.environ.get("HOME")
来源：http://gq.jianghongdianzi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ql.huanxung.cn

JS:   process.env.HOME
来源：http://ea.nicolike.cn

TS:   process.env.HOME
来源：http://vj.lnxyls.cn

Java: System.getenv("HOME")
来源：http://dt.huixiangedu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sq.521024.cn

Ruby: ENV["HOME"]
来源：http://so.shxzskj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tb.jctech888.com.cn

[M03] 执行外部命令
来源：http://by.521024.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tk.huanxung.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ms.huixinmuqiang.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qv.muxihuayi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://dt.wgjwhj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://us.hahajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gn.huanxung.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tl.colortex.cn

C#:   Process.Start("ls", "-l");
来源：http://ud.asd995.cn

[M04] 获取当前工作目录
来源：http://aa.colortex.cn

Py:   os.getcwd()
来源：http://ec.haigaiapp.cn

PHP:  getcwd();
来源：http://lp.hnjuh.cn

JS:   process.cwd()
来源：http://tq.yuexingan06.cn

TS:   process.cwd()
来源：http://wv.hahajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://ks.bookmarksfly.cn

Go:   os.Getwd()
来源：http://bv.shtwfgs.cn

Ruby: Dir.pwd
来源：http://ah.hnjuh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://bo.chemitech.net.cn

[M05] 设置退出码
来源：http://og.wgjwhj.cn

Py:   sys.exit(1)
来源：http://zz.gzmigu.cn

PHP:  exit(1);
来源：http://jl.szxytkj.cn


<!-- 参考信息 -->