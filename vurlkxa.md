代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ju.huixiangedu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sq.nicolike.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lv.panjiajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xm.hahajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://av.hnjuh.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vh.hahajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nk.jctech888.com.cn

================================================================================
来源：http://ha.shxzskj.cn

J. 日期与时间
来源：http://hv.chemitech.net.cn

================================================================================
来源：http://ww.huanxung.cn

[J01] 获取当前时间
来源：http://ly.newstarts.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ed.colortex.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rh.newstarts.cn

JS:   new Date();  Date.now()
来源：http://qw.hnjuh.cn

TS:   new Date();  Date.now()
来源：http://vq.huixinmuqiang.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://sv.521024.cn

Go:   time.Now()
来源：http://kb.gzmigu.cn

Ruby: Time.now
来源：http://js.panjiajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wf.huixiangedu.cn

[J02] 格式化输出
来源：http://ed.szsharing.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ft.wgjwhj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bu.jctech888.com.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tb.colortex.cn

TS:   d.toISOString()
来源：http://qn.huixinmuqiang.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pt.shxzukj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ls.chemitech.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://np.muxihuayi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://am.huanxung.cn

[J03] 字符串解析为日期
来源：http://fa.bjjhwx.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://eb.colortex.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vj.shxzskj.cn

JS:   new Date("2024-01-02")
来源：http://dx.wgjwhj.cn

TS:   new Date("2024-01-02")
来源：http://zu.panjiajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rt.huixiangedu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wr.hnjuh.cn

Ruby: Date.parse("2024-01-02")
来源：http://qx.bookmarksfly.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cb.chemitech.net.cn

[J04] 时间戳与日期互转
来源：http://wj.haigaiapp.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rb.bookmarksfly.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qb.9csxet.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ov.colortex.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qw.huixinmuqiang.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xw.yuexingan06.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ht.szxytkj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yc.jctech888.com.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wx.521024.cn

[J05] 时间加减（加 7 天）
来源：http://ay.huanxung.cn

Py:   now + timedelta(days=7)
来源：http://te.gzmigu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jt.asd995.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tq.jctech888.com.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gw.shxzskj.cn

Java: LocalDate.now().plusDays(7)
来源：http://rl.szxytkj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xr.muxihuayi.cn

Ruby: Time.now + 7 * 86400
来源：http://jf.jianghongdianzi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://sy.bookmarksfly.cn

[J06] 计算两时间之差
来源：http://yt.bookmarksfly.cn

Py:   (end - start).total_seconds()
来源：http://nh.nicolike.cn

PHP:  $end->diff($start)->days;
来源：http://lx.gzmigu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://iv.hahajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tj.haigaiapp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://oj.nicolike.cn

Go:   end.Sub(start).Hours()
来源：http://ys.haigaiapp.cn

Ruby: end - start                 # 返回秒数
来源：http://rm.lnxyls.cn

C#:   (end - start).TotalSeconds
来源：http://bo.shtwfgs.cn

[J07] 比较两个日期
来源：http://se.jianghongdianzi.cn

Py:   d1 < d2;  d1 == d2
来源：http://uu.lnxyls.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bk.bjjhwx.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qx.hnjuh.cn

TS:   d1.getTime() < d2.getTime()
来源：http://wy.panjiajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vg.huixinmuqiang.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ev.haigaiapp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qo.colortex.cn

C#:   d1 < d2;  d1 == d2
来源：http://ea.muxihuayi.cn

[J08] 提取年月日与星期
来源：http://ol.hahajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yi.asd995.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://he.colortex.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://co.521024.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wi.hahajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sm.asd995.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nv.9csxet.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ih.shxzukj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qw.szxytkj.cn

[J09] 时区处理
来源：http://qv.shxzskj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sg.hahajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ug.shtwfgs.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vv.haigaiapp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xx.szsharing.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://iw.nicolike.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rl.hahajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ux.panjiajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vh.newstarts.cn

[J10] 取今天 / 本月第一天
来源：http://yc.nszjky.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jv.nicolike.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cf.hnjuh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ia.huixiangedu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://li.hnjuh.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vz.shxzskj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yw.colortex.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ky.huanxung.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ha.newstarts.cn

================================================================================
来源：http://ho.jianghongdianzi.cn

K. JSON 与序列化
来源：http://rj.wgjwhj.cn

================================================================================
来源：http://kq.shtwfgs.cn

[K01] 对象转 JSON 字符串
来源：http://xy.nszjky.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vq.shtwfgs.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://np.nicolike.cn

JS:   JSON.stringify(obj)
来源：http://jb.szxytkj.cn

TS:   JSON.stringify(obj)
来源：http://ai.hahajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jf.colortex.cn

