代发 wailian999

Ruby: s.scan(/error/i)
来源：http://wp.yuexingan06.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ev.huixinmuqiang.cn

[I08] 贪婪与非贪婪匹配
来源：http://gh.521024.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pf.newstarts.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ui.jianghongdianzi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vw.shtwfgs.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://aq.bookmarksfly.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://up.yuntaijiaju.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gz.jctech888.com.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ro.hnjuh.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fh.bookmarksfly.cn

================================================================================
来源：http://rg.9csxet.cn

J. 日期与时间
来源：http://qj.szxytkj.cn

================================================================================
来源：http://ch.hnjuh.cn

[J01] 获取当前时间
来源：http://ki.yuntaijiaju.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lp.newstarts.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://og.wgjwhj.cn

JS:   new Date();  Date.now()
来源：http://nh.shtwfgs.cn

TS:   new Date();  Date.now()
来源：http://pk.bookmarksfly.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hb.bjjhwx.cn

Go:   time.Now()
来源：http://ou.521024.cn

Ruby: Time.now
来源：http://bp.huixiangedu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cz.nicolike.cn

[J02] 格式化输出
来源：http://qm.yuntaijiaju.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gm.szxytkj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://oi.nszjky.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://am.hahajie.cn

TS:   d.toISOString()
来源：http://gw.jctech888.com.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ty.chemitech.net.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mu.shxzskj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ec.colortex.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nm.9csxet.cn

[J03] 字符串解析为日期
来源：http://oa.wgjwhj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ct.szsharing.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qa.hnjuh.cn

JS:   new Date("2024-01-02")
来源：http://xu.nicolike.cn

TS:   new Date("2024-01-02")
来源：http://pg.szsharing.cn

Java: LocalDate.parse("2024-01-02")
来源：http://lf.panjiajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mr.szsharing.cn

Ruby: Date.parse("2024-01-02")
来源：http://wj.hnjuh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zb.shtwfgs.cn

[J04] 时间戳与日期互转
来源：http://ac.hnjuh.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hj.521024.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sk.jctech888.com.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ct.hnjuh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zb.nicolike.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://we.chemitech.net.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gx.haigaiapp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vq.wgjwhj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ae.hahajie.cn

[J05] 时间加减（加 7 天）
来源：http://hu.muxihuayi.cn

Py:   now + timedelta(days=7)
来源：http://op.huanxung.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lm.hahajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lm.colortex.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uk.bookmarksfly.cn

Java: LocalDate.now().plusDays(7)
来源：http://ny.colortex.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yz.bjjhwx.cn

Ruby: Time.now + 7 * 86400
来源：http://lf.yuexingan06.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pa.colortex.cn

[J06] 计算两时间之差
来源：http://gp.lnxyls.cn

Py:   (end - start).total_seconds()
来源：http://la.lnxyls.cn

PHP:  $end->diff($start)->days;
来源：http://au.wgjwhj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zq.newstarts.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rh.jctech888.com.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mi.huixinmuqiang.cn

Go:   end.Sub(start).Hours()
来源：http://sj.521024.cn

Ruby: end - start                 # 返回秒数
来源：http://gh.hnjuh.cn

C#:   (end - start).TotalSeconds
来源：http://dr.521024.cn

[J07] 比较两个日期
来源：http://sf.nszjky.cn

Py:   d1 < d2;  d1 == d2
来源：http://fq.nszjky.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mi.nicolike.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qh.szxytkj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rm.chemitech.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vc.521024.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nz.newstarts.cn

Ruby: d1 < d2;  d1 == d2
来源：http://rt.muxihuayi.cn

C#:   d1 < d2;  d1 == d2
来源：http://az.newstarts.cn

[J08] 提取年月日与星期
来源：http://pm.shxzskj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hr.szxytkj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ig.nszjky.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zs.newstarts.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kb.9csxet.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://le.asd995.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://to.jianghongdianzi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gf.newstarts.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ml.shtwfgs.cn

[J09] 时区处理
来源：http://wz.chemitech.net.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nb.colortex.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://za.wgjwhj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fc.haigaiapp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qu.yuntaijiaju.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dj.asd995.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gk.huixiangedu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://rc.hnjuh.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bv.szxytkj.cn

[J10] 取今天 / 本月第一天
来源：http://zd.haigaiapp.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cw.huixiangedu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bb.asd995.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yr.gzmigu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nc.bookmarksfly.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yu.haigaiapp.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ky.newstarts.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ly.szsharing.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jv.521024.cn

================================================================================
来源：http://bc.gzmigu.cn

K. JSON 与序列化
来源：http://xq.asd995.cn

================================================================================
来源：http://uu.shtwfgs.cn

