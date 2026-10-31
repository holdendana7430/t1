代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://as.gzmigu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wn.muxihuayi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ai.lnxyls.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://li.hnjuh.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vm.shtwfgs.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://sp.bjjhwx.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lr.nszjky.cn

================================================================================
来源：http://cj.yuexingan06.cn

J. 日期与时间
来源：http://fj.szsharing.cn

================================================================================
来源：http://ge.huixinmuqiang.cn

[J01] 获取当前时间
来源：http://dg.colortex.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://om.shtwfgs.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://my.colortex.cn

JS:   new Date();  Date.now()
来源：http://sk.wgjwhj.cn

TS:   new Date();  Date.now()
来源：http://kr.panjiajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zw.9csxet.cn

Go:   time.Now()
来源：http://il.nicolike.cn

Ruby: Time.now
来源：http://bj.nicolike.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ae.gzmigu.cn

[J02] 格式化输出
来源：http://gk.huanxung.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vk.shxzskj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wc.shxzukj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nm.huanxung.cn

TS:   d.toISOString()
来源：http://yi.jctech888.com.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://eb.huixiangedu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bn.yuexingan06.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mq.yuntaijiaju.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uy.yuntaijiaju.cn

[J03] 字符串解析为日期
来源：http://eu.9csxet.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jg.muxihuayi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://am.szsharing.cn

JS:   new Date("2024-01-02")
来源：http://hc.colortex.cn

TS:   new Date("2024-01-02")
来源：http://kq.521024.cn

Java: LocalDate.parse("2024-01-02")
来源：http://kw.lnxyls.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cr.newstarts.cn

Ruby: Date.parse("2024-01-02")
来源：http://qr.chemitech.net.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cs.yuntaijiaju.cn

[J04] 时间戳与日期互转
来源：http://xg.gzmigu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uf.jianghongdianzi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ta.huixinmuqiang.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nd.nicolike.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://eb.hahajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ou.shxzskj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cd.hahajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://me.shxzskj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xu.yuexingan06.cn

[J05] 时间加减（加 7 天）
来源：http://cd.asd995.cn

Py:   now + timedelta(days=7)
来源：http://zp.newstarts.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lr.jctech888.com.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vw.haigaiapp.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://io.szsharing.cn

Java: LocalDate.now().plusDays(7)
来源：http://ka.szsharing.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qk.shtwfgs.cn

Ruby: Time.now + 7 * 86400
来源：http://nn.shtwfgs.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ar.lnxyls.cn

[J06] 计算两时间之差
来源：http://vr.nszjky.cn

Py:   (end - start).total_seconds()
来源：http://wc.chemitech.net.cn

PHP:  $end->diff($start)->days;
来源：http://fk.jianghongdianzi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zk.hahajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ku.haigaiapp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ze.szsharing.cn

Go:   end.Sub(start).Hours()
来源：http://on.gzmigu.cn

Ruby: end - start                 # 返回秒数
来源：http://le.nszjky.cn

C#:   (end - start).TotalSeconds
来源：http://ez.shxzskj.cn

[J07] 比较两个日期
来源：http://hg.nicolike.cn

Py:   d1 < d2;  d1 == d2
来源：http://cb.jianghongdianzi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fk.szsharing.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bj.newstarts.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xo.hnjuh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zy.hahajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://aj.szxytkj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zw.jctech888.com.cn

C#:   d1 < d2;  d1 == d2
来源：http://bz.9csxet.cn

[J08] 提取年月日与星期
来源：http://qs.panjiajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kx.muxihuayi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zg.asd995.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ga.gzmigu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xm.shtwfgs.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bx.newstarts.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kh.shxzukj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://an.nicolike.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uh.nszjky.cn

[J09] 时区处理
来源：http://zx.bjjhwx.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rh.bookmarksfly.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zl.521024.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nf.huanxung.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ck.hahajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gi.lnxyls.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gs.huanxung.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vr.szxytkj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ji.wgjwhj.cn

[J10] 取今天 / 本月第一天
来源：http://hx.wgjwhj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://od.asd995.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://iw.yuntaijiaju.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xg.hnjuh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yy.szxytkj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ch.newstarts.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ne.asd995.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kh.huixiangedu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bv.panjiajie.cn

================================================================================
来源：http://no.lnxyls.cn

K. JSON 与序列化
来源：http://ja.huanxung.cn

================================================================================
来源：http://jb.bjjhwx.cn

[K01] 对象转 JSON 字符串
来源：http://ep.szsharing.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://iq.asd995.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://sn.shtwfgs.cn

JS:   JSON.stringify(obj)
来源：http://fy.chemitech.net.cn

