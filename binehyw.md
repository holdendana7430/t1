代发 wailian999

Ruby: s.scan(/error/i)
来源：http://vi.9csxet.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xq.yuntaijiaju.cn

[I08] 贪婪与非贪婪匹配
来源：http://ab.yuntaijiaju.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dd.shtwfgs.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xu.hnjuh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lk.shtwfgs.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wh.shtwfgs.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vv.jianghongdianzi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pi.szxytkj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fa.nszjky.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ia.szxytkj.cn

================================================================================
来源：http://et.hnjuh.cn

J. 日期与时间
来源：http://fq.yuexingan06.cn

================================================================================
来源：http://tv.9csxet.cn

[J01] 获取当前时间
来源：http://gg.nicolike.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://co.521024.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bo.hahajie.cn

JS:   new Date();  Date.now()
来源：http://vv.panjiajie.cn

TS:   new Date();  Date.now()
来源：http://go.newstarts.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ne.muxihuayi.cn

Go:   time.Now()
来源：http://cz.gzmigu.cn

Ruby: Time.now
来源：http://zd.9csxet.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pk.shxzukj.cn

[J02] 格式化输出
来源：http://cr.bookmarksfly.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tx.newstarts.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ee.panjiajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uc.yuexingan06.cn

TS:   d.toISOString()
来源：http://jq.shtwfgs.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bn.asd995.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fj.panjiajie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ho.jianghongdianzi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ss.haigaiapp.cn

[J03] 字符串解析为日期
来源：http://pg.huanxung.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zw.szsharing.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fp.nszjky.cn

JS:   new Date("2024-01-02")
来源：http://hj.gzmigu.cn

TS:   new Date("2024-01-02")
来源：http://eb.colortex.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mk.huixiangedu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://od.nszjky.cn

Ruby: Date.parse("2024-01-02")
来源：http://yh.newstarts.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ew.chemitech.net.cn

[J04] 时间戳与日期互转
来源：http://sf.wgjwhj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rw.yuexingan06.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ab.huixinmuqiang.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ba.huixiangedu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ld.bookmarksfly.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uy.haigaiapp.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mc.huanxung.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dl.asd995.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://le.haigaiapp.cn

[J05] 时间加减（加 7 天）
来源：http://cw.jctech888.com.cn

Py:   now + timedelta(days=7)
来源：http://id.szsharing.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zc.colortex.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hd.jctech888.com.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hn.yuntaijiaju.cn

Java: LocalDate.now().plusDays(7)
来源：http://ep.huixinmuqiang.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ib.bookmarksfly.cn

Ruby: Time.now + 7 * 86400
来源：http://np.asd995.cn

C#:   DateTime.Now.AddDays(7)
来源：http://if.asd995.cn

[J06] 计算两时间之差
来源：http://km.wgjwhj.cn

Py:   (end - start).total_seconds()
来源：http://ye.newstarts.cn

PHP:  $end->diff($start)->days;
来源：http://kg.haigaiapp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gr.gzmigu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gz.muxihuayi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gs.yuntaijiaju.cn

Go:   end.Sub(start).Hours()
来源：http://xq.asd995.cn

Ruby: end - start                 # 返回秒数
来源：http://vs.wgjwhj.cn

C#:   (end - start).TotalSeconds
来源：http://qd.panjiajie.cn

[J07] 比较两个日期
来源：http://kt.yuntaijiaju.cn

Py:   d1 < d2;  d1 == d2
来源：http://el.szsharing.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wh.nicolike.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bz.huixiangedu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://va.9csxet.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mf.yuntaijiaju.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uy.jianghongdianzi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://yt.huixiangedu.cn

C#:   d1 < d2;  d1 == d2
来源：http://hn.jctech888.com.cn

[J08] 提取年月日与星期
来源：http://rb.shxzukj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hr.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xl.shxzukj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hp.huanxung.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pq.panjiajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mt.huixinmuqiang.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tv.gzmigu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vp.hahajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xi.huixiangedu.cn

[J09] 时区处理
来源：http://tg.jianghongdianzi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zr.chemitech.net.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gy.shxzukj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zp.yuntaijiaju.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ql.jctech888.com.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gu.shtwfgs.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mv.chemitech.net.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jc.nicolike.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xy.hnjuh.cn

[J10] 取今天 / 本月第一天
来源：http://ie.521024.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vn.shxzskj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://eb.colortex.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sg.shxzskj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ri.panjiajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://of.gzmigu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jq.huanxung.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zo.shtwfgs.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xi.shxzskj.cn

================================================================================
来源：http://mu.shxzskj.cn

K. JSON 与序列化
来源：http://jy.shxzskj.cn

