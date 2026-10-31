代发 wailian999

Ruby: s.scan(/error/i)
来源：http://ha.jctech888.com.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mk.colortex.cn

[I08] 贪婪与非贪婪匹配
来源：http://dk.panjiajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ct.newstarts.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gt.szsharing.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ih.shtwfgs.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pv.panjiajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://kk.shtwfgs.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lo.shtwfgs.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mc.huixinmuqiang.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bm.9csxet.cn

================================================================================
来源：http://og.jianghongdianzi.cn

J. 日期与时间
来源：http://ab.bookmarksfly.cn

================================================================================
来源：http://ul.jianghongdianzi.cn

[J01] 获取当前时间
来源：http://qz.panjiajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://di.huixinmuqiang.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tf.szsharing.cn

JS:   new Date();  Date.now()
来源：http://ez.gzmigu.cn

TS:   new Date();  Date.now()
来源：http://kl.bookmarksfly.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://nt.szsharing.cn

Go:   time.Now()
来源：http://cr.jianghongdianzi.cn

Ruby: Time.now
来源：http://ww.haigaiapp.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nf.jctech888.com.cn

[J02] 格式化输出
来源：http://ja.muxihuayi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zl.huixiangedu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://st.szxytkj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zx.nicolike.cn

TS:   d.toISOString()
来源：http://pk.bookmarksfly.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xi.521024.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yd.jianghongdianzi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zk.huanxung.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pw.szsharing.cn

[J03] 字符串解析为日期
来源：http://sw.521024.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ss.colortex.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gq.yuexingan06.cn

JS:   new Date("2024-01-02")
来源：http://vy.newstarts.cn

TS:   new Date("2024-01-02")
来源：http://yz.szxytkj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hu.yuntaijiaju.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tu.nicolike.cn

Ruby: Date.parse("2024-01-02")
来源：http://ho.bjjhwx.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yo.hnjuh.cn

[J04] 时间戳与日期互转
来源：http://ac.colortex.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jv.huanxung.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://as.huanxung.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tx.jianghongdianzi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://us.haigaiapp.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nv.nszjky.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fq.muxihuayi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qq.huixinmuqiang.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ce.newstarts.cn

[J05] 时间加减（加 7 天）
来源：http://os.hahajie.cn

Py:   now + timedelta(days=7)
来源：http://oi.szxytkj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://fa.yuntaijiaju.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ci.asd995.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mn.bjjhwx.cn

Java: LocalDate.now().plusDays(7)
来源：http://iz.panjiajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ar.hnjuh.cn

Ruby: Time.now + 7 * 86400
来源：http://oh.nszjky.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ps.panjiajie.cn

[J06] 计算两时间之差
来源：http://te.bookmarksfly.cn

Py:   (end - start).total_seconds()
来源：http://bp.colortex.cn

PHP:  $end->diff($start)->days;
来源：http://ha.yuntaijiaju.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gi.hahajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ga.huixiangedu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bc.chemitech.net.cn

Go:   end.Sub(start).Hours()
来源：http://th.huanxung.cn

Ruby: end - start                 # 返回秒数
来源：http://jg.haigaiapp.cn

C#:   (end - start).TotalSeconds
来源：http://he.nszjky.cn

[J07] 比较两个日期
来源：http://nv.chemitech.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://pz.szxytkj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ke.shxzskj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ni.muxihuayi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ap.yuntaijiaju.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nr.huixinmuqiang.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pv.colortex.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ck.gzmigu.cn

C#:   d1 < d2;  d1 == d2
来源：http://jn.huixiangedu.cn

[J08] 提取年月日与星期
来源：http://cl.muxihuayi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cg.shxzukj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lc.colortex.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wk.lnxyls.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://za.szxytkj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ja.huanxung.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lk.szxytkj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ue.haigaiapp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cs.yuexingan06.cn

[J09] 时区处理
来源：http://cj.lnxyls.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dd.9csxet.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sy.huanxung.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sv.szxytkj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cp.wgjwhj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ch.bjjhwx.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mm.521024.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ha.jctech888.com.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fo.bjjhwx.cn

[J10] 取今天 / 本月第一天
来源：http://cy.szsharing.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jx.yuexingan06.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ok.shxzukj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://do.lnxyls.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jd.shxzskj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://iy.huanxung.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kr.shxzskj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tl.nicolike.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qt.huixiangedu.cn

================================================================================
来源：http://qn.haigaiapp.cn

K. JSON 与序列化
来源：http://oh.wgjwhj.cn

================================================================================
来源：http://tz.szsharing.cn

[K01] 对象转 JSON 字符串
来源：http://gy.shtwfgs.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hh.bookmarksfly.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ij.bjjhwx.cn

