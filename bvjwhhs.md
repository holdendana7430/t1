代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ov.9csxet.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ar.yuexingan06.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cr.gzmigu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zt.yuexingan06.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yi.jianghongdianzi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zi.yuntaijiaju.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://oz.chemitech.net.cn

================================================================================
来源：http://pi.shtwfgs.cn

J. 日期与时间
来源：http://gc.nicolike.cn

================================================================================
来源：http://ef.lnxyls.cn

[J01] 获取当前时间
来源：http://iq.9csxet.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vd.huixinmuqiang.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sl.yuexingan06.cn

JS:   new Date();  Date.now()
来源：http://cm.nicolike.cn

TS:   new Date();  Date.now()
来源：http://uf.chemitech.net.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pl.bjjhwx.cn

Go:   time.Now()
来源：http://kd.9csxet.cn

Ruby: Time.now
来源：http://er.colortex.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://em.asd995.cn

[J02] 格式化输出
来源：http://cx.wgjwhj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zc.panjiajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ve.huanxung.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ww.jianghongdianzi.cn

TS:   d.toISOString()
来源：http://uu.szxytkj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tc.hahajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sj.shtwfgs.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hc.9csxet.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://va.hnjuh.cn

[J03] 字符串解析为日期
来源：http://df.shxzskj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ip.yuexingan06.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ov.hahajie.cn

JS:   new Date("2024-01-02")
来源：http://wn.newstarts.cn

TS:   new Date("2024-01-02")
来源：http://ol.shxzskj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ki.asd995.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ol.szxytkj.cn

Ruby: Date.parse("2024-01-02")
来源：http://gq.colortex.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://la.lnxyls.cn

[J04] 时间戳与日期互转
来源：http://bj.szsharing.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nv.hnjuh.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ti.nicolike.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vg.jianghongdianzi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://kz.wgjwhj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://aw.huixiangedu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://js.asd995.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ij.hahajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bu.hnjuh.cn

[J05] 时间加减（加 7 天）
来源：http://gy.9csxet.cn

Py:   now + timedelta(days=7)
来源：http://so.newstarts.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://fe.muxihuayi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wa.wgjwhj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mj.huanxung.cn

Java: LocalDate.now().plusDays(7)
来源：http://br.huixinmuqiang.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.9csxet.cn

Ruby: Time.now + 7 * 86400
来源：http://ti.huixinmuqiang.cn

C#:   DateTime.Now.AddDays(7)
来源：http://my.gzmigu.cn

[J06] 计算两时间之差
来源：http://jy.bjjhwx.cn

Py:   (end - start).total_seconds()
来源：http://tc.jctech888.com.cn

PHP:  $end->diff($start)->days;
来源：http://vf.jctech888.com.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cm.panjiajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://er.9csxet.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ii.szsharing.cn

Go:   end.Sub(start).Hours()
来源：http://qy.gzmigu.cn

Ruby: end - start                 # 返回秒数
来源：http://qq.bjjhwx.cn

C#:   (end - start).TotalSeconds
来源：http://ax.shxzskj.cn

[J07] 比较两个日期
来源：http://wt.jctech888.com.cn

Py:   d1 < d2;  d1 == d2
来源：http://iu.hahajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://eq.lnxyls.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fv.bookmarksfly.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ao.shxzukj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kn.asd995.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qt.shtwfgs.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jh.lnxyls.cn

C#:   d1 < d2;  d1 == d2
来源：http://vp.yuexingan06.cn

[J08] 提取年月日与星期
来源：http://km.bjjhwx.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mw.hahajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rj.nicolike.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ou.nszjky.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rw.wgjwhj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://iz.panjiajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ah.nicolike.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://en.chemitech.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zw.shxzukj.cn

[J09] 时区处理
来源：http://er.yuntaijiaju.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dy.colortex.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vn.muxihuayi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sw.muxihuayi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bt.9csxet.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ec.yuntaijiaju.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://il.yuexingan06.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mt.jianghongdianzi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jv.newstarts.cn

[J10] 取今天 / 本月第一天
来源：http://ck.9csxet.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zt.huixinmuqiang.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zu.asd995.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bl.wgjwhj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ud.nszjky.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lh.shtwfgs.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://si.bookmarksfly.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zv.bjjhwx.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ke.szsharing.cn

================================================================================
来源：http://ay.9csxet.cn

K. JSON 与序列化
来源：http://rn.nicolike.cn

================================================================================
来源：http://wb.shxzukj.cn

[K01] 对象转 JSON 字符串
来源：http://nx.521024.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dt.szsharing.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zk.nicolike.cn

JS:   JSON.stringify(obj)
来源：http://od.hahajie.cn