Go:   json.Marshal(obj)
来源：http://eb.szsharing.cn

Ruby: obj.to_json                                     // require "json"
来源：http://lb.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ll.huanxung.cn

[K02] JSON 字符串转对象
来源：http://ui.yuexingan06.cn

Py:   json.loads(s)
来源：http://yk.shxzukj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ol.shtwfgs.cn

JS:   JSON.parse(s)
来源：http://eh.huixinmuqiang.cn

TS:   JSON.parse(s)
来源：http://ag.huixiangedu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bv.huanxung.cn

Go:   json.Unmarshal(data, &v)
来源：http://te.huixiangedu.cn

Ruby: JSON.parse(s)
来源：http://og.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nt.szsharing.cn

[K03] JSON 美化输出（带缩进）
来源：http://ps.hnjuh.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cx.bjjhwx.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://oo.9csxet.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kf.asd995.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://pc.szxytkj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rq.gzmigu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ax.bjjhwx.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nb.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gr.nszjky.cn

[K04] 读取 JSON 文件
来源：http://sq.9csxet.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mf.nszjky.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iu.bookmarksfly.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dp.wgjwhj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ux.colortex.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kd.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fs.shxzskj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rf.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tk.huixinmuqiang.cn

[K05] 深拷贝对象
来源：http://pv.newstarts.cn

Py:   copy.deepcopy(obj)
来源：http://kx.nicolike.cn

PHP:  unserialize(serialize($obj));
来源：http://wi.jctech888.com.cn

JS:   structuredClone(obj)
来源：http://bh.bjjhwx.cn

TS:   structuredClone(obj)
来源：http://jl.lnxyls.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://pf.nszjky.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zt.gzmigu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ee.muxihuayi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tg.chemitech.net.cn

[K06] 解析 URL 查询串
来源：http://dq.shtwfgs.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gn.huixinmuqiang.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zo.shxzukj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eh.gzmigu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zm.shxzukj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bo.bjjhwx.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dy.panjiajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xx.yuexingan06.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kr.521024.cn

[K07] 进制转换
来源：http://ua.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zw.jianghongdianzi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vo.panjiajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jl.newstarts.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jl.huixinmuqiang.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qv.chemitech.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yr.huixinmuqiang.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sz.jianghongdianzi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xf.shxzskj.cn

[K08] 二进制序列化（非 JSON）
来源：http://lw.bookmarksfly.cn

Py:   pickle.dumps(obj)
来源：http://zj.hnjuh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lt.bookmarksfly.cn

JS:   v8.serialize(obj)        // Node
来源：http://xu.jctech888.com.cn

TS:   v8.serialize(obj)        // Node
来源：http://ev.chemitech.net.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xz.szsharing.cn

Go:   encoding/gob
来源：http://to.colortex.cn

Ruby: Marshal.dump(obj)
来源：http://df.nicolike.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jq.huixinmuqiang.cn

================================================================================
来源：http://ph.521024.cn

L. 网络请求
来源：http://gw.panjiajie.cn

================================================================================
来源：http://vd.nicolike.cn

[L01] 发送 GET 请求
来源：http://yq.9csxet.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ry.lnxyls.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bh.szsharing.cn

JS:   await fetch(url)
来源：http://dt.szsharing.cn

TS:   await fetch(url)
来源：http://xf.bookmarksfly.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://eb.hnjuh.cn

Go:   resp, err := http.Get(url)
来源：http://av.colortex.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ao.nicolike.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://py.gzmigu.cn

[L02] 发送 POST JSON
来源：http://gd.panjiajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://us.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bn.chemitech.net.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://be.newstarts.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eu.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gj.huixiangedu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://er.jianghongdianzi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hb.asd995.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://us.bookmarksfly.cn

[L03] 设置自定义请求头
来源：http://ha.chemitech.net.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://af.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ky.hnjuh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ch.shxzskj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hd.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rs.jctech888.com.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ac.shtwfgs.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fd.szsharing.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ml.jianghongdianzi.cn

[L04] 设置超时
来源：http://of.panjiajie.cn

Py:   requests.get(url, timeout=5)
来源：http://ca.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://db.lnxyls.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dh.bookmarksfly.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ts.szsharing.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uh.nicolike.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mg.chemitech.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ek.jianghongdianzi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ku.muxihuayi.cn

[L05] 上传文件（multipart）
来源：http://rf.nicolike.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hb.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hy.panjiajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pi.jianghongdianzi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rp.shtwfgs.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tt.lnxyls.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ws.haigaiapp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dv.bookmarksfly.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vv.bookmarksfly.cn

[L06] 解析响应为 JSON
来源：http://qr.9csxet.cn