JS:   JSON.stringify(obj)
来源：http://ac.521024.cn

TS:   JSON.stringify(obj)
来源：http://rg.9csxet.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ij.huixiangedu.cn

Go:   json.Marshal(obj)
来源：http://eu.jctech888.com.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qh.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://cp.haigaiapp.cn

[K02] JSON 字符串转对象
来源：http://wh.asd995.cn

Py:   json.loads(s)
来源：http://tv.panjiajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dp.shxzukj.cn

JS:   JSON.parse(s)
来源：http://jc.panjiajie.cn

TS:   JSON.parse(s)
来源：http://zu.shtwfgs.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ab.huixinmuqiang.cn

Go:   json.Unmarshal(data, &v)
来源：http://aw.yuntaijiaju.cn

Ruby: JSON.parse(s)
来源：http://gb.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fp.nicolike.cn

[K03] JSON 美化输出（带缩进）
来源：http://ir.huixiangedu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lk.huixiangedu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rc.huixiangedu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://cr.shxzukj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://kl.asd995.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zt.shtwfgs.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cl.nszjky.cn

Ruby: JSON.pretty_generate(obj)
来源：http://im.gzmigu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lh.shxzukj.cn

[K04] 读取 JSON 文件
来源：http://ea.shxzukj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fk.hnjuh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fh.gzmigu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jianghongdianzi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pu.wgjwhj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ri.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sv.yuexingan06.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ee.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lg.asd995.cn

[K05] 深拷贝对象
来源：http://qz.haigaiapp.cn

Py:   copy.deepcopy(obj)
来源：http://np.nicolike.cn

PHP:  unserialize(serialize($obj));
来源：http://rm.gzmigu.cn

JS:   structuredClone(obj)
来源：http://pk.shxzskj.cn

TS:   structuredClone(obj)
来源：http://op.huixinmuqiang.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rd.shxzukj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ng.szxytkj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sq.wgjwhj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gp.haigaiapp.cn

[K06] 解析 URL 查询串
来源：http://bb.hahajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://px.newstarts.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://du.chemitech.net.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jq.jianghongdianzi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fu.huixinmuqiang.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ti.9csxet.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cx.colortex.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ij.nszjky.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lq.shxzskj.cn

[K07] 进制转换
来源：http://pc.chemitech.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ma.wgjwhj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cf.haigaiapp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pz.hnjuh.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sb.hnjuh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gj.shxzskj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jw.newstarts.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ez.huixinmuqiang.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nd.shxzukj.cn

[K08] 二进制序列化（非 JSON）
来源：http://su.jianghongdianzi.cn

Py:   pickle.dumps(obj)
来源：http://db.wgjwhj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pb.haigaiapp.cn

JS:   v8.serialize(obj)        // Node
来源：http://ua.hnjuh.cn

TS:   v8.serialize(obj)        // Node
来源：http://wg.haigaiapp.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ry.chemitech.net.cn

Go:   encoding/gob
来源：http://ic.haigaiapp.cn

Ruby: Marshal.dump(obj)
来源：http://dd.asd995.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uu.gzmigu.cn

================================================================================
来源：http://xh.panjiajie.cn

L. 网络请求
来源：http://mw.shxzukj.cn

================================================================================
来源：http://rv.shxzukj.cn

[L01] 发送 GET 请求
来源：http://ke.gzmigu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hn.jctech888.com.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dt.gzmigu.cn

JS:   await fetch(url)
来源：http://wb.521024.cn

TS:   await fetch(url)
来源：http://ua.shtwfgs.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ls.shxzskj.cn

Go:   resp, err := http.Get(url)
来源：http://ww.hahajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dn.huanxung.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jf.huixiangedu.cn

[L02] 发送 POST JSON
来源：http://dt.wgjwhj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bw.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://oh.muxihuayi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mg.shxzukj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zi.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nn.gzmigu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kn.yuntaijiaju.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ty.yuntaijiaju.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vv.shxzskj.cn

[L03] 设置自定义请求头
来源：http://xu.jianghongdianzi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qy.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ey.chemitech.net.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rw.hahajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lv.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hw.hahajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rr.lnxyls.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ey.newstarts.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vv.gzmigu.cn

[L04] 设置超时
来源：http://re.haigaiapp.cn

Py:   requests.get(url, timeout=5)
来源：http://sg.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ks.gzmigu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hx.hnjuh.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vu.chemitech.net.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xr.szxytkj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ma.bookmarksfly.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zb.nszjky.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ob.huixiangedu.cn