[K01] 对象转 JSON 字符串
来源：http://yo.shtwfgs.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qg.wgjwhj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://td.newstarts.cn

JS:   JSON.stringify(obj)
来源：http://ph.newstarts.cn

TS:   JSON.stringify(obj)
来源：http://ag.jianghongdianzi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sj.jianghongdianzi.cn

Go:   json.Marshal(obj)
来源：http://vb.521024.cn

Ruby: obj.to_json                                     // require "json"
来源：http://or.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zs.hahajie.cn

[K02] JSON 字符串转对象
来源：http://ro.szxytkj.cn

Py:   json.loads(s)
来源：http://iy.nicolike.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://in.gzmigu.cn

JS:   JSON.parse(s)
来源：http://wn.bookmarksfly.cn

TS:   JSON.parse(s)
来源：http://jc.nicolike.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://me.muxihuayi.cn

Go:   json.Unmarshal(data, &v)
来源：http://uu.lnxyls.cn

Ruby: JSON.parse(s)
来源：http://td.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ux.newstarts.cn

[K03] JSON 美化输出（带缩进）
来源：http://xy.haigaiapp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vm.szsharing.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ps.bjjhwx.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nd.gzmigu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://jy.shxzskj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wc.szsharing.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://aa.yuexingan06.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hr.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ly.521024.cn

[K04] 读取 JSON 文件
来源：http://iw.jctech888.com.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xd.colortex.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ww.lnxyls.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://on.yuntaijiaju.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iq.521024.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xe.gzmigu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://iv.bjjhwx.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://md.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ho.szsharing.cn

[K05] 深拷贝对象
来源：http://jz.nszjky.cn

Py:   copy.deepcopy(obj)
来源：http://dc.huanxung.cn

PHP:  unserialize(serialize($obj));
来源：http://mx.asd995.cn

JS:   structuredClone(obj)
来源：http://dy.szsharing.cn

TS:   structuredClone(obj)
来源：http://np.hnjuh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zy.haigaiapp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pc.szsharing.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hi.521024.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pc.bjjhwx.cn

[K06] 解析 URL 查询串
来源：http://kt.huixiangedu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zc.panjiajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tj.521024.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zw.jctech888.com.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://re.hnjuh.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rx.gzmigu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mz.huanxung.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ak.jianghongdianzi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gr.chemitech.net.cn

[K07] 进制转换
来源：http://dx.hahajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tf.shtwfgs.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yp.chemitech.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zl.asd995.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lj.newstarts.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ro.bjjhwx.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ys.shtwfgs.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wj.bookmarksfly.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kh.yuntaijiaju.cn

[K08] 二进制序列化（非 JSON）
来源：http://zu.szxytkj.cn

Py:   pickle.dumps(obj)
来源：http://zp.bjjhwx.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ek.nszjky.cn

JS:   v8.serialize(obj)        // Node
来源：http://ms.bookmarksfly.cn

TS:   v8.serialize(obj)        // Node
来源：http://ve.gzmigu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ce.szxytkj.cn

Go:   encoding/gob
来源：http://uu.shtwfgs.cn

Ruby: Marshal.dump(obj)
来源：http://xp.yuntaijiaju.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ad.shtwfgs.cn

================================================================================
来源：http://uy.bjjhwx.cn

L. 网络请求
来源：http://st.bjjhwx.cn

================================================================================
来源：http://th.haigaiapp.cn

[L01] 发送 GET 请求
来源：http://fw.panjiajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sy.hahajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fv.bjjhwx.cn

JS:   await fetch(url)
来源：http://wg.shxzskj.cn

TS:   await fetch(url)
来源：http://ke.chemitech.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://do.huixinmuqiang.cn

Go:   resp, err := http.Get(url)
来源：http://mj.huixinmuqiang.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hr.jctech888.com.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mw.huixiangedu.cn

[L02] 发送 POST JSON
来源：http://cu.haigaiapp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://kk.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ps.lnxyls.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ja.wgjwhj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://da.colortex.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sq.hahajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://in.bjjhwx.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pb.521024.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zs.panjiajie.cn

[L03] 设置自定义请求头
来源：http://ov.huixinmuqiang.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://iu.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gc.colortex.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ia.shxzskj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kq.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mr.shxzskj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rw.jianghongdianzi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cc.huixiangedu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fu.asd995.cn

[L04] 设置超时
来源：http://ph.jianghongdianzi.cn

Py:   requests.get(url, timeout=5)
来源：http://it.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mo.yuntaijiaju.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wc.jctech888.com.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ww.muxihuayi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hp.521024.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yc.haigaiapp.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jctech888.com.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://or.bookmarksfly.cn

