代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://se.shxzskj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://av.9csxet.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ku.huanxung.cn

================================================================================
来源：http://ms.hnjuh.cn

J. 日期与时间
来源：http://er.lnxyls.cn

================================================================================
来源：http://nt.chemitech.net.cn

[J01] 获取当前时间
来源：http://gx.yuntaijiaju.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fr.shxzukj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ra.shxzskj.cn

JS:   new Date();  Date.now()
来源：http://sg.9csxet.cn

TS:   new Date();  Date.now()
来源：http://qq.shxzskj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ut.shxzskj.cn

Go:   time.Now()
来源：http://xe.nicolike.cn

Ruby: Time.now
来源：http://he.chemitech.net.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fy.bjjhwx.cn

[J02] 格式化输出
来源：http://ad.shxzskj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ut.bookmarksfly.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bp.huixinmuqiang.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://on.hnjuh.cn

TS:   d.toISOString()
来源：http://ov.huanxung.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lz.hahajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gw.wgjwhj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ig.gzmigu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qr.szxytkj.cn

[J03] 字符串解析为日期
来源：http://fv.jianghongdianzi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ew.muxihuayi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gd.lnxyls.cn

JS:   new Date("2024-01-02")
来源：http://cj.bjjhwx.cn

TS:   new Date("2024-01-02")
来源：http://du.asd995.cn

Java: LocalDate.parse("2024-01-02")
来源：http://kc.lnxyls.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cn.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://mg.haigaiapp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xw.colortex.cn

[J04] 时间戳与日期互转
来源：http://hx.panjiajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yg.521024.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yf.shxzskj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ex.shxzskj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gl.jctech888.com.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tq.gzmigu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ai.haigaiapp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qn.nicolike.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xa.521024.cn

[J05] 时间加减（加 7 天）
来源：http://sg.9csxet.cn

Py:   now + timedelta(days=7)
来源：http://bz.bjjhwx.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qt.shxzskj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ck.521024.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cu.hnjuh.cn

Java: LocalDate.now().plusDays(7)
来源：http://tc.shtwfgs.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://br.szsharing.cn

Ruby: Time.now + 7 * 86400
来源：http://wk.bjjhwx.cn

C#:   DateTime.Now.AddDays(7)
来源：http://aq.shxzskj.cn

[J06] 计算两时间之差
来源：http://qe.shxzskj.cn

Py:   (end - start).total_seconds()
来源：http://pa.nicolike.cn

PHP:  $end->diff($start)->days;
来源：http://ri.yuntaijiaju.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ft.9csxet.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://os.yuntaijiaju.cn

Java: Duration.between(start, end).toSeconds()
来源：http://by.hahajie.cn

Go:   end.Sub(start).Hours()
来源：http://ai.huanxung.cn

Ruby: end - start                 # 返回秒数
来源：http://qk.szxytkj.cn

C#:   (end - start).TotalSeconds
来源：http://hu.521024.cn

[J07] 比较两个日期
来源：http://zh.panjiajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://gi.521024.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mc.wgjwhj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://sw.chemitech.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ux.gzmigu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tm.hahajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rp.gzmigu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lr.muxihuayi.cn

C#:   d1 < d2;  d1 == d2
来源：http://dl.shxzskj.cn

[J08] 提取年月日与星期
来源：http://bv.huixiangedu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://iz.yuexingan06.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qx.huixiangedu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ha.bookmarksfly.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ra.panjiajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://re.jctech888.com.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ji.newstarts.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zz.wgjwhj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cf.newstarts.cn

[J09] 时区处理
来源：http://op.muxihuayi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mz.huixiangedu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pm.lnxyls.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bm.nicolike.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rj.asd995.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bu.nszjky.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yx.yuntaijiaju.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ca.hnjuh.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://la.huixiangedu.cn

[J10] 取今天 / 本月第一天
来源：http://wr.huanxung.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bj.nicolike.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zs.colortex.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qt.huanxung.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zi.gzmigu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hu.hahajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xj.asd995.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://me.bjjhwx.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oh.521024.cn

================================================================================
来源：http://bt.yuntaijiaju.cn

K. JSON 与序列化
来源：http://ow.wgjwhj.cn

================================================================================
来源：http://lo.chemitech.net.cn

[K01] 对象转 JSON 字符串
来源：http://qz.huanxung.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://eh.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xa.szsharing.cn

JS:   JSON.stringify(obj)
来源：http://dl.muxihuayi.cn

TS:   JSON.stringify(obj)
来源：http://gq.gzmigu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cd.asd995.cn

Go:   json.Marshal(obj)
来源：http://iy.shtwfgs.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ch.lnxyls.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qn.huanxung.cn