TS:   JSON.stringify(obj)
来源：http://hv.hahajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cx.521024.cn

Go:   json.Marshal(obj)
来源：http://sx.haigaiapp.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hz.521024.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ck.gzmigu.cn

[K02] JSON 字符串转对象
来源：http://wd.shtwfgs.cn

Py:   json.loads(s)
来源：http://fw.shxzskj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ab.hahajie.cn

JS:   JSON.parse(s)
来源：http://pi.bjjhwx.cn

TS:   JSON.parse(s)
来源：http://la.shxzskj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ej.hahajie.cn

Go:   json.Unmarshal(data, &v)
来源：http://oc.huixiangedu.cn

Ruby: JSON.parse(s)
来源：http://mc.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jh.shtwfgs.cn

[K03] JSON 美化输出（带缩进）
来源：http://zy.huixiangedu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uf.haigaiapp.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://da.huixiangedu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://js.lnxyls.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wx.bookmarksfly.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dq.szxytkj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dt.shtwfgs.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kl.hnjuh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zm.lnxyls.cn

[K04] 读取 JSON 文件
来源：http://hu.nicolike.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mn.haigaiapp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ka.shtwfgs.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://po.nszjky.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hf.wgjwhj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://er.hahajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xw.521024.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ai.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pm.hnjuh.cn

[K05] 深拷贝对象
来源：http://iy.yuntaijiaju.cn

Py:   copy.deepcopy(obj)
来源：http://nu.shtwfgs.cn

PHP:  unserialize(serialize($obj));
来源：http://sw.jctech888.com.cn

JS:   structuredClone(obj)
来源：http://fh.shtwfgs.cn

TS:   structuredClone(obj)
来源：http://kj.huanxung.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dp.bookmarksfly.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bb.hahajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hc.asd995.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://iv.jianghongdianzi.cn

[K06] 解析 URL 查询串
来源：http://ln.521024.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://es.shtwfgs.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bz.nicolike.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iq.szsharing.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pz.huixinmuqiang.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://id.huanxung.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ru.hnjuh.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nu.bjjhwx.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uq.yuntaijiaju.cn

[K07] 进制转换
来源：http://ae.chemitech.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wl.bookmarksfly.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ph.9csxet.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qv.asd995.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wy.jctech888.com.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ms.muxihuayi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vf.nicolike.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cz.nszjky.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cm.yuexingan06.cn

[K08] 二进制序列化（非 JSON）
来源：http://sw.shxzskj.cn

Py:   pickle.dumps(obj)
来源：http://gt.9csxet.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ia.hahajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://hv.szsharing.cn

TS:   v8.serialize(obj)        // Node
来源：http://gm.nszjky.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rh.jianghongdianzi.cn

Go:   encoding/gob
来源：http://dw.newstarts.cn

Ruby: Marshal.dump(obj)
来源：http://ym.jianghongdianzi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vh.9csxet.cn

================================================================================
来源：http://zx.yuexingan06.cn

L. 网络请求
来源：http://lt.shxzskj.cn

================================================================================
来源：http://gg.asd995.cn

[L01] 发送 GET 请求
来源：http://zt.yuexingan06.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dm.colortex.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rc.yuntaijiaju.cn

JS:   await fetch(url)
来源：http://ab.haigaiapp.cn

TS:   await fetch(url)
来源：http://we.muxihuayi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tw.jctech888.com.cn

Go:   resp, err := http.Get(url)
来源：http://bx.huixinmuqiang.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://lf.bookmarksfly.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bg.bookmarksfly.cn

[L02] 发送 POST JSON
来源：http://kj.szxytkj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ns.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cv.521024.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dj.huanxung.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hd.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ty.wgjwhj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sp.jianghongdianzi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://co.asd995.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vf.panjiajie.cn

[L03] 设置自定义请求头
来源：http://jz.colortex.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jm.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ql.hnjuh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oq.yuexingan06.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dg.521024.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zj.yuexingan06.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rq.szxytkj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hn.hnjuh.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bg.szsharing.cn

[L04] 设置超时
来源：http://go.chemitech.net.cn

Py:   requests.get(url, timeout=5)
来源：http://ew.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ud.panjiajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gt.jctech888.com.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ie.huixiangedu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ne.lnxyls.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zc.huixinmuqiang.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nn.colortex.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jl.szxytkj.cn

[L05] 上传文件（multipart）
来源：http://dh.nicolike.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gv.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tq.chemitech.net.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://px.bjjhwx.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jl.colortex.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ey.huixinmuqiang.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xy.gzmigu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ix.nszjky.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kw.haigaiapp.cn

[L06] 解析响应为 JSON
来源：http://yl.panjiajie.cn

