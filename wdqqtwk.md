代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kq.9csxet.cn

TS:   /error/gim
来源：http://cd.huixiangedu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fu.bookmarksfly.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://aq.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://sa.jianghongdianzi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lj.muxihuayi.cn

[I08] 贪婪与非贪婪匹配
来源：http://aq.colortex.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ka.lnxyls.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ax.huixiangedu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cn.hahajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xe.yuntaijiaju.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qv.521024.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kj.hahajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pm.newstarts.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gx.newstarts.cn

================================================================================
来源：http://dn.bookmarksfly.cn

J. 日期与时间
来源：http://dw.nszjky.cn

================================================================================
来源：http://ma.panjiajie.cn

[J01] 获取当前时间
来源：http://ke.muxihuayi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zx.panjiajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wg.gzmigu.cn

JS:   new Date();  Date.now()
来源：http://hs.szxytkj.cn

TS:   new Date();  Date.now()
来源：http://jg.yuntaijiaju.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ka.jctech888.com.cn

Go:   time.Now()
来源：http://lx.nicolike.cn

Ruby: Time.now
来源：http://wv.9csxet.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dd.521024.cn

[J02] 格式化输出
来源：http://dt.gzmigu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yk.jianghongdianzi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mh.nszjky.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://eu.colortex.cn

TS:   d.toISOString()
来源：http://ck.shxzukj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://aj.hahajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qr.521024.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dn.bookmarksfly.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pv.szsharing.cn

[J03] 字符串解析为日期
来源：http://tx.shtwfgs.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xr.huanxung.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nc.nszjky.cn

JS:   new Date("2024-01-02")
来源：http://kz.huanxung.cn

TS:   new Date("2024-01-02")
来源：http://eg.wgjwhj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://eu.nicolike.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vr.gzmigu.cn

Ruby: Date.parse("2024-01-02")
来源：http://ll.521024.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gm.szsharing.cn

[J04] 时间戳与日期互转
来源：http://mc.hnjuh.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://oe.bjjhwx.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xs.jianghongdianzi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hj.jianghongdianzi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vj.hahajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ke.haigaiapp.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nr.yuntaijiaju.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kl.szxytkj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dt.huixinmuqiang.cn

[J05] 时间加减（加 7 天）
来源：http://st.shxzskj.cn

Py:   now + timedelta(days=7)
来源：http://df.wgjwhj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ng.huixinmuqiang.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mb.nszjky.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://me.shtwfgs.cn

Java: LocalDate.now().plusDays(7)
来源：http://rr.bjjhwx.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ll.jianghongdianzi.cn

Ruby: Time.now + 7 * 86400
来源：http://is.yuntaijiaju.cn

C#:   DateTime.Now.AddDays(7)
来源：http://lv.huixinmuqiang.cn

[J06] 计算两时间之差
来源：http://yg.jianghongdianzi.cn

Py:   (end - start).total_seconds()
来源：http://vm.lnxyls.cn

PHP:  $end->diff($start)->days;
来源：http://gl.hahajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zk.asd995.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://os.hahajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lm.jianghongdianzi.cn

Go:   end.Sub(start).Hours()
来源：http://ss.muxihuayi.cn

Ruby: end - start                 # 返回秒数
来源：http://is.521024.cn

C#:   (end - start).TotalSeconds
来源：http://lu.9csxet.cn

[J07] 比较两个日期
来源：http://ii.szxytkj.cn

Py:   d1 < d2;  d1 == d2
来源：http://kl.shxzskj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ja.newstarts.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mw.huixiangedu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://sj.huanxung.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ts.panjiajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tc.haigaiapp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://rl.muxihuayi.cn

C#:   d1 < d2;  d1 == d2
来源：http://gy.szsharing.cn

[J08] 提取年月日与星期
来源：http://ya.hahajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fn.huanxung.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://au.gzmigu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cj.haigaiapp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xu.jctech888.com.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qb.colortex.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fs.haigaiapp.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gr.chemitech.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yd.haigaiapp.cn

[J09] 时区处理
来源：http://be.nicolike.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ve.jianghongdianzi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xo.shxzskj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gk.nicolike.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oz.shxzukj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qu.hahajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zg.newstarts.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ee.nszjky.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ag.yuntaijiaju.cn

[J10] 取今天 / 本月第一天
来源：http://tf.chemitech.net.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ye.asd995.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hq.szxytkj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ff.bjjhwx.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dt.newstarts.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jc.yuntaijiaju.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tb.asd995.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://em.hahajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dv.shxzskj.cn

================================================================================
来源：http://vc.shxzskj.cn