[K02] JSON 字符串转对象
来源：http://nu.huixiangedu.cn

Py:   json.loads(s)
来源：http://kc.yuntaijiaju.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xf.bookmarksfly.cn

JS:   JSON.parse(s)
来源：http://qi.bjjhwx.cn

TS:   JSON.parse(s)
来源：http://dn.jianghongdianzi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://db.colortex.cn

Go:   json.Unmarshal(data, &v)
来源：http://wc.nszjky.cn

Ruby: JSON.parse(s)
来源：http://je.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kq.huixiangedu.cn

[K03] JSON 美化输出（带缩进）
来源：http://kt.wgjwhj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://md.9csxet.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fm.asd995.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jm.jctech888.com.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mh.chemitech.net.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ve.panjiajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://in.huixinmuqiang.cn

Ruby: JSON.pretty_generate(obj)
来源：http://oh.shxzskj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://st.huixinmuqiang.cn

[K04] 读取 JSON 文件
来源：http://ch.9csxet.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fa.521024.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nl.yuntaijiaju.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://js.panjiajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fy.hnjuh.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yb.gzmigu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://an.newstarts.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ac.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nl.szsharing.cn

[K05] 深拷贝对象
来源：http://rc.huixinmuqiang.cn

Py:   copy.deepcopy(obj)
来源：http://os.szsharing.cn

PHP:  unserialize(serialize($obj));
来源：http://vr.shxzskj.cn

JS:   structuredClone(obj)
来源：http://ms.lnxyls.cn

TS:   structuredClone(obj)
来源：http://yv.bookmarksfly.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://pr.colortex.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sn.chemitech.net.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ax.huanxung.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pg.hnjuh.cn

[K06] 解析 URL 查询串
来源：http://nx.521024.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nj.shxzukj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lf.shxzukj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xo.521024.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yf.huixinmuqiang.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mm.colortex.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zc.muxihuayi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gg.yuexingan06.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ke.huixiangedu.cn

[K07] 进制转换
来源：http://ql.panjiajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ue.yuexingan06.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tb.shxzskj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ae.szsharing.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bw.jianghongdianzi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dd.newstarts.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gf.9csxet.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oi.hahajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bh.bjjhwx.cn

[K08] 二进制序列化（非 JSON）
来源：http://rt.nszjky.cn

Py:   pickle.dumps(obj)
来源：http://bl.nszjky.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ii.muxihuayi.cn

JS:   v8.serialize(obj)        // Node
来源：http://gg.wgjwhj.cn

TS:   v8.serialize(obj)        // Node
来源：http://yy.lnxyls.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hf.asd995.cn

Go:   encoding/gob
来源：http://kh.bjjhwx.cn

Ruby: Marshal.dump(obj)
来源：http://hw.jctech888.com.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xf.szxytkj.cn

================================================================================
来源：http://jp.shxzskj.cn

L. 网络请求
来源：http://ly.huixiangedu.cn

================================================================================
来源：http://zn.szsharing.cn

[L01] 发送 GET 请求
来源：http://rt.shxzskj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lg.jctech888.com.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ng.chemitech.net.cn

JS:   await fetch(url)
来源：http://se.huanxung.cn

TS:   await fetch(url)
来源：http://yt.huixiangedu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ew.szxytkj.cn

Go:   resp, err := http.Get(url)
来源：http://uf.nicolike.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zb.shtwfgs.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jz.colortex.cn

[L02] 发送 POST JSON
来源：http://hb.szxytkj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://tv.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vj.bjjhwx.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ap.nszjky.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qy.asd995.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tf.jctech888.com.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rm.chemitech.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ya.yuexingan06.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://km.huixiangedu.cn

[L03] 设置自定义请求头
来源：http://mc.muxihuayi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jg.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yr.nszjky.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ro.bjjhwx.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qc.colortex.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jy.yuntaijiaju.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ns.chemitech.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xd.shtwfgs.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sp.521024.cn

[L04] 设置超时
来源：http://dt.asd995.cn

Py:   requests.get(url, timeout=5)
来源：http://cb.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mb.hahajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zg.nicolike.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bk.colortex.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ku.huixinmuqiang.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://iz.yuntaijiaju.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wk.9csxet.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fq.bookmarksfly.cn

[L05] 上传文件（multipart）
来源：http://gr.jianghongdianzi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://on.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gu.colortex.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ze.521024.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mk.521024.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://di.wgjwhj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uo.jianghongdianzi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yn.521024.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pt.huanxung.cn

[L06] 解析响应为 JSON
来源：http://kz.newstarts.cn

Py:   resp.json()
来源：http://dw.hahajie.cn

PHP:  json_decode($body, true);
来源：http://to.huixinmuqiang.cn

