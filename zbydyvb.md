代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ni.yuexingan06.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ah.nicolike.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nk.szxytkj.cn

================================================================================
来源：http://cn.lnxyls.cn

J. 日期与时间
来源：http://np.colortex.cn

================================================================================
来源：http://pe.shxzskj.cn

[J01] 获取当前时间
来源：http://he.jctech888.com.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://nu.szsharing.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lf.bjjhwx.cn

JS:   new Date();  Date.now()
来源：http://gy.huixiangedu.cn

TS:   new Date();  Date.now()
来源：http://kv.shxzukj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://nx.bookmarksfly.cn

Go:   time.Now()
来源：http://tk.shxzskj.cn

Ruby: Time.now
来源：http://tw.hnjuh.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://oj.shxzskj.cn

[J02] 格式化输出
来源：http://ae.chemitech.net.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mm.huanxung.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://un.asd995.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://if.asd995.cn

TS:   d.toISOString()
来源：http://qa.jianghongdianzi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tl.jctech888.com.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xt.jctech888.com.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zt.shtwfgs.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zw.lnxyls.cn

[J03] 字符串解析为日期
来源：http://cm.asd995.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lc.szxytkj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zu.newstarts.cn

JS:   new Date("2024-01-02")
来源：http://xi.muxihuayi.cn

TS:   new Date("2024-01-02")
来源：http://pq.asd995.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cr.szsharing.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ro.shxzskj.cn

Ruby: Date.parse("2024-01-02")
来源：http://xs.szsharing.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://au.bjjhwx.cn

[J04] 时间戳与日期互转
来源：http://xl.521024.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cx.colortex.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tt.chemitech.net.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pr.521024.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ax.521024.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xg.nszjky.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fz.lnxyls.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jr.yuexingan06.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cy.bookmarksfly.cn

[J05] 时间加减（加 7 天）
来源：http://ig.lnxyls.cn

Py:   now + timedelta(days=7)
来源：http://rg.hnjuh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wn.hahajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ck.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://eo.521024.cn

Java: LocalDate.now().plusDays(7)
来源：http://rg.haigaiapp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ib.huixinmuqiang.cn

Ruby: Time.now + 7 * 86400
来源：http://hj.huanxung.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gn.gzmigu.cn

[J06] 计算两时间之差
来源：http://gp.jctech888.com.cn

Py:   (end - start).total_seconds()
来源：http://sa.haigaiapp.cn

PHP:  $end->diff($start)->days;
来源：http://iy.jianghongdianzi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kn.asd995.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vt.9csxet.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xv.huixiangedu.cn

Go:   end.Sub(start).Hours()
来源：http://kt.jctech888.com.cn

Ruby: end - start                 # 返回秒数
来源：http://xu.9csxet.cn

C#:   (end - start).TotalSeconds
来源：http://hy.nicolike.cn

[J07] 比较两个日期
来源：http://pp.lnxyls.cn

Py:   d1 < d2;  d1 == d2
来源：http://hw.panjiajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://iy.lnxyls.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jp.szsharing.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jy.hnjuh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kz.chemitech.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jh.colortex.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fz.haigaiapp.cn

C#:   d1 < d2;  d1 == d2
来源：http://mh.haigaiapp.cn

[J08] 提取年月日与星期
来源：http://ks.szsharing.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://do.shxzukj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dv.shxzukj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mx.huanxung.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ky.newstarts.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pa.9csxet.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dl.shtwfgs.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yx.huixiangedu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hl.bjjhwx.cn

[J09] 时区处理
来源：http://qx.shxzukj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ha.chemitech.net.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vl.huixinmuqiang.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vw.yuexingan06.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ed.panjiajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://iv.huanxung.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cm.hahajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://rz.shxzukj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pb.chemitech.net.cn

[J10] 取今天 / 本月第一天
来源：http://xb.9csxet.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://by.chemitech.net.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cz.nszjky.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ql.newstarts.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yc.nszjky.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vp.huanxung.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ll.9csxet.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cc.huanxung.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zc.hnjuh.cn

================================================================================
来源：http://si.chemitech.net.cn

K. JSON 与序列化
来源：http://ov.wgjwhj.cn

================================================================================
来源：http://zc.huixinmuqiang.cn

[K01] 对象转 JSON 字符串
来源：http://yx.nszjky.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ny.colortex.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ao.haigaiapp.cn

JS:   JSON.stringify(obj)
来源：http://ci.nicolike.cn

TS:   JSON.stringify(obj)
来源：http://ss.9csxet.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ri.huanxung.cn

Go:   json.Marshal(obj)
来源：http://ul.nszjky.cn

Ruby: obj.to_json                                     // require "json"
来源：http://pl.nicolike.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://co.bookmarksfly.cn

