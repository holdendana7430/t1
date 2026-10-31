代发 wailian999

Ruby: s.scan(/error/i)
来源：http://bc.shxzskj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dt.bjjhwx.cn

[I08] 贪婪与非贪婪匹配
来源：http://hc.gzmigu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nu.jctech888.com.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bh.huixiangedu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sa.panjiajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pi.panjiajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xi.shxzukj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://et.huixiangedu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ds.huixiangedu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lc.haigaiapp.cn

================================================================================
来源：http://wj.yuexingan06.cn

J. 日期与时间
来源：http://hz.nszjky.cn

================================================================================
来源：http://li.bjjhwx.cn

[J01] 获取当前时间
来源：http://sl.hnjuh.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://dr.nszjky.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fu.asd995.cn

JS:   new Date();  Date.now()
来源：http://fg.asd995.cn

TS:   new Date();  Date.now()
来源：http://rg.521024.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qz.gzmigu.cn

Go:   time.Now()
来源：http://am.hnjuh.cn

Ruby: Time.now
来源：http://lb.yuexingan06.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://be.shxzskj.cn

[J02] 格式化输出
来源：http://ei.jianghongdianzi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kl.huixiangedu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gj.gzmigu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bo.shxzskj.cn

TS:   d.toISOString()
来源：http://nz.bjjhwx.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vn.9csxet.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://eg.szsharing.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ap.asd995.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jc.szsharing.cn

[J03] 字符串解析为日期
来源：http://xz.yuexingan06.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yb.bjjhwx.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bx.lnxyls.cn

JS:   new Date("2024-01-02")
来源：http://ir.9csxet.cn

TS:   new Date("2024-01-02")
来源：http://wy.chemitech.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://tq.huanxung.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ld.huixiangedu.cn

Ruby: Date.parse("2024-01-02")
来源：http://et.gzmigu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.shxzukj.cn

[J04] 时间戳与日期互转
来源：http://ht.haigaiapp.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://oc.nicolike.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://oh.huixinmuqiang.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ej.nicolike.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://nt.huixiangedu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gx.chemitech.net.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gm.nicolike.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qn.jctech888.com.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gz.hnjuh.cn

[J05] 时间加减（加 7 天）
来源：http://re.bjjhwx.cn

Py:   now + timedelta(days=7)
来源：http://bh.bjjhwx.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://he.bookmarksfly.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gq.huixiangedu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fp.wgjwhj.cn

Java: LocalDate.now().plusDays(7)
来源：http://lm.9csxet.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yv.nicolike.cn

Ruby: Time.now + 7 * 86400
来源：http://nb.haigaiapp.cn

C#:   DateTime.Now.AddDays(7)
来源：http://yu.bookmarksfly.cn

[J06] 计算两时间之差
来源：http://zx.szsharing.cn

Py:   (end - start).total_seconds()
来源：http://rj.shxzskj.cn

PHP:  $end->diff($start)->days;
来源：http://ro.haigaiapp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yf.wgjwhj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mk.hahajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://my.newstarts.cn

Go:   end.Sub(start).Hours()
来源：http://ig.chemitech.net.cn

Ruby: end - start                 # 返回秒数
来源：http://od.yuntaijiaju.cn

C#:   (end - start).TotalSeconds
来源：http://ir.chemitech.net.cn

[J07] 比较两个日期
来源：http://kr.newstarts.cn

Py:   d1 < d2;  d1 == d2
来源：http://br.9csxet.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ob.asd995.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ia.muxihuayi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://cj.haigaiapp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sg.huixiangedu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lg.521024.cn

Ruby: d1 < d2;  d1 == d2
来源：http://rs.jctech888.com.cn

C#:   d1 < d2;  d1 == d2
来源：http://rw.haigaiapp.cn

[J08] 提取年月日与星期
来源：http://sp.haigaiapp.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://oi.jctech888.com.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cj.hahajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://km.wgjwhj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yq.huanxung.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ux.nicolike.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cp.chemitech.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://si.shxzukj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jm.muxihuayi.cn

[J09] 时区处理
来源：http://za.huanxung.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ny.haigaiapp.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hn.bookmarksfly.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ra.lnxyls.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://es.shtwfgs.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wt.shtwfgs.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qk.shtwfgs.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://sh.wgjwhj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hw.hahajie.cn

[J10] 取今天 / 本月第一天
来源：http://ax.colortex.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://aq.9csxet.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mz.newstarts.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hd.jctech888.com.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://au.newstarts.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hx.bjjhwx.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tt.lnxyls.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wk.bookmarksfly.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ti.yuexingan06.cn

================================================================================
来源：http://nw.shxzskj.cn

K. JSON 与序列化
来源：http://be.shxzukj.cn