JS:   await resp.json()
来源：http://cn.haigaiapp.cn

TS:   await resp.json()
来源：http://hr.yuexingan06.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ks.hahajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wb.huixinmuqiang.cn

Ruby: JSON.parse(resp.body)
来源：http://tt.wgjwhj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qi.wgjwhj.cn

[L07] 处理 HTTP 状态码
来源：http://pl.lnxyls.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ot.jctech888.com.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cy.lnxyls.cn

JS:   resp.ok;  resp.status
来源：http://vg.yuexingan06.cn

TS:   resp.ok;  resp.status
来源：http://bk.shxzskj.cn

Java: resp.statusCode()
来源：http://vy.nicolike.cn

Go:   resp.StatusCode
来源：http://qp.haigaiapp.cn

Ruby: resp.code.to_i
来源：http://wb.yuexingan06.cn

C#:   (int)resp.StatusCode
来源：http://ve.muxihuayi.cn

[L08] 并发请求多个地址
来源：http://jj.jctech888.com.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tz.panjiajie.cn

PHP:  curl_multi_init() 系列
来源：http://wu.nszjky.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ju.nszjky.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dy.colortex.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qn.wgjwhj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yt.muxihuayi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zp.haigaiapp.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xw.9csxet.cn

================================================================================
来源：http://ps.chemitech.net.cn

M. 命令行 / 进程 / 环境
来源：http://uw.muxihuayi.cn

================================================================================
来源：http://ey.newstarts.cn

[M01] 读取命令行参数
来源：http://ki.colortex.cn

Py:   sys.argv[1:]
来源：http://fc.yuexingan06.cn

PHP:  $argv;  $argc;
来源：http://hf.huixinmuqiang.cn

JS:   process.argv.slice(2)
来源：http://yt.lnxyls.cn

TS:   process.argv.slice(2)
来源：http://gw.huixiangedu.cn

Java: args 数组（main 方法参数）
来源：http://zs.yuexingan06.cn

Go:   os.Args[1:]
来源：http://gd.jctech888.com.cn

Ruby: ARGV
来源：http://kx.bjjhwx.cn

C#:   args 数组（Main 方法参数）
来源：http://cc.yuexingan06.cn

[M02] 读取环境变量
来源：http://fv.hahajie.cn

Py:   os.environ.get("HOME")
来源：http://jk.521024.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vh.szxytkj.cn

JS:   process.env.HOME
来源：http://wo.szxytkj.cn

TS:   process.env.HOME
来源：http://wo.bookmarksfly.cn

Java: System.getenv("HOME")
来源：http://rs.panjiajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bv.nszjky.cn

Ruby: ENV["HOME"]
来源：http://xt.hnjuh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sd.jianghongdianzi.cn

[M03] 执行外部命令
来源：http://lj.jctech888.com.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kb.yuexingan06.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dp.asd995.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ht.shtwfgs.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wl.chemitech.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rs.nszjky.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://cl.chemitech.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ie.shtwfgs.cn

C#:   Process.Start("ls", "-l");
来源：http://pk.panjiajie.cn

[M04] 获取当前工作目录
来源：http://hp.huixiangedu.cn

Py:   os.getcwd()
来源：http://qj.shxzskj.cn

PHP:  getcwd();
来源：http://jc.newstarts.cn

JS:   process.cwd()
来源：http://my.panjiajie.cn

TS:   process.cwd()
来源：http://zo.panjiajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://le.gzmigu.cn

Go:   os.Getwd()
来源：http://id.huixiangedu.cn

Ruby: Dir.pwd
来源：http://sk.bookmarksfly.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ui.panjiajie.cn

[M05] 设置退出码
来源：http://qj.yuexingan06.cn

Py:   sys.exit(1)
来源：http://bw.nicolike.cn

PHP:  exit(1);
来源：http://lz.bjjhwx.cn

JS:   process.exit(1)
来源：http://nk.nicolike.cn

TS:   process.exit(1)
来源：http://jk.huanxung.cn

Java: System.exit(1)
来源：http://mn.muxihuayi.cn

Go:   os.Exit(1)
来源：http://gc.hahajie.cn

Ruby: exit 1
来源：http://ao.bjjhwx.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mv.huixinmuqiang.cn

[M06] 向标准错误输出
来源：http://yb.nicolike.cn

Py:   print("err", file=sys.stderr)
来源：http://ky.huanxung.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://dc.nicolike.cn

JS:   console.error("err")
来源：http://cb.newstarts.cn

TS:   console.error("err")
来源：http://qv.hnjuh.cn

Java: System.err.println("err")
来源：http://kn.9csxet.cn


<!-- 参考信息 -->