TS:   JSON.stringify(obj)
来源：http://tm.bookmarksfly.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pf.yuexingan06.cn

Go:   json.Marshal(obj)
来源：http://sp.nszjky.cn

Ruby: obj.to_json                                     // require "json"
来源：http://sz.hahajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://du.huixinmuqiang.cn

[K02] JSON 字符串转对象
来源：http://iv.gzmigu.cn

Py:   json.loads(s)
来源：http://ad.bookmarksfly.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fi.wgjwhj.cn

JS:   JSON.parse(s)
来源：http://rd.jctech888.com.cn

TS:   JSON.parse(s)
来源：http://id.bjjhwx.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nu.panjiajie.cn

Go:   json.Unmarshal(data, &v)
来源：http://ka.hnjuh.cn

Ruby: JSON.parse(s)
来源：http://dh.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yu.gzmigu.cn

[K03] JSON 美化输出（带缩进）
来源：http://qv.huixinmuqiang.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hy.chemitech.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://he.hahajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://mb.shtwfgs.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nt.haigaiapp.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ow.nicolike.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ef.huanxung.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ru.hnjuh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xu.haigaiapp.cn

[K04] 读取 JSON 文件
来源：http://ku.szxytkj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://oh.haigaiapp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ru.haigaiapp.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lb.nszjky.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xk.9csxet.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://el.nicolike.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qf.jctech888.com.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://tv.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tb.hahajie.cn

[K05] 深拷贝对象
来源：http://po.9csxet.cn

Py:   copy.deepcopy(obj)
来源：http://qs.colortex.cn

PHP:  unserialize(serialize($obj));
来源：http://dp.wgjwhj.cn

JS:   structuredClone(obj)
来源：http://vw.muxihuayi.cn

TS:   structuredClone(obj)
来源：http://gk.shtwfgs.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mq.muxihuayi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sa.hnjuh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://to.hahajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xj.yuexingan06.cn

[K06] 解析 URL 查询串
来源：http://cw.huanxung.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://li.nszjky.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vt.hnjuh.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zn.wgjwhj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vm.jianghongdianzi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ce.haigaiapp.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ix.chemitech.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ir.yuexingan06.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://an.shtwfgs.cn

[K07] 进制转换
来源：http://nz.shtwfgs.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kv.521024.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nr.521024.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mm.colortex.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tw.nszjky.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fy.shxzskj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hm.panjiajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rx.panjiajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ds.asd995.cn

[K08] 二进制序列化（非 JSON）
来源：http://oe.hnjuh.cn

Py:   pickle.dumps(obj)
来源：http://lm.yuexingan06.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ez.szsharing.cn

JS:   v8.serialize(obj)        // Node
来源：http://iy.wgjwhj.cn

TS:   v8.serialize(obj)        // Node
来源：http://ua.huanxung.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://po.jianghongdianzi.cn

Go:   encoding/gob
来源：http://io.jctech888.com.cn

Ruby: Marshal.dump(obj)
来源：http://mx.muxihuayi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mm.szxytkj.cn

================================================================================
来源：http://ud.gzmigu.cn

L. 网络请求
来源：http://aa.9csxet.cn

================================================================================
来源：http://kb.521024.cn

[L01] 发送 GET 请求
来源：http://ou.bjjhwx.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pr.szsharing.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yt.shxzskj.cn

JS:   await fetch(url)
来源：http://ir.hnjuh.cn

TS:   await fetch(url)
来源：http://sj.szsharing.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hm.bookmarksfly.cn

Go:   resp, err := http.Get(url)
来源：http://fn.szxytkj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://md.9csxet.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fa.newstarts.cn

[L02] 发送 POST JSON
来源：http://of.521024.cn

Py:   requests.post(url, json={"a": 1})
来源：http://td.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ir.hnjuh.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ig.shxzukj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ym.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xo.wgjwhj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://iv.panjiajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ho.yuntaijiaju.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xc.shxzskj.cn

[L03] 设置自定义请求头
来源：http://vm.huixiangedu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qo.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://eg.panjiajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pq.panjiajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://to.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vg.hahajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xp.newstarts.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mh.shxzskj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kk.bjjhwx.cn

[L04] 设置超时
来源：http://fq.yuexingan06.cn

Py:   requests.get(url, timeout=5)
来源：http://eh.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://no.jctech888.com.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yr.hahajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ta.nicolike.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wt.szxytkj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sa.panjiajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gc.haigaiapp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vw.haigaiapp.cn

[L05] 上传文件（multipart）
来源：http://ri.hahajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kq.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yz.9csxet.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wa.jianghongdianzi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://az.hahajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mp.bjjhwx.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jg.yuntaijiaju.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://oz.bookmarksfly.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gp.szsharing.cn

