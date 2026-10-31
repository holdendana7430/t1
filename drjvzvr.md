代发 wailian999

J. 日期与时间
来源：http://xt.521024.cn

================================================================================
来源：http://ed.yuexingan06.cn

[J01] 获取当前时间
来源：http://zg.chemitech.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wh.newstarts.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ab.panjiajie.cn

JS:   new Date();  Date.now()
来源：http://ls.bookmarksfly.cn

TS:   new Date();  Date.now()
来源：http://bk.gzmigu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rw.shxzskj.cn

Go:   time.Now()
来源：http://rk.huixiangedu.cn

Ruby: Time.now
来源：http://en.muxihuayi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://za.huixinmuqiang.cn

[J02] 格式化输出
来源：http://ij.nszjky.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pb.newstarts.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gx.shxzskj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xk.wgjwhj.cn

TS:   d.toISOString()
来源：http://ho.lnxyls.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lr.huanxung.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mf.gzmigu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vv.huanxung.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dw.muxihuayi.cn

[J03] 字符串解析为日期
来源：http://fw.gzmigu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://og.shtwfgs.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bz.yuexingan06.cn

JS:   new Date("2024-01-02")
来源：http://zh.521024.cn

TS:   new Date("2024-01-02")
来源：http://yw.colortex.cn

Java: LocalDate.parse("2024-01-02")
来源：http://nc.muxihuayi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hc.lnxyls.cn

Ruby: Date.parse("2024-01-02")
来源：http://sd.muxihuayi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gh.shxzukj.cn

[J04] 时间戳与日期互转
来源：http://sb.gzmigu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://np.shtwfgs.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nl.haigaiapp.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fq.gzmigu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vg.asd995.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kz.asd995.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://za.9csxet.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://df.jctech888.com.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ju.asd995.cn

[J05] 时间加减（加 7 天）
来源：http://sc.chemitech.net.cn

Py:   now + timedelta(days=7)
来源：http://qx.jianghongdianzi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pb.hahajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mu.lnxyls.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lh.shtwfgs.cn

Java: LocalDate.now().plusDays(7)
来源：http://bh.szxytkj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hy.jctech888.com.cn

Ruby: Time.now + 7 * 86400
来源：http://fl.9csxet.cn

C#:   DateTime.Now.AddDays(7)
来源：http://cu.huixinmuqiang.cn

[J06] 计算两时间之差
来源：http://sc.chemitech.net.cn

Py:   (end - start).total_seconds()
来源：http://db.nicolike.cn

PHP:  $end->diff($start)->days;
来源：http://br.huixiangedu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vz.521024.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ye.hnjuh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ou.newstarts.cn

Go:   end.Sub(start).Hours()
来源：http://sr.newstarts.cn

Ruby: end - start                 # 返回秒数
来源：http://tk.9csxet.cn

C#:   (end - start).TotalSeconds
来源：http://gb.colortex.cn

[J07] 比较两个日期
来源：http://yh.newstarts.cn

Py:   d1 < d2;  d1 == d2
来源：http://aq.nszjky.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sp.521024.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zd.szxytkj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gi.haigaiapp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cm.szxytkj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tf.huanxung.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zb.szxytkj.cn

C#:   d1 < d2;  d1 == d2
来源：http://yv.hnjuh.cn

[J08] 提取年月日与星期
来源：http://rx.newstarts.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kv.newstarts.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qc.521024.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://du.9csxet.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dv.huixiangedu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wf.huixiangedu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sd.chemitech.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://la.9csxet.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rf.huixinmuqiang.cn

[J09] 时区处理
来源：http://na.wgjwhj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wa.521024.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pa.gzmigu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ro.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jq.nicolike.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vm.szsharing.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ju.shtwfgs.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://no.huixiangedu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ex.lnxyls.cn

[J10] 取今天 / 本月第一天
来源：http://um.newstarts.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://do.nszjky.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zl.wgjwhj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tr.nszjky.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rq.hahajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lf.bjjhwx.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hv.hahajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gw.9csxet.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tw.lnxyls.cn

================================================================================
来源：http://wm.shxzukj.cn

K. JSON 与序列化
来源：http://hg.chemitech.net.cn

================================================================================
来源：http://kj.nszjky.cn

[K01] 对象转 JSON 字符串
来源：http://kk.hahajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rs.panjiajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mx.wgjwhj.cn

JS:   JSON.stringify(obj)
来源：http://hl.shtwfgs.cn

TS:   JSON.stringify(obj)
来源：http://xh.hnjuh.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gv.colortex.cn

Go:   json.Marshal(obj)
来源：http://yt.haigaiapp.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dz.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://df.shtwfgs.cn

[K02] JSON 字符串转对象
来源：http://kj.bookmarksfly.cn