K. JSON 与序列化
来源：http://xi.muxihuayi.cn

================================================================================
来源：http://jd.hnjuh.cn

[K01] 对象转 JSON 字符串
来源：http://dg.huanxung.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yw.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oa.nszjky.cn

JS:   JSON.stringify(obj)
来源：http://ev.szxytkj.cn

TS:   JSON.stringify(obj)
来源：http://hy.colortex.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jh.jctech888.com.cn

Go:   json.Marshal(obj)
来源：http://wa.521024.cn

Ruby: obj.to_json                                     // require "json"
来源：http://at.szsharing.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fl.hahajie.cn

[K02] JSON 字符串转对象
来源：http://vx.szsharing.cn

Py:   json.loads(s)
来源：http://xc.jianghongdianzi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pb.yuexingan06.cn

JS:   JSON.parse(s)
来源：http://aa.bjjhwx.cn

TS:   JSON.parse(s)
来源：http://bi.hahajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ko.panjiajie.cn

Go:   json.Unmarshal(data, &v)
来源：http://aq.newstarts.cn

Ruby: JSON.parse(s)
来源：http://eq.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://az.shxzukj.cn

[K03] JSON 美化输出（带缩进）
来源：http://tu.szxytkj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ad.szsharing.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gu.jctech888.com.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://lk.szsharing.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://en.jctech888.com.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gz.jianghongdianzi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ha.asd995.cn

Ruby: JSON.pretty_generate(obj)
来源：http://be.hnjuh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uu.nicolike.cn

[K04] 读取 JSON 文件
来源：http://yw.nszjky.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nj.9csxet.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zi.szxytkj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sh.colortex.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ln.huixinmuqiang.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wp.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://iv.shxzskj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rw.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jw.hnjuh.cn

[K05] 深拷贝对象
来源：http://zj.bookmarksfly.cn

Py:   copy.deepcopy(obj)
来源：http://aw.shxzukj.cn

PHP:  unserialize(serialize($obj));
来源：http://zi.bjjhwx.cn

JS:   structuredClone(obj)
来源：http://su.9csxet.cn

TS:   structuredClone(obj)
来源：http://zv.szsharing.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://km.9csxet.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ey.szsharing.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jh.szxytkj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://op.shxzskj.cn

[K06] 解析 URL 查询串
来源：http://mn.lnxyls.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ll.jianghongdianzi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://po.szsharing.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ha.huixiangedu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://um.newstarts.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zc.shxzukj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hi.bjjhwx.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cg.hahajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ac.szsharing.cn

[K07] 进制转换
来源：http://rb.jianghongdianzi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pz.huixiangedu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sp.nicolike.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://se.panjiajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://by.jctech888.com.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uv.shxzukj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xj.haigaiapp.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cu.yuexingan06.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://oj.nszjky.cn

[K08] 二进制序列化（非 JSON）
来源：http://eb.szsharing.cn

Py:   pickle.dumps(obj)
来源：http://ci.panjiajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dc.shxzukj.cn

JS:   v8.serialize(obj)        // Node
来源：http://kv.huixinmuqiang.cn

TS:   v8.serialize(obj)        // Node
来源：http://bw.hnjuh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ie.nicolike.cn

Go:   encoding/gob
来源：http://gw.muxihuayi.cn

Ruby: Marshal.dump(obj)
来源：http://ek.szxytkj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xn.szsharing.cn

================================================================================
来源：http://tx.newstarts.cn

L. 网络请求
来源：http://wi.asd995.cn

================================================================================
来源：http://cz.chemitech.net.cn

[L01] 发送 GET 请求
来源：http://re.jianghongdianzi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gi.haigaiapp.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yt.yuexingan06.cn

JS:   await fetch(url)
来源：http://nm.nicolike.cn

TS:   await fetch(url)
来源：http://pn.shxzskj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://io.huixinmuqiang.cn

Go:   resp, err := http.Get(url)
来源：http://gt.9csxet.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bw.szxytkj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://he.bookmarksfly.cn

[L02] 发送 POST JSON
来源：http://oc.yuexingan06.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qk.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hr.nszjky.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bp.huixinmuqiang.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://db.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://th.nszjky.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ud.hnjuh.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uo.jctech888.com.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qc.hnjuh.cn

[L03] 设置自定义请求头
来源：http://vs.nszjky.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mn.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://oq.9csxet.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gj.yuntaijiaju.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vh.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vl.muxihuayi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://py.jctech888.com.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lg.jianghongdianzi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pl.jctech888.com.cn

[L04] 设置超时
来源：http://rc.yuntaijiaju.cn