================================================================================
来源：http://za.yuexingan06.cn

[K01] 对象转 JSON 字符串
来源：http://qm.lnxyls.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ie.hahajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pi.hahajie.cn

JS:   JSON.stringify(obj)
来源：http://bt.yuexingan06.cn

TS:   JSON.stringify(obj)
来源：http://wq.shxzskj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ul.gzmigu.cn

Go:   json.Marshal(obj)
来源：http://rg.yuexingan06.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zg.lnxyls.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xl.muxihuayi.cn

[K02] JSON 字符串转对象
来源：http://fl.521024.cn

Py:   json.loads(s)
来源：http://ia.szxytkj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xo.hnjuh.cn

JS:   JSON.parse(s)
来源：http://dx.521024.cn

TS:   JSON.parse(s)
来源：http://yg.hnjuh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cj.szxytkj.cn

Go:   json.Unmarshal(data, &v)
来源：http://fv.muxihuayi.cn

Ruby: JSON.parse(s)
来源：http://jv.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://we.szxytkj.cn

[K03] JSON 美化输出（带缩进）
来源：http://yv.szsharing.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://iv.panjiajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://me.wgjwhj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ww.haigaiapp.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://am.muxihuayi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vc.jctech888.com.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jz.jctech888.com.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xf.lnxyls.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nc.haigaiapp.cn

[K04] 读取 JSON 文件
来源：http://cw.newstarts.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rr.haigaiapp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fg.panjiajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eu.nszjky.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iq.wgjwhj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://oi.newstarts.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ka.nicolike.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ok.521024.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://so.muxihuayi.cn

[K05] 深拷贝对象
来源：http://qr.chemitech.net.cn

Py:   copy.deepcopy(obj)
来源：http://jb.colortex.cn

PHP:  unserialize(serialize($obj));
来源：http://dt.9csxet.cn

JS:   structuredClone(obj)
来源：http://uj.shxzskj.cn

TS:   structuredClone(obj)
来源：http://oh.lnxyls.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gc.nszjky.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yk.lnxyls.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tj.chemitech.net.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wo.asd995.cn

[K06] 解析 URL 查询串
来源：http://pe.shtwfgs.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kw.hnjuh.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://uh.szxytkj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gm.colortex.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rf.nszjky.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rd.9csxet.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hp.haigaiapp.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ks.huanxung.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://su.9csxet.cn

[K07] 进制转换
来源：http://rk.yuntaijiaju.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://so.szxytkj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pe.colortex.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tj.yuntaijiaju.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sg.bjjhwx.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ns.haigaiapp.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://se.huixinmuqiang.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jj.521024.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yi.asd995.cn

[K08] 二进制序列化（非 JSON）
来源：http://yx.lnxyls.cn

Py:   pickle.dumps(obj)
来源：http://sw.szxytkj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://qe.huixiangedu.cn

JS:   v8.serialize(obj)        // Node
来源：http://jz.hnjuh.cn

TS:   v8.serialize(obj)        // Node
来源：http://iv.shxzukj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ei.panjiajie.cn

Go:   encoding/gob
来源：http://dj.shxzskj.cn

Ruby: Marshal.dump(obj)
来源：http://uy.jctech888.com.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xv.bjjhwx.cn

================================================================================
来源：http://di.chemitech.net.cn

L. 网络请求
来源：http://uz.chemitech.net.cn

================================================================================
来源：http://rd.szxytkj.cn

[L01] 发送 GET 请求
来源：http://qh.bookmarksfly.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://na.nszjky.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ez.huixinmuqiang.cn

JS:   await fetch(url)
来源：http://an.shxzskj.cn

TS:   await fetch(url)
来源：http://nv.jctech888.com.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dq.nicolike.cn

Go:   resp, err := http.Get(url)
来源：http://uw.wgjwhj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://li.wgjwhj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sv.shxzskj.cn

[L02] 发送 POST JSON
来源：http://lc.shxzskj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fk.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vt.szxytkj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://if.haigaiapp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pc.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fl.chemitech.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vh.shxzukj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mu.colortex.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://el.shxzukj.cn

[L03] 设置自定义请求头
来源：http://ot.hnjuh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zb.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fv.muxihuayi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dm.yuntaijiaju.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ws.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://go.wgjwhj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xl.muxihuayi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ln.521024.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bp.asd995.cn

[L04] 设置超时
来源：http://ac.yuntaijiaju.cn

Py:   requests.get(url, timeout=5)
来源：http://tk.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zy.wgjwhj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ns.huixinmuqiang.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kv.shxzukj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ae.szsharing.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yc.colortex.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fi.nicolike.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dn.bjjhwx.cn