Py:   resp.json()
来源：http://qb.gzmigu.cn

PHP:  json_decode($body, true);
来源：http://vj.asd995.cn

JS:   await resp.json()
来源：http://sm.bjjhwx.cn

TS:   await resp.json()
来源：http://uq.9csxet.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yp.bjjhwx.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hr.hnjuh.cn

Ruby: JSON.parse(resp.body)
来源：http://ar.shtwfgs.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lj.panjiajie.cn

[L07] 处理 HTTP 状态码
来源：http://xm.shxzukj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ow.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hl.hnjuh.cn

JS:   resp.ok;  resp.status
来源：http://pg.huixiangedu.cn

TS:   resp.ok;  resp.status
来源：http://fn.shxzukj.cn

Java: resp.statusCode()
来源：http://cl.huixiangedu.cn

Go:   resp.StatusCode
来源：http://gd.wgjwhj.cn

Ruby: resp.code.to_i
来源：http://nq.shxzukj.cn

C#:   (int)resp.StatusCode
来源：http://qh.nicolike.cn

[L08] 并发请求多个地址
来源：http://qr.szsharing.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hk.muxihuayi.cn

PHP:  curl_multi_init() 系列
来源：http://ti.wgjwhj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vc.chemitech.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fh.9csxet.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jz.hnjuh.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tc.bjjhwx.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ct.yuntaijiaju.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://oa.huixiangedu.cn

================================================================================
来源：http://kf.newstarts.cn

M. 命令行 / 进程 / 环境
来源：http://cb.newstarts.cn

================================================================================
来源：http://vt.jianghongdianzi.cn

[M01] 读取命令行参数
来源：http://yr.hahajie.cn

Py:   sys.argv[1:]
来源：http://ry.huixinmuqiang.cn

PHP:  $argv;  $argc;
来源：http://op.lnxyls.cn

JS:   process.argv.slice(2)
来源：http://pe.yuntaijiaju.cn

TS:   process.argv.slice(2)
来源：http://ax.chemitech.net.cn

Java: args 数组（main 方法参数）
来源：http://bu.bookmarksfly.cn

Go:   os.Args[1:]
来源：http://ze.muxihuayi.cn

Ruby: ARGV
来源：http://rz.gzmigu.cn

C#:   args 数组（Main 方法参数）
来源：http://xo.huixinmuqiang.cn

[M02] 读取环境变量
来源：http://hk.bookmarksfly.cn

Py:   os.environ.get("HOME")
来源：http://yq.huixinmuqiang.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bg.bjjhwx.cn

JS:   process.env.HOME
来源：http://ts.wgjwhj.cn

TS:   process.env.HOME
来源：http://dk.hahajie.cn

Java: System.getenv("HOME")
来源：http://qr.521024.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qh.huixinmuqiang.cn

Ruby: ENV["HOME"]
来源：http://sj.nszjky.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ib.panjiajie.cn

[M03] 执行外部命令
来源：http://jm.shxzukj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vs.asd995.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ng.panjiajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://na.yuexingan06.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nr.hahajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jp.bjjhwx.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ml.colortex.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tb.bjjhwx.cn

C#:   Process.Start("ls", "-l");
来源：http://td.szxytkj.cn

[M04] 获取当前工作目录
来源：http://yp.lnxyls.cn

Py:   os.getcwd()
来源：http://dd.hnjuh.cn

PHP:  getcwd();
来源：http://sg.nicolike.cn

JS:   process.cwd()
来源：http://tt.huixinmuqiang.cn

TS:   process.cwd()
来源：http://bv.wgjwhj.cn

Java: Path.of("").toAbsolutePath()
来源：http://mw.jianghongdianzi.cn

Go:   os.Getwd()
来源：http://fc.bookmarksfly.cn

Ruby: Dir.pwd
来源：http://ws.9csxet.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qa.panjiajie.cn

[M05] 设置退出码
来源：http://rj.panjiajie.cn

Py:   sys.exit(1)
来源：http://xq.521024.cn

PHP:  exit(1);
来源：http://ym.gzmigu.cn

JS:   process.exit(1)
来源：http://ly.bjjhwx.cn

TS:   process.exit(1)
来源：http://xu.asd995.cn

Java: System.exit(1)
来源：http://ti.nicolike.cn

Go:   os.Exit(1)
来源：http://nd.jctech888.com.cn

Ruby: exit 1
来源：http://hm.shtwfgs.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bm.bookmarksfly.cn

[M06] 向标准错误输出
来源：http://pz.szxytkj.cn

Py:   print("err", file=sys.stderr)
来源：http://nu.shxzukj.cn


<!-- 参考信息 -->