================================================================================
来源：http://yc.huanxung.cn

[K01] 对象转 JSON 字符串
来源：http://bv.nicolike.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ja.nicolike.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hl.jctech888.com.cn

JS:   JSON.stringify(obj)
来源：http://eu.nszjky.cn

TS:   JSON.stringify(obj)
来源：http://fq.gzmigu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://iq.521024.cn

Go:   json.Marshal(obj)
来源：http://gd.muxihuayi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ed.shxzskj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bo.wgjwhj.cn

[K02] JSON 字符串转对象
来源：http://zb.huixiangedu.cn

Py:   json.loads(s)
来源：http://ry.shxzukj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wt.lnxyls.cn

JS:   JSON.parse(s)
来源：http://ea.shtwfgs.cn

TS:   JSON.parse(s)
来源：http://if.wgjwhj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jl.szxytkj.cn

Go:   json.Unmarshal(data, &v)
来源：http://nq.szxytkj.cn

Ruby: JSON.parse(s)
来源：http://tp.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wf.bookmarksfly.cn

[K03] JSON 美化输出（带缩进）
来源：http://pa.521024.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lr.wgjwhj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://co.yuntaijiaju.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://we.yuntaijiaju.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://jy.jianghongdianzi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uo.gzmigu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dk.hahajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://oy.huanxung.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tf.colortex.cn

[K04] 读取 JSON 文件
来源：http://rp.hahajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nm.yuntaijiaju.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fi.asd995.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ox.newstarts.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ex.hnjuh.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kt.gzmigu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zt.muxihuayi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ug.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ou.nicolike.cn

[K05] 深拷贝对象
来源：http://kd.shtwfgs.cn

Py:   copy.deepcopy(obj)
来源：http://ws.wgjwhj.cn

PHP:  unserialize(serialize($obj));
来源：http://kv.muxihuayi.cn

JS:   structuredClone(obj)
来源：http://qa.nszjky.cn

TS:   structuredClone(obj)
来源：http://ax.gzmigu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zq.chemitech.net.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://if.szsharing.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ed.bjjhwx.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://el.jctech888.com.cn

[K06] 解析 URL 查询串
来源：http://gr.huixinmuqiang.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hf.newstarts.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lv.chemitech.net.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mf.newstarts.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qh.huixinmuqiang.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wu.haigaiapp.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mr.bookmarksfly.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sk.colortex.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vr.9csxet.cn

[K07] 进制转换
来源：http://qs.bjjhwx.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ng.nszjky.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rl.huanxung.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pr.shxzukj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gi.lnxyls.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ee.gzmigu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pt.szsharing.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://md.bjjhwx.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://eg.colortex.cn

[K08] 二进制序列化（非 JSON）
来源：http://fa.521024.cn

Py:   pickle.dumps(obj)
来源：http://qp.bookmarksfly.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://se.huanxung.cn

JS:   v8.serialize(obj)        // Node
来源：http://lp.panjiajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://ri.hahajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ks.huanxung.cn

Go:   encoding/gob
来源：http://id.521024.cn

Ruby: Marshal.dump(obj)
来源：http://zf.huixinmuqiang.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wb.szxytkj.cn

================================================================================
来源：http://dp.shtwfgs.cn

L. 网络请求
来源：http://cc.szxytkj.cn

================================================================================
来源：http://pv.jctech888.com.cn

[L01] 发送 GET 请求
来源：http://xg.lnxyls.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gc.szxytkj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ei.yuexingan06.cn

JS:   await fetch(url)
来源：http://nu.nszjky.cn

TS:   await fetch(url)
来源：http://bx.jctech888.com.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sb.huixiangedu.cn

Go:   resp, err := http.Get(url)
来源：http://xq.szsharing.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bo.hnjuh.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://im.shxzskj.cn

[L02] 发送 POST JSON
来源：http://vu.newstarts.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vb.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ba.jctech888.com.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://um.szxytkj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fl.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zz.szxytkj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tu.hahajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hm.shtwfgs.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vl.bookmarksfly.cn

[L03] 设置自定义请求头
来源：http://xo.lnxyls.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vj.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ym.bookmarksfly.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cj.yuexingan06.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jb.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://se.huixiangedu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fa.panjiajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fd.panjiajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qz.szsharing.cn

[L04] 设置超时
来源：http://gq.newstarts.cn

Py:   requests.get(url, timeout=5)
来源：http://dt.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://si.huixinmuqiang.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jv.gzmigu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lx.lnxyls.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wm.huixinmuqiang.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://op.chemitech.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wg.asd995.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://eb.hahajie.cn