[K02] JSON 字符串转对象
来源：http://fg.hnjuh.cn

Py:   json.loads(s)
来源：http://bo.szsharing.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bz.szsharing.cn

JS:   JSON.parse(s)
来源：http://xo.hahajie.cn

TS:   JSON.parse(s)
来源：http://xp.jctech888.com.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ow.lnxyls.cn

Go:   json.Unmarshal(data, &v)
来源：http://sl.yuntaijiaju.cn

Ruby: JSON.parse(s)
来源：http://xh.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zm.muxihuayi.cn

[K03] JSON 美化输出（带缩进）
来源：http://bq.shtwfgs.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pc.521024.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ss.jctech888.com.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vq.hahajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ep.chemitech.net.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://el.jctech888.com.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uv.newstarts.cn

Ruby: JSON.pretty_generate(obj)
来源：http://sx.szxytkj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ht.szsharing.cn

[K04] 读取 JSON 文件
来源：http://el.wgjwhj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rb.huixiangedu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jo.nicolike.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ev.nicolike.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aq.newstarts.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://iq.hahajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://oo.bjjhwx.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://oc.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qs.shtwfgs.cn

[K05] 深拷贝对象
来源：http://vv.nszjky.cn

Py:   copy.deepcopy(obj)
来源：http://po.shxzskj.cn

PHP:  unserialize(serialize($obj));
来源：http://fi.hnjuh.cn

JS:   structuredClone(obj)
来源：http://en.9csxet.cn

TS:   structuredClone(obj)
来源：http://zi.lnxyls.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fe.huanxung.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wb.bookmarksfly.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ya.muxihuayi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cs.yuntaijiaju.cn

[K06] 解析 URL 查询串
来源：http://ka.shxzukj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ha.huanxung.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zg.yuntaijiaju.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tu.nszjky.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ul.shxzukj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mz.newstarts.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wi.haigaiapp.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vi.jianghongdianzi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://je.muxihuayi.cn

[K07] 进制转换
来源：http://ab.hahajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tj.chemitech.net.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ip.jctech888.com.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gi.huanxung.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yf.szxytkj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://go.huixinmuqiang.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ml.bjjhwx.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kj.huixinmuqiang.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kl.szxytkj.cn

[K08] 二进制序列化（非 JSON）
来源：http://xs.bjjhwx.cn

Py:   pickle.dumps(obj)
来源：http://vs.lnxyls.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cm.bjjhwx.cn

JS:   v8.serialize(obj)        // Node
来源：http://cm.newstarts.cn

TS:   v8.serialize(obj)        // Node
来源：http://kt.yuntaijiaju.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lx.jctech888.com.cn

Go:   encoding/gob
来源：http://qu.521024.cn

Ruby: Marshal.dump(obj)
来源：http://ep.nicolike.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lx.bjjhwx.cn

================================================================================
来源：http://mk.huixiangedu.cn

L. 网络请求
来源：http://cc.nicolike.cn

================================================================================
来源：http://wk.bjjhwx.cn

[L01] 发送 GET 请求
来源：http://in.szsharing.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lq.szsharing.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cd.hnjuh.cn

JS:   await fetch(url)
来源：http://hh.hahajie.cn

TS:   await fetch(url)
来源：http://dx.521024.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nb.asd995.cn

Go:   resp, err := http.Get(url)
来源：http://fw.bjjhwx.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jg.nicolike.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ti.szxytkj.cn

[L02] 发送 POST JSON
来源：http://wp.nicolike.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xb.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hi.huanxung.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zj.wgjwhj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wz.asd995.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tv.bjjhwx.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rf.szsharing.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jj.huixiangedu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wx.bookmarksfly.cn

[L03] 设置自定义请求头
来源：http://cm.newstarts.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mo.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yo.yuntaijiaju.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kn.bjjhwx.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bz.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qr.muxihuayi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sn.huanxung.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cu.shxzukj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bl.szxytkj.cn

[L04] 设置超时
来源：http://zd.yuntaijiaju.cn

Py:   requests.get(url, timeout=5)
来源：http://vd.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://av.huixinmuqiang.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wo.nicolike.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nz.gzmigu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gj.jctech888.com.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://je.bookmarksfly.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hl.wgjwhj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vw.wgjwhj.cn

[L05] 上传文件（multipart）
来源：http://zc.huixiangedu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hs.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://du.yuexingan06.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://by.muxihuayi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://au.muxihuayi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fi.szxytkj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cp.asd995.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qt.huanxung.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xf.asd995.cn

[L06] 解析响应为 JSON
来源：http://kc.huixiangedu.cn

Py:   resp.json()
来源：http://ed.shxzskj.cn

PHP:  json_decode($body, true);
来源：http://rc.huixiangedu.cn

