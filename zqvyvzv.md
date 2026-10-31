代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qc.colortex.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fx.chemitech.net.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hc.szxytkj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://db.lnxyls.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zh.asd995.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gq.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cn.hahajie.cn

================================================================================
来源：http://ev.huixiangedu.cn

J. 日期与时间
来源：http://bm.yuexingan06.cn

================================================================================
来源：http://xc.yuntaijiaju.cn

[J01] 获取当前时间
来源：http://cd.asd995.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://gg.hnjuh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://to.haigaiapp.cn

JS:   new Date();  Date.now()
来源：http://tx.hnjuh.cn

TS:   new Date();  Date.now()
来源：http://yj.szsharing.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ci.yuntaijiaju.cn

Go:   time.Now()
来源：http://ea.szxytkj.cn

Ruby: Time.now
来源：http://aa.huanxung.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fv.panjiajie.cn

[J02] 格式化输出
来源：http://bf.huixiangedu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rr.huixiangedu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ac.jctech888.com.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lz.huixiangedu.cn

TS:   d.toISOString()
来源：http://yn.newstarts.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xj.lnxyls.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nq.huanxung.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zt.nicolike.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uj.lnxyls.cn

[J03] 字符串解析为日期
来源：http://ab.newstarts.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://iv.jctech888.com.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qw.nicolike.cn

JS:   new Date("2024-01-02")
来源：http://rm.szsharing.cn

TS:   new Date("2024-01-02")
来源：http://dr.huixiangedu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://tj.9csxet.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wd.shxzskj.cn

Ruby: Date.parse("2024-01-02")
来源：http://yc.lnxyls.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ws.gzmigu.cn

[J04] 时间戳与日期互转
来源：http://tx.haigaiapp.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xo.huixiangedu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ao.shtwfgs.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jj.jctech888.com.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cm.szxytkj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yp.huanxung.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nh.haigaiapp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wb.yuexingan06.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qe.shtwfgs.cn

[J05] 时间加减（加 7 天）
来源：http://ti.jctech888.com.cn

Py:   now + timedelta(days=7)
来源：http://hz.shxzukj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qk.panjiajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://js.haigaiapp.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zu.newstarts.cn

Java: LocalDate.now().plusDays(7)
来源：http://li.nicolike.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cf.huanxung.cn

Ruby: Time.now + 7 * 86400
来源：http://mb.9csxet.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wb.yuexingan06.cn

[J06] 计算两时间之差
来源：http://jt.shxzukj.cn

Py:   (end - start).total_seconds()
来源：http://wr.gzmigu.cn

PHP:  $end->diff($start)->days;
来源：http://np.newstarts.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hd.gzmigu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jc.huixiangedu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://yg.jianghongdianzi.cn

Go:   end.Sub(start).Hours()
来源：http://mp.shtwfgs.cn

Ruby: end - start                 # 返回秒数
来源：http://yb.yuntaijiaju.cn

C#:   (end - start).TotalSeconds
来源：http://sa.lnxyls.cn

[J07] 比较两个日期
来源：http://fk.521024.cn

Py:   d1 < d2;  d1 == d2
来源：http://hy.521024.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://aj.shtwfgs.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xo.shtwfgs.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bu.huanxung.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://oz.colortex.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://eu.shxzukj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pp.huixinmuqiang.cn

C#:   d1 < d2;  d1 == d2
来源：http://pu.nicolike.cn

[J08] 提取年月日与星期
来源：http://oz.9csxet.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dn.newstarts.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nk.shtwfgs.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tu.bjjhwx.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fz.muxihuayi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rv.hahajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ot.bjjhwx.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pq.9csxet.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dw.shtwfgs.cn

[J09] 时区处理
来源：http://ua.bookmarksfly.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kz.bookmarksfly.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vc.hahajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mn.chemitech.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://by.colortex.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tm.szxytkj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kk.9csxet.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gt.haigaiapp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://er.wgjwhj.cn

[J10] 取今天 / 本月第一天
来源：http://gz.nicolike.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://yp.huixinmuqiang.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xg.hnjuh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qa.newstarts.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jw.muxihuayi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ly.asd995.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pr.521024.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ai.yuexingan06.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tv.szxytkj.cn

================================================================================
来源：http://kt.huixiangedu.cn

K. JSON 与序列化
来源：http://rt.colortex.cn

================================================================================
来源：http://gv.muxihuayi.cn

[K01] 对象转 JSON 字符串
来源：http://fa.muxihuayi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fw.shxzskj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zs.szxytkj.cn

JS:   JSON.stringify(obj)
来源：http://vd.colortex.cn