[L06] 解析响应为 JSON
来源：http://jl.shxzskj.cn

Py:   resp.json()
来源：http://xb.szxytkj.cn

PHP:  json_decode($body, true);
来源：http://iz.panjiajie.cn

JS:   await resp.json()
来源：http://to.szsharing.cn

TS:   await resp.json()
来源：http://mi.huanxung.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xm.jctech888.com.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kd.huixinmuqiang.cn

Ruby: JSON.parse(resp.body)
来源：http://fd.nszjky.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hv.lnxyls.cn

[L07] 处理 HTTP 状态码
来源：http://wo.521024.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rj.521024.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://np.muxihuayi.cn

JS:   resp.ok;  resp.status
来源：http://zu.bjjhwx.cn

TS:   resp.ok;  resp.status
来源：http://ch.chemitech.net.cn

Java: resp.statusCode()
来源：http://oh.szxytkj.cn

Go:   resp.StatusCode
来源：http://qe.szsharing.cn

Ruby: resp.code.to_i
来源：http://xh.wgjwhj.cn

C#:   (int)resp.StatusCode
来源：http://dw.muxihuayi.cn

[L08] 并发请求多个地址
来源：http://dk.521024.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://db.muxihuayi.cn

PHP:  curl_multi_init() 系列
来源：http://bx.shxzskj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ky.nicolike.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ep.yuntaijiaju.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yp.nszjky.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://um.newstarts.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://um.9csxet.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qh.yuntaijiaju.cn

================================================================================
来源：http://yd.huixiangedu.cn

M. 命令行 / 进程 / 环境
来源：http://tq.yuntaijiaju.cn

================================================================================
来源：http://xt.nicolike.cn

[M01] 读取命令行参数
来源：http://wn.newstarts.cn

Py:   sys.argv[1:]
来源：http://tl.jianghongdianzi.cn

PHP:  $argv;  $argc;
来源：http://sn.bookmarksfly.cn

JS:   process.argv.slice(2)
来源：http://mj.nszjky.cn

TS:   process.argv.slice(2)
来源：http://vj.gzmigu.cn

Java: args 数组（main 方法参数）
来源：http://pp.9csxet.cn

Go:   os.Args[1:]
来源：http://qv.shxzskj.cn

Ruby: ARGV
来源：http://ok.panjiajie.cn

C#:   args 数组（Main 方法参数）
来源：http://oo.nszjky.cn

[M02] 读取环境变量
来源：http://ge.haigaiapp.cn

Py:   os.environ.get("HOME")
来源：http://er.nicolike.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tv.wgjwhj.cn

JS:   process.env.HOME
来源：http://vx.gzmigu.cn

TS:   process.env.HOME
来源：http://bk.gzmigu.cn

Java: System.getenv("HOME")
来源：http://ou.hahajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ux.shtwfgs.cn

Ruby: ENV["HOME"]
来源：http://lf.yuntaijiaju.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yz.9csxet.cn

[M03] 执行外部命令
来源：http://tn.yuntaijiaju.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://df.lnxyls.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cc.huanxung.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://mv.panjiajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xa.wgjwhj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nh.haigaiapp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wq.wgjwhj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://du.521024.cn

C#:   Process.Start("ls", "-l");
来源：http://ex.yuntaijiaju.cn

[M04] 获取当前工作目录
来源：http://he.jianghongdianzi.cn

Py:   os.getcwd()
来源：http://cg.szsharing.cn

PHP:  getcwd();
来源：http://bs.haigaiapp.cn

JS:   process.cwd()
来源：http://bc.haigaiapp.cn

TS:   process.cwd()
来源：http://zt.wgjwhj.cn

Java: Path.of("").toAbsolutePath()
来源：http://pt.9csxet.cn

Go:   os.Getwd()
来源：http://ro.muxihuayi.cn

Ruby: Dir.pwd
来源：http://ml.521024.cn

C#:   Directory.GetCurrentDirectory()
来源：http://iv.hnjuh.cn

[M05] 设置退出码
来源：http://zd.hahajie.cn

Py:   sys.exit(1)
来源：http://qv.muxihuayi.cn

PHP:  exit(1);
来源：http://yw.shtwfgs.cn

JS:   process.exit(1)
来源：http://mk.szsharing.cn

TS:   process.exit(1)
来源：http://uk.nicolike.cn

Java: System.exit(1)
来源：http://su.haigaiapp.cn

Go:   os.Exit(1)
来源：http://lm.shxzskj.cn

Ruby: exit 1
来源：http://ro.yuexingan06.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jo.nicolike.cn

[M06] 向标准错误输出
来源：http://uk.shxzukj.cn

Py:   print("err", file=sys.stderr)
来源：http://xp.jianghongdianzi.cn


<!-- 参考信息 -->