Py:   json.loads(s)
来源：http://kg.hahajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yg.huixiangedu.cn

JS:   JSON.parse(s)
来源：http://va.bookmarksfly.cn

TS:   JSON.parse(s)
来源：http://vp.asd995.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gi.haigaiapp.cn

Go:   json.Unmarshal(data, &v)
来源：http://ei.chemitech.net.cn

Ruby: JSON.parse(s)
来源：http://jb.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fz.gzmigu.cn

[K03] JSON 美化输出（带缩进）
来源：http://bf.nicolike.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lz.newstarts.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kv.shxzukj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://or.chemitech.net.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vi.haigaiapp.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://da.gzmigu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ej.wgjwhj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wy.szsharing.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fj.huixinmuqiang.cn

[K04] 读取 JSON 文件
来源：http://zd.huixiangedu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ut.colortex.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wr.newstarts.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vu.asd995.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lb.jianghongdianzi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yd.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hk.yuntaijiaju.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ud.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://up.yuexingan06.cn

[K05] 深拷贝对象
来源：http://dg.huanxung.cn

Py:   copy.deepcopy(obj)
来源：http://vx.haigaiapp.cn

PHP:  unserialize(serialize($obj));
来源：http://gt.521024.cn

JS:   structuredClone(obj)
来源：http://og.colortex.cn

TS:   structuredClone(obj)
来源：http://ya.shxzukj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fs.jianghongdianzi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ae.shtwfgs.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ev.bjjhwx.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://jf.jianghongdianzi.cn

[K06] 解析 URL 查询串
来源：http://pc.colortex.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bg.muxihuayi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gi.yuexingan06.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ky.shxzskj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://em.muxihuayi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://co.colortex.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gn.bookmarksfly.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ki.huanxung.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bf.chemitech.net.cn

[K07] 进制转换
来源：http://wg.yuntaijiaju.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bo.nicolike.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kz.yuntaijiaju.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xz.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ym.shtwfgs.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ej.hnjuh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fx.hahajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yu.haigaiapp.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://co.wgjwhj.cn

[K08] 二进制序列化（非 JSON）
来源：http://qe.yuexingan06.cn

Py:   pickle.dumps(obj)
来源：http://mo.jctech888.com.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dj.shxzukj.cn

JS:   v8.serialize(obj)        // Node
来源：http://be.shxzukj.cn

TS:   v8.serialize(obj)        // Node
来源：http://tb.haigaiapp.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yf.521024.cn

Go:   encoding/gob
来源：http://jc.jianghongdianzi.cn

Ruby: Marshal.dump(obj)
来源：http://dd.jctech888.com.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fb.9csxet.cn

================================================================================
来源：http://po.bookmarksfly.cn

L. 网络请求
来源：http://hq.521024.cn

================================================================================
来源：http://zz.shxzukj.cn

[L01] 发送 GET 请求
来源：http://xi.bjjhwx.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zc.nicolike.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rx.chemitech.net.cn

JS:   await fetch(url)
来源：http://ac.muxihuayi.cn

TS:   await fetch(url)
来源：http://vv.lnxyls.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fd.huanxung.cn

Go:   resp, err := http.Get(url)
来源：http://pb.chemitech.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bq.huixinmuqiang.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bk.muxihuayi.cn

[L02] 发送 POST JSON
来源：http://vd.jianghongdianzi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mj.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lc.jianghongdianzi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ed.yuntaijiaju.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nj.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qe.lnxyls.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://by.jianghongdianzi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ya.jianghongdianzi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gm.nicolike.cn

[L03] 设置自定义请求头
来源：http://hd.newstarts.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xp.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dz.jianghongdianzi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ry.newstarts.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xq.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lj.huanxung.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ae.chemitech.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vz.hahajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://oc.szxytkj.cn

[L04] 设置超时
来源：http://oy.jianghongdianzi.cn

Py:   requests.get(url, timeout=5)
来源：http://sn.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xj.szsharing.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yo.shtwfgs.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qo.521024.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wt.yuexingan06.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ap.bjjhwx.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tx.gzmigu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ml.bookmarksfly.cn

[L05] 上传文件（multipart）
来源：http://zt.asd995.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fm.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qd.lnxyls.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qk.hahajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sr.jctech888.com.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gw.shtwfgs.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tp.9csxet.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xq.nicolike.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xr.newstarts.cn

[L06] 解析响应为 JSON
来源：http://ou.jianghongdianzi.cn

Py:   resp.json()
来源：http://xx.nicolike.cn

PHP:  json_decode($body, true);
来源：http://sx.huixinmuqiang.cn

JS:   await resp.json()
来源：http://no.colortex.cn

TS:   await resp.json()
来源：http://wg.colortex.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ih.hahajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lf.newstarts.cn