Py:   resp.json()
来源：http://ty.wgjwhj.cn

PHP:  json_decode($body, true);
来源：http://yw.asd995.cn

JS:   await resp.json()
来源：http://qd.yuexingan06.cn

TS:   await resp.json()
来源：http://lu.bookmarksfly.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://af.huixiangedu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xb.521024.cn

Ruby: JSON.parse(resp.body)
来源：http://xg.bookmarksfly.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pq.panjiajie.cn

[L07] 处理 HTTP 状态码
来源：http://nj.shxzukj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hb.gzmigu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hl.jianghongdianzi.cn

JS:   resp.ok;  resp.status
来源：http://vz.hahajie.cn

TS:   resp.ok;  resp.status
来源：http://dt.hnjuh.cn

Java: resp.statusCode()
来源：http://qe.jianghongdianzi.cn

Go:   resp.StatusCode
来源：http://td.huixinmuqiang.cn

Ruby: resp.code.to_i
来源：http://ge.huanxung.cn

C#:   (int)resp.StatusCode
来源：http://fv.szxytkj.cn

[L08] 并发请求多个地址
来源：http://of.huanxung.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xo.jctech888.com.cn

PHP:  curl_multi_init() 系列
来源：http://sq.shtwfgs.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qd.haigaiapp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nf.haigaiapp.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ob.jctech888.com.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://if.hnjuh.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mq.asd995.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://im.bookmarksfly.cn

================================================================================
来源：http://rg.panjiajie.cn

M. 命令行 / 进程 / 环境
来源：http://tn.szxytkj.cn

================================================================================
来源：http://yf.hahajie.cn

[M01] 读取命令行参数
来源：http://xh.haigaiapp.cn

Py:   sys.argv[1:]
来源：http://oa.shxzskj.cn

PHP:  $argv;  $argc;
来源：http://kn.huixinmuqiang.cn

JS:   process.argv.slice(2)
来源：http://we.521024.cn

TS:   process.argv.slice(2)
来源：http://nn.chemitech.net.cn

Java: args 数组（main 方法参数）
来源：http://kb.yuntaijiaju.cn

Go:   os.Args[1:]
来源：http://rc.panjiajie.cn

Ruby: ARGV
来源：http://lc.huixiangedu.cn

C#:   args 数组（Main 方法参数）
来源：http://vb.9csxet.cn

[M02] 读取环境变量
来源：http://ge.jctech888.com.cn

Py:   os.environ.get("HOME")
来源：http://lr.shxzukj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pn.jctech888.com.cn

JS:   process.env.HOME
来源：http://kb.yuntaijiaju.cn

TS:   process.env.HOME
来源：http://yj.huixiangedu.cn

Java: System.getenv("HOME")
来源：http://nj.huanxung.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wk.shtwfgs.cn

Ruby: ENV["HOME"]
来源：http://uv.gzmigu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zx.nszjky.cn

[M03] 执行外部命令
来源：http://ll.yuexingan06.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mb.haigaiapp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ee.hnjuh.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://tw.jianghongdianzi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xm.huixiangedu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hw.huixiangedu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vc.9csxet.cn

Ruby: system("ls -l");  `ls -l`
来源：http://cz.lnxyls.cn

C#:   Process.Start("ls", "-l");
来源：http://km.chemitech.net.cn

[M04] 获取当前工作目录
来源：http://cn.huanxung.cn

Py:   os.getcwd()
来源：http://uo.huixinmuqiang.cn

PHP:  getcwd();
来源：http://wl.hnjuh.cn

JS:   process.cwd()
来源：http://sk.nszjky.cn

TS:   process.cwd()
来源：http://gy.asd995.cn

Java: Path.of("").toAbsolutePath()
来源：http://yr.jianghongdianzi.cn

Go:   os.Getwd()
来源：http://lf.wgjwhj.cn

Ruby: Dir.pwd
来源：http://td.muxihuayi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jt.huanxung.cn

[M05] 设置退出码
来源：http://zk.lnxyls.cn

Py:   sys.exit(1)
来源：http://gp.huixinmuqiang.cn

PHP:  exit(1);
来源：http://yc.yuexingan06.cn

JS:   process.exit(1)
来源：http://rg.9csxet.cn

TS:   process.exit(1)
来源：http://xa.lnxyls.cn

Java: System.exit(1)
来源：http://el.shxzskj.cn

Go:   os.Exit(1)
来源：http://na.shtwfgs.cn

Ruby: exit 1
来源：http://ol.nicolike.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ph.bjjhwx.cn

[M06] 向标准错误输出
来源：http://oa.shtwfgs.cn

Py:   print("err", file=sys.stderr)
来源：http://zd.hnjuh.cn


<!-- 参考信息 -->