[L05] 上传文件（multipart）
来源：http://id.muxihuayi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gz.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ce.jianghongdianzi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dm.gzmigu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://io.muxihuayi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ay.chemitech.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fp.bjjhwx.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://it.wgjwhj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://to.jctech888.com.cn

[L06] 解析响应为 JSON
来源：http://fo.szsharing.cn

Py:   resp.json()
来源：http://zs.colortex.cn

PHP:  json_decode($body, true);
来源：http://ml.jianghongdianzi.cn

JS:   await resp.json()
来源：http://vi.shxzskj.cn

TS:   await resp.json()
来源：http://ax.shxzukj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://si.haigaiapp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ak.yuntaijiaju.cn

Ruby: JSON.parse(resp.body)
来源：http://hx.bookmarksfly.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://je.hnjuh.cn

[L07] 处理 HTTP 状态码
来源：http://sb.nicolike.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ec.chemitech.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tp.nszjky.cn

JS:   resp.ok;  resp.status
来源：http://oa.9csxet.cn

TS:   resp.ok;  resp.status
来源：http://ir.nicolike.cn

Java: resp.statusCode()
来源：http://gh.colortex.cn

Go:   resp.StatusCode
来源：http://xh.hahajie.cn

Ruby: resp.code.to_i
来源：http://ro.jctech888.com.cn

C#:   (int)resp.StatusCode
来源：http://gb.szxytkj.cn

[L08] 并发请求多个地址
来源：http://ld.shtwfgs.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://md.wgjwhj.cn

PHP:  curl_multi_init() 系列
来源：http://cl.nszjky.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://av.hnjuh.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://we.jctech888.com.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uc.lnxyls.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://af.521024.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jx.bookmarksfly.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ud.shxzukj.cn

================================================================================
来源：http://he.nszjky.cn

M. 命令行 / 进程 / 环境
来源：http://hr.shtwfgs.cn

================================================================================
来源：http://jy.lnxyls.cn

[M01] 读取命令行参数
来源：http://ut.lnxyls.cn

Py:   sys.argv[1:]
来源：http://zg.huixinmuqiang.cn

PHP:  $argv;  $argc;
来源：http://rd.newstarts.cn

JS:   process.argv.slice(2)
来源：http://sz.muxihuayi.cn

TS:   process.argv.slice(2)
来源：http://jn.bookmarksfly.cn

Java: args 数组（main 方法参数）
来源：http://vv.chemitech.net.cn

Go:   os.Args[1:]
来源：http://vv.bjjhwx.cn

Ruby: ARGV
来源：http://wg.hnjuh.cn

C#:   args 数组（Main 方法参数）
来源：http://wu.gzmigu.cn

[M02] 读取环境变量
来源：http://hd.wgjwhj.cn

Py:   os.environ.get("HOME")
来源：http://an.chemitech.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ua.muxihuayi.cn

JS:   process.env.HOME
来源：http://pu.chemitech.net.cn

TS:   process.env.HOME
来源：http://hn.newstarts.cn

Java: System.getenv("HOME")
来源：http://tq.yuntaijiaju.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lx.shxzskj.cn

Ruby: ENV["HOME"]
来源：http://lj.asd995.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cf.haigaiapp.cn

[M03] 执行外部命令
来源：http://gz.newstarts.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nc.jianghongdianzi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bx.lnxyls.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ol.nicolike.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tm.newstarts.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ml.jctech888.com.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nf.bookmarksfly.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ej.haigaiapp.cn

C#:   Process.Start("ls", "-l");
来源：http://em.9csxet.cn

[M04] 获取当前工作目录
来源：http://hw.nicolike.cn

Py:   os.getcwd()
来源：http://wy.lnxyls.cn

PHP:  getcwd();
来源：http://iy.nicolike.cn

JS:   process.cwd()
来源：http://dm.szxytkj.cn

TS:   process.cwd()
来源：http://gh.nszjky.cn

Java: Path.of("").toAbsolutePath()
来源：http://ej.bjjhwx.cn

Go:   os.Getwd()
来源：http://md.panjiajie.cn

Ruby: Dir.pwd
来源：http://jb.szxytkj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sa.lnxyls.cn

[M05] 设置退出码
来源：http://qj.szxytkj.cn

Py:   sys.exit(1)
来源：http://qy.huixinmuqiang.cn

PHP:  exit(1);
来源：http://pb.huixinmuqiang.cn

JS:   process.exit(1)
来源：http://hd.panjiajie.cn

TS:   process.exit(1)
来源：http://dy.shxzukj.cn

Java: System.exit(1)
来源：http://lf.szxytkj.cn

Go:   os.Exit(1)
来源：http://qi.shxzskj.cn


<!-- 参考信息 -->