TS:   JSON.stringify(obj)
来源：http://hk.gzmigu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sr.nicolike.cn

Go:   json.Marshal(obj)
来源：http://ua.shtwfgs.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gi.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vu.colortex.cn

[K02] JSON 字符串转对象
来源：http://mv.nicolike.cn

Py:   json.loads(s)
来源：http://fg.colortex.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.521024.cn

JS:   JSON.parse(s)
来源：http://so.521024.cn

TS:   JSON.parse(s)
来源：http://we.szsharing.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hv.newstarts.cn

Go:   json.Unmarshal(data, &v)
来源：http://xd.huixiangedu.cn

Ruby: JSON.parse(s)
来源：http://jf.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kv.panjiajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://am.asd995.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ry.shxzukj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nk.huixiangedu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://df.lnxyls.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ka.asd995.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vi.bjjhwx.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zh.muxihuayi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ng.huanxung.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wd.szxytkj.cn

[K04] 读取 JSON 文件
来源：http://lk.haigaiapp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qd.wgjwhj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://va.hnjuh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nc.asd995.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oo.newstarts.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cj.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kh.chemitech.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ws.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dt.9csxet.cn

[K05] 深拷贝对象
来源：http://st.newstarts.cn

Py:   copy.deepcopy(obj)
来源：http://eg.huixiangedu.cn

PHP:  unserialize(serialize($obj));
来源：http://zj.yuntaijiaju.cn

JS:   structuredClone(obj)
来源：http://xl.shtwfgs.cn

TS:   structuredClone(obj)
来源：http://lb.wgjwhj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://lb.bjjhwx.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ty.huixiangedu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ze.nszjky.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ya.hnjuh.cn

[K06] 解析 URL 查询串
来源：http://jg.gzmigu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bi.9csxet.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gm.chemitech.net.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ba.huixinmuqiang.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ky.yuntaijiaju.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://md.chemitech.net.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ii.szxytkj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jd.szxytkj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qw.haigaiapp.cn

[K07] 进制转换
来源：http://td.hahajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sd.huixiangedu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lh.asd995.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://oi.yuntaijiaju.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zt.shtwfgs.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ry.haigaiapp.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ig.wgjwhj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://so.shxzskj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ky.gzmigu.cn

[K08] 二进制序列化（非 JSON）
来源：http://ft.9csxet.cn

Py:   pickle.dumps(obj)
来源：http://cg.haigaiapp.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://by.jianghongdianzi.cn

JS:   v8.serialize(obj)        // Node
来源：http://mj.shxzskj.cn

TS:   v8.serialize(obj)        // Node
来源：http://xe.bookmarksfly.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lg.jianghongdianzi.cn

Go:   encoding/gob
来源：http://jf.yuntaijiaju.cn

Ruby: Marshal.dump(obj)
来源：http://aw.haigaiapp.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qh.haigaiapp.cn

================================================================================
来源：http://kc.yuexingan06.cn

L. 网络请求
来源：http://df.asd995.cn

================================================================================
来源：http://vo.nszjky.cn

[L01] 发送 GET 请求
来源：http://dz.wgjwhj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ek.panjiajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ik.lnxyls.cn

JS:   await fetch(url)
来源：http://fv.gzmigu.cn

TS:   await fetch(url)
来源：http://wi.shxzskj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gi.bjjhwx.cn

Go:   resp, err := http.Get(url)
来源：http://jm.shtwfgs.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://od.yuexingan06.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kg.nicolike.cn

[L02] 发送 POST JSON
来源：http://rs.shtwfgs.cn

Py:   requests.post(url, json={"a": 1})
来源：http://oy.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xj.szxytkj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pq.huixinmuqiang.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mh.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hy.hahajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jv.szsharing.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yr.nicolike.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jz.shxzskj.cn

[L03] 设置自定义请求头
来源：http://jh.shxzskj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://os.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bi.521024.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ua.jianghongdianzi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xv.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ex.newstarts.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lx.huixinmuqiang.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ud.bjjhwx.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://oq.bjjhwx.cn

[L04] 设置超时
来源：http://xp.hnjuh.cn

Py:   requests.get(url, timeout=5)
来源：http://yd.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fd.newstarts.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dw.muxihuayi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cu.muxihuayi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hv.yuntaijiaju.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rb.panjiajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pj.hnjuh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qx.shxzskj.cn

[L05] 上传文件（multipart）
来源：http://lb.huixinmuqiang.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dg.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mn.asd995.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zh.bjjhwx.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zg.colortex.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ts.jianghongdianzi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gg.hnjuh.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wp.9csxet.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ur.gzmigu.cn

[L06] 解析响应为 JSON
来源：http://zk.bookmarksfly.cn