Ruby: JSON.parse(resp.body)
来源：http://mi.hnjuh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://oz.haigaiapp.cn

[L07] 处理 HTTP 状态码
来源：http://hf.yuntaijiaju.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fp.gzmigu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xe.muxihuayi.cn

JS:   resp.ok;  resp.status
来源：http://ef.bjjhwx.cn

TS:   resp.ok;  resp.status
来源：http://li.bookmarksfly.cn

Java: resp.statusCode()
来源：http://iq.yuntaijiaju.cn

Go:   resp.StatusCode
来源：http://na.hahajie.cn

Ruby: resp.code.to_i
来源：http://sg.bookmarksfly.cn

C#:   (int)resp.StatusCode
来源：http://dv.jianghongdianzi.cn

[L08] 并发请求多个地址
来源：http://qh.newstarts.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fv.lnxyls.cn

PHP:  curl_multi_init() 系列
来源：http://vs.panjiajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pv.jctech888.com.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://en.jianghongdianzi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fd.9csxet.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://is.szxytkj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zw.colortex.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vu.hahajie.cn

================================================================================
来源：http://ss.lnxyls.cn

M. 命令行 / 进程 / 环境
来源：http://pj.shxzskj.cn

================================================================================
来源：http://ar.szsharing.cn

[M01] 读取命令行参数
来源：http://ne.huixiangedu.cn

Py:   sys.argv[1:]
来源：http://jt.szsharing.cn

PHP:  $argv;  $argc;
来源：http://ez.gzmigu.cn

JS:   process.argv.slice(2)
来源：http://ju.shxzukj.cn

TS:   process.argv.slice(2)
来源：http://xv.hahajie.cn

Java: args 数组（main 方法参数）
来源：http://pe.shtwfgs.cn

Go:   os.Args[1:]
来源：http://ib.jctech888.com.cn

Ruby: ARGV
来源：http://cv.huanxung.cn

C#:   args 数组（Main 方法参数）
来源：http://fa.szxytkj.cn

[M02] 读取环境变量
来源：http://bj.shxzukj.cn

Py:   os.environ.get("HOME")
来源：http://sr.wgjwhj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zq.yuexingan06.cn

JS:   process.env.HOME
来源：http://mt.szsharing.cn

TS:   process.env.HOME
来源：http://qr.chemitech.net.cn

Java: System.getenv("HOME")
来源：http://xg.wgjwhj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jx.hahajie.cn

Ruby: ENV["HOME"]
来源：http://gt.shtwfgs.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qs.szxytkj.cn

[M03] 执行外部命令
来源：http://vl.lnxyls.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mn.huixinmuqiang.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xo.szsharing.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kk.shtwfgs.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pf.yuntaijiaju.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nm.chemitech.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vc.newstarts.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ep.asd995.cn

C#:   Process.Start("ls", "-l");
来源：http://rc.newstarts.cn

[M04] 获取当前工作目录
来源：http://te.bookmarksfly.cn

Py:   os.getcwd()
来源：http://fy.lnxyls.cn

PHP:  getcwd();
来源：http://yl.muxihuayi.cn

JS:   process.cwd()
来源：http://zd.wgjwhj.cn

TS:   process.cwd()
来源：http://nm.gzmigu.cn

Java: Path.of("").toAbsolutePath()
来源：http://vc.shxzukj.cn

Go:   os.Getwd()
来源：http://kq.bjjhwx.cn

Ruby: Dir.pwd
来源：http://lt.huixinmuqiang.cn

C#:   Directory.GetCurrentDirectory()
来源：http://uo.colortex.cn

[M05] 设置退出码
来源：http://nm.521024.cn

Py:   sys.exit(1)
来源：http://mb.hahajie.cn

PHP:  exit(1);
来源：http://sq.haigaiapp.cn

JS:   process.exit(1)
来源：http://jz.huanxung.cn

TS:   process.exit(1)
来源：http://vv.nszjky.cn

Java: System.exit(1)
来源：http://nt.asd995.cn

Go:   os.Exit(1)
来源：http://of.huanxung.cn

Ruby: exit 1
来源：http://nu.521024.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fi.colortex.cn

[M06] 向标准错误输出
来源：http://ej.nicolike.cn

Py:   print("err", file=sys.stderr)
来源：http://is.hnjuh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://zt.jianghongdianzi.cn

JS:   console.error("err")
来源：http://kb.nicolike.cn

TS:   console.error("err")
来源：http://ku.newstarts.cn

Java: System.err.println("err")
来源：http://rb.muxihuayi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ci.asd995.cn

Ruby: warn "err"
来源：http://hd.521024.cn

C#:   Console.Error.WriteLine("err")
来源：http://ja.nszjky.cn

[M07] 判断是否为主入口
来源：http://jf.hnjuh.cn


<!-- 参考信息 -->