[L05] 上传文件（multipart）
来源：http://ml.asd995.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ck.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ki.huixiangedu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://az.jctech888.com.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yc.shxzukj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nk.bjjhwx.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kf.jianghongdianzi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tp.gzmigu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fk.haigaiapp.cn

[L06] 解析响应为 JSON
来源：http://mn.shxzukj.cn

Py:   resp.json()
来源：http://xy.colortex.cn

PHP:  json_decode($body, true);
来源：http://tl.gzmigu.cn

JS:   await resp.json()
来源：http://bp.huanxung.cn

TS:   await resp.json()
来源：http://of.jianghongdianzi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ba.colortex.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kd.521024.cn

Ruby: JSON.parse(resp.body)
来源：http://ps.nicolike.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yj.lnxyls.cn

[L07] 处理 HTTP 状态码
来源：http://oj.szxytkj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rf.bookmarksfly.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://os.lnxyls.cn

JS:   resp.ok;  resp.status
来源：http://lf.asd995.cn

TS:   resp.ok;  resp.status
来源：http://pg.shtwfgs.cn

Java: resp.statusCode()
来源：http://mi.asd995.cn

Go:   resp.StatusCode
来源：http://yk.bjjhwx.cn

Ruby: resp.code.to_i
来源：http://mh.jctech888.com.cn

C#:   (int)resp.StatusCode
来源：http://bm.newstarts.cn

[L08] 并发请求多个地址
来源：http://lp.bookmarksfly.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xu.jctech888.com.cn

PHP:  curl_multi_init() 系列
来源：http://cs.newstarts.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fy.szsharing.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dw.szxytkj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lh.szxytkj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kt.9csxet.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yp.muxihuayi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://de.muxihuayi.cn

================================================================================
来源：http://mj.colortex.cn

M. 命令行 / 进程 / 环境
来源：http://pa.9csxet.cn

================================================================================
来源：http://gz.huixiangedu.cn

[M01] 读取命令行参数
来源：http://xu.asd995.cn

Py:   sys.argv[1:]
来源：http://jg.shxzskj.cn

PHP:  $argv;  $argc;
来源：http://kx.bjjhwx.cn

JS:   process.argv.slice(2)
来源：http://re.asd995.cn

TS:   process.argv.slice(2)
来源：http://fd.nszjky.cn

Java: args 数组（main 方法参数）
来源：http://ij.nszjky.cn

Go:   os.Args[1:]
来源：http://vv.szsharing.cn

Ruby: ARGV
来源：http://lu.lnxyls.cn

C#:   args 数组（Main 方法参数）
来源：http://ah.wgjwhj.cn

[M02] 读取环境变量
来源：http://ji.hahajie.cn

Py:   os.environ.get("HOME")
来源：http://ud.9csxet.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zo.nicolike.cn

JS:   process.env.HOME
来源：http://zt.shxzukj.cn

TS:   process.env.HOME
来源：http://yi.hnjuh.cn

Java: System.getenv("HOME")
来源：http://ox.jianghongdianzi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gc.colortex.cn

Ruby: ENV["HOME"]
来源：http://jq.wgjwhj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fn.huixiangedu.cn

[M03] 执行外部命令
来源：http://dd.huixinmuqiang.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ev.yuexingan06.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pl.jctech888.com.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ll.bookmarksfly.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gj.panjiajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bk.nicolike.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hf.yuexingan06.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kv.huixinmuqiang.cn

C#:   Process.Start("ls", "-l");
来源：http://mm.yuntaijiaju.cn

[M04] 获取当前工作目录
来源：http://pa.nicolike.cn

Py:   os.getcwd()
来源：http://ev.lnxyls.cn

PHP:  getcwd();
来源：http://ct.hnjuh.cn

JS:   process.cwd()
来源：http://mt.chemitech.net.cn

TS:   process.cwd()
来源：http://ru.bookmarksfly.cn

Java: Path.of("").toAbsolutePath()
来源：http://of.9csxet.cn

Go:   os.Getwd()
来源：http://at.nszjky.cn

Ruby: Dir.pwd
来源：http://qx.nszjky.cn

C#:   Directory.GetCurrentDirectory()
来源：http://og.bookmarksfly.cn

[M05] 设置退出码
来源：http://rm.haigaiapp.cn

Py:   sys.exit(1)
来源：http://pn.yuexingan06.cn

PHP:  exit(1);
来源：http://lw.jctech888.com.cn

JS:   process.exit(1)
来源：http://gt.shtwfgs.cn

TS:   process.exit(1)
来源：http://fu.chemitech.net.cn

Java: System.exit(1)
来源：http://xp.nicolike.cn

Go:   os.Exit(1)
来源：http://uf.huixinmuqiang.cn


<!-- 参考信息 -->