Py:   resp.json()
来源：http://ka.bookmarksfly.cn

PHP:  json_decode($body, true);
来源：http://pj.nszjky.cn

JS:   await resp.json()
来源：http://zz.haigaiapp.cn

TS:   await resp.json()
来源：http://nh.gzmigu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://im.colortex.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dc.nicolike.cn

Ruby: JSON.parse(resp.body)
来源：http://il.szxytkj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://aa.szsharing.cn

[L07] 处理 HTTP 状态码
来源：http://gl.muxihuayi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zo.9csxet.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tp.yuntaijiaju.cn

JS:   resp.ok;  resp.status
来源：http://st.shxzukj.cn

TS:   resp.ok;  resp.status
来源：http://wp.huixinmuqiang.cn

Java: resp.statusCode()
来源：http://tl.chemitech.net.cn

Go:   resp.StatusCode
来源：http://xd.panjiajie.cn

Ruby: resp.code.to_i
来源：http://az.colortex.cn

C#:   (int)resp.StatusCode
来源：http://ys.muxihuayi.cn

[L08] 并发请求多个地址
来源：http://hp.hnjuh.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hn.hahajie.cn

PHP:  curl_multi_init() 系列
来源：http://mm.szsharing.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dd.asd995.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xq.gzmigu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tv.wgjwhj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://er.9csxet.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hd.hnjuh.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wm.huixinmuqiang.cn

================================================================================
来源：http://yn.lnxyls.cn

M. 命令行 / 进程 / 环境
来源：http://sp.muxihuayi.cn

================================================================================
来源：http://nv.chemitech.net.cn

[M01] 读取命令行参数
来源：http://jv.nicolike.cn

Py:   sys.argv[1:]
来源：http://zm.bjjhwx.cn

PHP:  $argv;  $argc;
来源：http://nc.yuntaijiaju.cn

JS:   process.argv.slice(2)
来源：http://gt.jctech888.com.cn

TS:   process.argv.slice(2)
来源：http://up.asd995.cn

Java: args 数组（main 方法参数）
来源：http://jx.yuntaijiaju.cn

Go:   os.Args[1:]
来源：http://ce.muxihuayi.cn

Ruby: ARGV
来源：http://um.gzmigu.cn

C#:   args 数组（Main 方法参数）
来源：http://yr.szxytkj.cn

[M02] 读取环境变量
来源：http://cx.huixinmuqiang.cn

Py:   os.environ.get("HOME")
来源：http://qe.nicolike.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ti.jianghongdianzi.cn

JS:   process.env.HOME
来源：http://sj.nszjky.cn

TS:   process.env.HOME
来源：http://cg.szsharing.cn

Java: System.getenv("HOME")
来源：http://my.chemitech.net.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vp.521024.cn

Ruby: ENV["HOME"]
来源：http://ev.yuexingan06.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dq.yuntaijiaju.cn

[M03] 执行外部命令
来源：http://hj.shtwfgs.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rk.hnjuh.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yw.newstarts.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://lo.huanxung.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ga.nszjky.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qq.jctech888.com.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vt.jctech888.com.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hn.szsharing.cn

C#:   Process.Start("ls", "-l");
来源：http://tv.newstarts.cn

[M04] 获取当前工作目录
来源：http://ui.jianghongdianzi.cn

Py:   os.getcwd()
来源：http://ek.bookmarksfly.cn

PHP:  getcwd();
来源：http://xk.9csxet.cn

JS:   process.cwd()
来源：http://xo.szsharing.cn

TS:   process.cwd()
来源：http://qx.huanxung.cn

Java: Path.of("").toAbsolutePath()
来源：http://wr.nicolike.cn

Go:   os.Getwd()
来源：http://rx.521024.cn

Ruby: Dir.pwd
来源：http://pc.panjiajie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://lq.szsharing.cn

[M05] 设置退出码
来源：http://yv.gzmigu.cn

Py:   sys.exit(1)
来源：http://xc.muxihuayi.cn

PHP:  exit(1);
来源：http://fo.gzmigu.cn

JS:   process.exit(1)
来源：http://uc.bookmarksfly.cn

TS:   process.exit(1)
来源：http://ac.bookmarksfly.cn

Java: System.exit(1)
来源：http://ei.colortex.cn

Go:   os.Exit(1)
来源：http://yk.huixinmuqiang.cn

Ruby: exit 1
来源：http://kg.shxzskj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ex.asd995.cn

[M06] 向标准错误输出
来源：http://wy.szxytkj.cn

Py:   print("err", file=sys.stderr)
来源：http://me.521024.cn


<!-- 参考信息 -->