[L05] 上传文件（multipart）
来源：http://qo.521024.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xi.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vj.chemitech.net.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yn.nszjky.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fq.jctech888.com.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://aa.yuntaijiaju.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yo.jianghongdianzi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hg.nicolike.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ii.jctech888.com.cn

[L06] 解析响应为 JSON
来源：http://bk.huixinmuqiang.cn

Py:   resp.json()
来源：http://zz.521024.cn

PHP:  json_decode($body, true);
来源：http://bb.hnjuh.cn

JS:   await resp.json()
来源：http://rk.bjjhwx.cn

TS:   await resp.json()
来源：http://hh.huixinmuqiang.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jh.9csxet.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://sa.nszjky.cn

Ruby: JSON.parse(resp.body)
来源：http://sh.shxzukj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ax.asd995.cn

[L07] 处理 HTTP 状态码
来源：http://po.shtwfgs.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xe.huixiangedu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://os.newstarts.cn

JS:   resp.ok;  resp.status
来源：http://eg.huixiangedu.cn

TS:   resp.ok;  resp.status
来源：http://sy.bjjhwx.cn

Java: resp.statusCode()
来源：http://rj.hahajie.cn

Go:   resp.StatusCode
来源：http://su.wgjwhj.cn

Ruby: resp.code.to_i
来源：http://qe.gzmigu.cn

C#:   (int)resp.StatusCode
来源：http://ad.yuntaijiaju.cn

[L08] 并发请求多个地址
来源：http://ur.bookmarksfly.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xe.hahajie.cn

PHP:  curl_multi_init() 系列
来源：http://jg.521024.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eb.hnjuh.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eh.hnjuh.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cs.shtwfgs.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cm.hahajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sn.jianghongdianzi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xx.huixinmuqiang.cn

================================================================================
来源：http://ri.9csxet.cn

M. 命令行 / 进程 / 环境
来源：http://ob.szsharing.cn

================================================================================
来源：http://ys.huixinmuqiang.cn

[M01] 读取命令行参数
来源：http://ga.huixinmuqiang.cn

Py:   sys.argv[1:]
来源：http://iz.jctech888.com.cn

PHP:  $argv;  $argc;
来源：http://hc.szsharing.cn

JS:   process.argv.slice(2)
来源：http://su.yuntaijiaju.cn

TS:   process.argv.slice(2)
来源：http://pd.chemitech.net.cn

Java: args 数组（main 方法参数）
来源：http://yj.muxihuayi.cn

Go:   os.Args[1:]
来源：http://oc.nszjky.cn

Ruby: ARGV
来源：http://du.shtwfgs.cn

C#:   args 数组（Main 方法参数）
来源：http://iv.lnxyls.cn

[M02] 读取环境变量
来源：http://tu.gzmigu.cn

Py:   os.environ.get("HOME")
来源：http://tj.gzmigu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rj.huanxung.cn

JS:   process.env.HOME
来源：http://dr.hahajie.cn

TS:   process.env.HOME
来源：http://cd.hahajie.cn

Java: System.getenv("HOME")
来源：http://sb.nszjky.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ka.colortex.cn

Ruby: ENV["HOME"]
来源：http://ub.9csxet.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oj.muxihuayi.cn

[M03] 执行外部命令
来源：http://xg.gzmigu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://er.colortex.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mx.huixiangedu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ox.wgjwhj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pi.szxytkj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xn.wgjwhj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://eq.szsharing.cn

Ruby: system("ls -l");  `ls -l`
来源：http://lz.9csxet.cn

C#:   Process.Start("ls", "-l");
来源：http://tl.hnjuh.cn

[M04] 获取当前工作目录
来源：http://xq.colortex.cn

Py:   os.getcwd()
来源：http://yh.shxzukj.cn

PHP:  getcwd();
来源：http://sq.colortex.cn

JS:   process.cwd()
来源：http://oq.shxzskj.cn

TS:   process.cwd()
来源：http://qs.9csxet.cn

Java: Path.of("").toAbsolutePath()
来源：http://ue.hahajie.cn

Go:   os.Getwd()
来源：http://qq.bjjhwx.cn

Ruby: Dir.pwd
来源：http://yu.asd995.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gk.wgjwhj.cn

[M05] 设置退出码
来源：http://bm.newstarts.cn

Py:   sys.exit(1)
来源：http://yb.nicolike.cn

PHP:  exit(1);
来源：http://bg.hnjuh.cn

JS:   process.exit(1)
来源：http://mw.jianghongdianzi.cn

TS:   process.exit(1)
来源：http://ms.yuntaijiaju.cn

Java: System.exit(1)
来源：http://nh.huanxung.cn

Go:   os.Exit(1)
来源：http://ml.shxzukj.cn


<!-- 参考信息 -->