[L05] 上传文件（multipart）
来源：http://pq.shtwfgs.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cf.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gd.jctech888.com.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://st.haigaiapp.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vi.jctech888.com.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://of.bjjhwx.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cn.szsharing.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://te.szxytkj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yv.yuntaijiaju.cn

[L06] 解析响应为 JSON
来源：http://pz.colortex.cn

Py:   resp.json()
来源：http://jb.szxytkj.cn

PHP:  json_decode($body, true);
来源：http://zk.lnxyls.cn

JS:   await resp.json()
来源：http://ri.9csxet.cn

TS:   await resp.json()
来源：http://sg.shtwfgs.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xs.lnxyls.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hm.shxzskj.cn

Ruby: JSON.parse(resp.body)
来源：http://sp.yuntaijiaju.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qw.newstarts.cn

[L07] 处理 HTTP 状态码
来源：http://do.hnjuh.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bl.huixinmuqiang.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sd.szxytkj.cn

JS:   resp.ok;  resp.status
来源：http://gd.huanxung.cn

TS:   resp.ok;  resp.status
来源：http://zo.chemitech.net.cn

Java: resp.statusCode()
来源：http://iy.nszjky.cn

Go:   resp.StatusCode
来源：http://fl.newstarts.cn

Ruby: resp.code.to_i
来源：http://cd.bjjhwx.cn

C#:   (int)resp.StatusCode
来源：http://io.gzmigu.cn

[L08] 并发请求多个地址
来源：http://sn.9csxet.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pd.nszjky.cn

PHP:  curl_multi_init() 系列
来源：http://vj.jctech888.com.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iw.panjiajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dg.huixinmuqiang.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pu.wgjwhj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ph.yuntaijiaju.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bs.colortex.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zc.wgjwhj.cn

================================================================================
来源：http://pz.yuexingan06.cn

M. 命令行 / 进程 / 环境
来源：http://yl.muxihuayi.cn

================================================================================
来源：http://ix.huixiangedu.cn

[M01] 读取命令行参数
来源：http://ov.szxytkj.cn

Py:   sys.argv[1:]
来源：http://no.bjjhwx.cn

PHP:  $argv;  $argc;
来源：http://ey.9csxet.cn

JS:   process.argv.slice(2)
来源：http://ij.gzmigu.cn

TS:   process.argv.slice(2)
来源：http://ta.yuexingan06.cn

Java: args 数组（main 方法参数）
来源：http://xg.shxzukj.cn

Go:   os.Args[1:]
来源：http://di.panjiajie.cn

Ruby: ARGV
来源：http://fm.colortex.cn

C#:   args 数组（Main 方法参数）
来源：http://wu.hnjuh.cn

[M02] 读取环境变量
来源：http://wn.haigaiapp.cn

Py:   os.environ.get("HOME")
来源：http://tg.hahajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nd.muxihuayi.cn

JS:   process.env.HOME
来源：http://wf.shxzskj.cn

TS:   process.env.HOME
来源：http://xk.asd995.cn

Java: System.getenv("HOME")
来源：http://el.hahajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://id.jctech888.com.cn

Ruby: ENV["HOME"]
来源：http://yp.colortex.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xy.huanxung.cn

[M03] 执行外部命令
来源：http://hg.colortex.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jj.jianghongdianzi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wt.panjiajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://cc.wgjwhj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xr.shxzukj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gq.yuntaijiaju.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://rh.asd995.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yv.lnxyls.cn

C#:   Process.Start("ls", "-l");
来源：http://me.szsharing.cn

[M04] 获取当前工作目录
来源：http://lg.hahajie.cn

Py:   os.getcwd()
来源：http://if.shtwfgs.cn

PHP:  getcwd();
来源：http://uo.yuexingan06.cn

JS:   process.cwd()
来源：http://kz.hnjuh.cn

TS:   process.cwd()
来源：http://rd.shtwfgs.cn

Java: Path.of("").toAbsolutePath()
来源：http://fm.muxihuayi.cn

Go:   os.Getwd()
来源：http://tl.muxihuayi.cn

Ruby: Dir.pwd
来源：http://ph.muxihuayi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://wp.521024.cn

[M05] 设置退出码
来源：http://gz.asd995.cn

Py:   sys.exit(1)
来源：http://lj.lnxyls.cn

PHP:  exit(1);
来源：http://oj.shtwfgs.cn

JS:   process.exit(1)
来源：http://vo.szsharing.cn

TS:   process.exit(1)
来源：http://ue.jctech888.com.cn

Java: System.exit(1)
来源：http://ti.bjjhwx.cn

Go:   os.Exit(1)
来源：http://jj.szsharing.cn


<!-- 参考信息 -->