Py:   requests.get(url, timeout=5)
来源：http://wb.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tl.yuntaijiaju.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ny.shxzukj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xa.jctech888.com.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://im.nicolike.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fe.gzmigu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cg.newstarts.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ny.haigaiapp.cn

[L05] 上传文件（multipart）
来源：http://st.gzmigu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zs.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jm.shxzukj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mi.nicolike.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pj.jianghongdianzi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vr.szxytkj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ys.bookmarksfly.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://py.yuexingan06.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ba.panjiajie.cn

[L06] 解析响应为 JSON
来源：http://fd.yuexingan06.cn

Py:   resp.json()
来源：http://xf.9csxet.cn

PHP:  json_decode($body, true);
来源：http://es.bookmarksfly.cn

JS:   await resp.json()
来源：http://wi.muxihuayi.cn

TS:   await resp.json()
来源：http://bc.szxytkj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yw.521024.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bj.huanxung.cn

Ruby: JSON.parse(resp.body)
来源：http://ue.asd995.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sd.panjiajie.cn

[L07] 处理 HTTP 状态码
来源：http://hr.chemitech.net.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://je.chemitech.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mz.asd995.cn

JS:   resp.ok;  resp.status
来源：http://ow.hnjuh.cn

TS:   resp.ok;  resp.status
来源：http://lj.szxytkj.cn

Java: resp.statusCode()
来源：http://ay.bjjhwx.cn

Go:   resp.StatusCode
来源：http://lf.shxzukj.cn

Ruby: resp.code.to_i
来源：http://kb.bookmarksfly.cn

C#:   (int)resp.StatusCode
来源：http://tj.gzmigu.cn

[L08] 并发请求多个地址
来源：http://ud.nszjky.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bz.shxzskj.cn

PHP:  curl_multi_init() 系列
来源：http://bq.gzmigu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://su.shxzskj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xt.yuexingan06.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uz.panjiajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qg.huanxung.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qq.bookmarksfly.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://af.newstarts.cn

================================================================================
来源：http://ht.bjjhwx.cn

M. 命令行 / 进程 / 环境
来源：http://we.jctech888.com.cn

================================================================================
来源：http://oa.521024.cn

[M01] 读取命令行参数
来源：http://ea.asd995.cn

Py:   sys.argv[1:]
来源：http://qr.colortex.cn

PHP:  $argv;  $argc;
来源：http://uu.yuntaijiaju.cn

JS:   process.argv.slice(2)
来源：http://ry.huanxung.cn

TS:   process.argv.slice(2)
来源：http://bh.szsharing.cn

Java: args 数组（main 方法参数）
来源：http://mk.jctech888.com.cn

Go:   os.Args[1:]
来源：http://tk.hahajie.cn

Ruby: ARGV
来源：http://gj.szsharing.cn

C#:   args 数组（Main 方法参数）
来源：http://lr.huixiangedu.cn

[M02] 读取环境变量
来源：http://wi.yuexingan06.cn

Py:   os.environ.get("HOME")
来源：http://ca.bjjhwx.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vm.shxzukj.cn

JS:   process.env.HOME
来源：http://dl.asd995.cn

TS:   process.env.HOME
来源：http://jn.newstarts.cn

Java: System.getenv("HOME")
来源：http://gm.9csxet.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dq.jianghongdianzi.cn

Ruby: ENV["HOME"]
来源：http://na.wgjwhj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jm.521024.cn

[M03] 执行外部命令
来源：http://um.asd995.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fj.chemitech.net.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wo.yuexingan06.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://fq.shtwfgs.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fh.hnjuh.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dl.bjjhwx.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xz.huixinmuqiang.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xi.haigaiapp.cn

C#:   Process.Start("ls", "-l");
来源：http://ey.panjiajie.cn

[M04] 获取当前工作目录
来源：http://fw.jctech888.com.cn

Py:   os.getcwd()
来源：http://uk.bjjhwx.cn

PHP:  getcwd();
来源：http://wb.bjjhwx.cn

JS:   process.cwd()
来源：http://hv.panjiajie.cn

TS:   process.cwd()
来源：http://rw.huixinmuqiang.cn

Java: Path.of("").toAbsolutePath()
来源：http://bg.huixiangedu.cn

Go:   os.Getwd()
来源：http://kb.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://yk.9csxet.cn

C#:   Directory.GetCurrentDirectory()
来源：http://kz.lnxyls.cn

[M05] 设置退出码
来源：http://kn.muxihuayi.cn

Py:   sys.exit(1)
来源：http://nc.9csxet.cn

PHP:  exit(1);
来源：http://zt.muxihuayi.cn


<!-- 参考信息 -->