JS:   await resp.json()
来源：http://od.szxytkj.cn

TS:   await resp.json()
来源：http://lp.hnjuh.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://er.chemitech.net.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nh.huixiangedu.cn

Ruby: JSON.parse(resp.body)
来源：http://mk.shxzskj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zo.muxihuayi.cn

[L07] 处理 HTTP 状态码
来源：http://bn.wgjwhj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fj.huixiangedu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ap.huixiangedu.cn

JS:   resp.ok;  resp.status
来源：http://jw.521024.cn

TS:   resp.ok;  resp.status
来源：http://vk.lnxyls.cn

Java: resp.statusCode()
来源：http://xa.haigaiapp.cn

Go:   resp.StatusCode
来源：http://ua.9csxet.cn

Ruby: resp.code.to_i
来源：http://nj.newstarts.cn

C#:   (int)resp.StatusCode
来源：http://xo.asd995.cn

[L08] 并发请求多个地址
来源：http://qr.shtwfgs.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sv.yuntaijiaju.cn

PHP:  curl_multi_init() 系列
来源：http://yd.hahajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rg.asd995.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://re.haigaiapp.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://eq.hnjuh.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sv.shxzukj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xz.yuexingan06.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jz.newstarts.cn

================================================================================
来源：http://yc.shtwfgs.cn

M. 命令行 / 进程 / 环境
来源：http://aq.bookmarksfly.cn

================================================================================
来源：http://rj.lnxyls.cn

[M01] 读取命令行参数
来源：http://kr.lnxyls.cn

Py:   sys.argv[1:]
来源：http://hq.colortex.cn

PHP:  $argv;  $argc;
来源：http://gv.shxzskj.cn

JS:   process.argv.slice(2)
来源：http://fl.jianghongdianzi.cn

TS:   process.argv.slice(2)
来源：http://ch.huixiangedu.cn

Java: args 数组（main 方法参数）
来源：http://iw.bjjhwx.cn

Go:   os.Args[1:]
来源：http://nm.shtwfgs.cn

Ruby: ARGV
来源：http://sj.shxzskj.cn

C#:   args 数组（Main 方法参数）
来源：http://dd.bjjhwx.cn

[M02] 读取环境变量
来源：http://fd.hahajie.cn

Py:   os.environ.get("HOME")
来源：http://jl.colortex.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fc.lnxyls.cn

JS:   process.env.HOME
来源：http://in.chemitech.net.cn

TS:   process.env.HOME
来源：http://tz.muxihuayi.cn

Java: System.getenv("HOME")
来源：http://zr.nicolike.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lz.huixinmuqiang.cn

Ruby: ENV["HOME"]
来源：http://ue.muxihuayi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sa.huixiangedu.cn

[M03] 执行外部命令
来源：http://ep.szxytkj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wa.shxzukj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jt.newstarts.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dw.nszjky.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gx.muxihuayi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lw.nszjky.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://co.hnjuh.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xs.9csxet.cn

C#:   Process.Start("ls", "-l");
来源：http://wl.jctech888.com.cn

[M04] 获取当前工作目录
来源：http://pt.gzmigu.cn

Py:   os.getcwd()
来源：http://ok.newstarts.cn

PHP:  getcwd();
来源：http://dq.muxihuayi.cn

JS:   process.cwd()
来源：http://hy.muxihuayi.cn

TS:   process.cwd()
来源：http://nn.huanxung.cn

Java: Path.of("").toAbsolutePath()
来源：http://mv.wgjwhj.cn

Go:   os.Getwd()
来源：http://zj.jctech888.com.cn

Ruby: Dir.pwd
来源：http://uq.bookmarksfly.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rx.muxihuayi.cn

[M05] 设置退出码
来源：http://jq.hnjuh.cn

Py:   sys.exit(1)
来源：http://qz.newstarts.cn

PHP:  exit(1);
来源：http://yz.wgjwhj.cn

JS:   process.exit(1)
来源：http://xp.huixinmuqiang.cn

TS:   process.exit(1)
来源：http://oi.bjjhwx.cn

Java: System.exit(1)
来源：http://hi.gzmigu.cn

Go:   os.Exit(1)
来源：http://ez.lnxyls.cn

Ruby: exit 1
来源：http://wl.szxytkj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://px.yuntaijiaju.cn

[M06] 向标准错误输出
来源：http://ql.shxzukj.cn

Py:   print("err", file=sys.stderr)
来源：http://vr.521024.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ld.muxihuayi.cn

JS:   console.error("err")
来源：http://jt.hnjuh.cn

TS:   console.error("err")
来源：http://qm.gzmigu.cn

Java: System.err.println("err")
来源：http://wt.chemitech.net.cn


<!-- 参考信息 -->