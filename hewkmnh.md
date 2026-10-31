代发 wailian999

J. 日期与时间
来源：http://yi.szsharing.cn

================================================================================
来源：http://op.hnjuh.cn

[J01] 获取当前时间
来源：http://tj.newstarts.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qq.newstarts.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fu.huixinmuqiang.cn

JS:   new Date();  Date.now()
来源：http://cl.hnjuh.cn

TS:   new Date();  Date.now()
来源：http://bb.szxytkj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wg.jianghongdianzi.cn

Go:   time.Now()
来源：http://jb.huanxung.cn

Ruby: Time.now
来源：http://wy.shxzskj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ua.jctech888.com.cn

[J02] 格式化输出
来源：http://jc.panjiajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fn.yuntaijiaju.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ez.yuntaijiaju.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bi.shxzskj.cn

TS:   d.toISOString()
来源：http://km.nszjky.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qr.nszjky.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qq.shxzskj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rf.huanxung.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kk.nicolike.cn

[J03] 字符串解析为日期
来源：http://ff.shxzskj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pu.yuexingan06.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zi.jctech888.com.cn

JS:   new Date("2024-01-02")
来源：http://eu.szsharing.cn

TS:   new Date("2024-01-02")
来源：http://pq.hahajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://lz.colortex.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mk.bjjhwx.cn

Ruby: Date.parse("2024-01-02")
来源：http://cv.shxzskj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pm.newstarts.cn

[J04] 时间戳与日期互转
来源：http://dg.huixiangedu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nb.gzmigu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ja.nicolike.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ls.yuntaijiaju.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jd.521024.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dv.newstarts.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cq.hahajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dr.szxytkj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vf.bookmarksfly.cn

[J05] 时间加减（加 7 天）
来源：http://ng.yuexingan06.cn

Py:   now + timedelta(days=7)
来源：http://ea.jctech888.com.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ec.521024.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yk.panjiajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kr.lnxyls.cn

Java: LocalDate.now().plusDays(7)
来源：http://jj.yuntaijiaju.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ml.lnxyls.cn

Ruby: Time.now + 7 * 86400
来源：http://an.szxytkj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zm.hahajie.cn

[J06] 计算两时间之差
来源：http://yi.shxzskj.cn

Py:   (end - start).total_seconds()
来源：http://uo.shtwfgs.cn

PHP:  $end->diff($start)->days;
来源：http://qi.haigaiapp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ss.nszjky.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mf.szsharing.cn

Java: Duration.between(start, end).toSeconds()
来源：http://uj.bookmarksfly.cn

Go:   end.Sub(start).Hours()
来源：http://pf.jctech888.com.cn

Ruby: end - start                 # 返回秒数
来源：http://tr.shxzskj.cn

C#:   (end - start).TotalSeconds
来源：http://ed.hnjuh.cn

[J07] 比较两个日期
来源：http://pb.colortex.cn

Py:   d1 < d2;  d1 == d2
来源：http://cf.huixinmuqiang.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fj.shxzskj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qv.newstarts.cn

TS:   d1.getTime() < d2.getTime()
来源：http://li.shtwfgs.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nv.jctech888.com.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ha.huixinmuqiang.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wz.newstarts.cn

C#:   d1 < d2;  d1 == d2
来源：http://ex.szxytkj.cn

[J08] 提取年月日与星期
来源：http://jf.bookmarksfly.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rc.haigaiapp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://je.chemitech.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ud.szxytkj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oh.asd995.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fi.yuexingan06.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pp.haigaiapp.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://op.bookmarksfly.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://av.muxihuayi.cn

[J09] 时区处理
来源：http://kf.hahajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gj.lnxyls.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pr.szxytkj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sc.lnxyls.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lq.nicolike.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wx.muxihuayi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://eo.szxytkj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gb.jctech888.com.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dc.nicolike.cn

[J10] 取今天 / 本月第一天
来源：http://fb.huanxung.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ro.panjiajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dp.yuntaijiaju.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://on.nicolike.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dn.jianghongdianzi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sv.jianghongdianzi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mg.yuexingan06.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nr.lnxyls.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ox.bjjhwx.cn

================================================================================
来源：http://ni.szsharing.cn

K. JSON 与序列化
来源：http://su.szsharing.cn

================================================================================
来源：http://zt.huanxung.cn

[K01] 对象转 JSON 字符串
来源：http://le.nicolike.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mh.bookmarksfly.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://iu.jianghongdianzi.cn

JS:   JSON.stringify(obj)
来源：http://uj.huanxung.cn

TS:   JSON.stringify(obj)
来源：http://bl.haigaiapp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ev.lnxyls.cn

Go:   json.Marshal(obj)
来源：http://wq.huixiangedu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://yj.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://if.chemitech.net.cn

[K02] JSON 字符串转对象
来源：http://iz.jctech888.com.cn

Py:   json.loads(s)
来源：http://lx.yuexingan06.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://te.9csxet.cn

JS:   JSON.parse(s)
来源：http://zo.521024.cn

TS:   JSON.parse(s)
来源：http://vk.shxzukj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tp.huanxung.cn

Go:   json.Unmarshal(data, &v)
来源：http://vf.shxzskj.cn

Ruby: JSON.parse(s)
来源：http://eq.colortex.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cz.hnjuh.cn

[K03] JSON 美化输出（带缩进）
来源：http://xv.nicolike.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lo.colortex.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ge.jctech888.com.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://su.asd995.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ju.jianghongdianzi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pf.bookmarksfly.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mo.panjiajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qw.panjiajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mv.9csxet.cn

[K04] 读取 JSON 文件
来源：http://rq.shtwfgs.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://po.szsharing.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bk.asd995.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dy.newstarts.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dc.szxytkj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://th.hnjuh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://iq.lnxyls.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ht.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ep.newstarts.cn

[K05] 深拷贝对象
来源：http://dz.szxytkj.cn

Py:   copy.deepcopy(obj)
来源：http://cj.haigaiapp.cn

PHP:  unserialize(serialize($obj));
来源：http://hb.muxihuayi.cn

JS:   structuredClone(obj)
来源：http://lg.bookmarksfly.cn

TS:   structuredClone(obj)
来源：http://qc.yuexingan06.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://we.asd995.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kg.huixinmuqiang.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qw.bjjhwx.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vm.huixinmuqiang.cn

[K06] 解析 URL 查询串
来源：http://gw.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ox.muxihuayi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ti.bookmarksfly.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jy.panjiajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cl.panjiajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fe.yuexingan06.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bz.bjjhwx.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vn.gzmigu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fq.shxzskj.cn

[K07] 进制转换
来源：http://vm.shtwfgs.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://co.newstarts.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ht.szsharing.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qf.shxzukj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qg.wgjwhj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://we.szsharing.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mk.shtwfgs.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://iu.huixiangedu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tz.bjjhwx.cn

[K08] 二进制序列化（非 JSON）
来源：http://mq.huixiangedu.cn

Py:   pickle.dumps(obj)
来源：http://qi.521024.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yr.colortex.cn

JS:   v8.serialize(obj)        // Node
来源：http://jz.gzmigu.cn

TS:   v8.serialize(obj)        // Node
来源：http://os.nszjky.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cv.gzmigu.cn

Go:   encoding/gob
来源：http://pr.gzmigu.cn

Ruby: Marshal.dump(obj)
来源：http://xf.lnxyls.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yz.jianghongdianzi.cn

================================================================================
来源：http://dh.bookmarksfly.cn

L. 网络请求
来源：http://nh.gzmigu.cn

================================================================================
来源：http://do.shxzukj.cn

[L01] 发送 GET 请求
来源：http://se.szxytkj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rm.bookmarksfly.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wg.szsharing.cn

JS:   await fetch(url)
来源：http://bk.szxytkj.cn

TS:   await fetch(url)
来源：http://an.nszjky.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ue.shtwfgs.cn

Go:   resp, err := http.Get(url)
来源：http://qh.szxytkj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://sx.wgjwhj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lw.huanxung.cn

[L02] 发送 POST JSON
来源：http://oa.nszjky.cn

Py:   requests.post(url, json={"a": 1})
来源：http://sr.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pl.szsharing.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xr.521024.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hm.colortex.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tc.gzmigu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yo.bjjhwx.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://us.newstarts.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xp.shxzukj.cn

[L03] 设置自定义请求头
来源：http://kn.muxihuayi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yn.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jz.szxytkj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oa.hahajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rc.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nk.lnxyls.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ep.chemitech.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zx.lnxyls.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ss.gzmigu.cn

[L04] 设置超时
来源：http://vf.panjiajie.cn

Py:   requests.get(url, timeout=5)
来源：http://vz.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fw.wgjwhj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://px.jctech888.com.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kh.bookmarksfly.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xj.jianghongdianzi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rp.szsharing.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qo.szxytkj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sq.muxihuayi.cn

[L05] 上传文件（multipart）
来源：http://ps.nicolike.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ao.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gy.shxzukj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jv.nicolike.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hf.muxihuayi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sv.panjiajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wt.bjjhwx.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tx.panjiajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xi.shxzskj.cn

[L06] 解析响应为 JSON
来源：http://cq.521024.cn

Py:   resp.json()
来源：http://qn.wgjwhj.cn

PHP:  json_decode($body, true);
来源：http://qi.bookmarksfly.cn

JS:   await resp.json()
来源：http://sv.bookmarksfly.cn

TS:   await resp.json()
来源：http://ga.szsharing.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vx.asd995.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zl.hnjuh.cn

Ruby: JSON.parse(resp.body)
来源：http://xx.wgjwhj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ac.huixiangedu.cn

[L07] 处理 HTTP 状态码
来源：http://kj.panjiajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rk.yuntaijiaju.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ue.jianghongdianzi.cn

JS:   resp.ok;  resp.status
来源：http://yu.hnjuh.cn

TS:   resp.ok;  resp.status
来源：http://nj.colortex.cn

Java: resp.statusCode()
来源：http://qf.gzmigu.cn

Go:   resp.StatusCode
来源：http://oe.szxytkj.cn

Ruby: resp.code.to_i
来源：http://oc.huanxung.cn

C#:   (int)resp.StatusCode
来源：http://jp.panjiajie.cn

[L08] 并发请求多个地址
来源：http://rk.hahajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gg.hnjuh.cn

PHP:  curl_multi_init() 系列
来源：http://uu.hnjuh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jr.lnxyls.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://om.panjiajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tb.bjjhwx.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ia.asd995.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zq.hahajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ke.gzmigu.cn

================================================================================
来源：http://uy.chemitech.net.cn

M. 命令行 / 进程 / 环境
来源：http://fb.yuexingan06.cn

================================================================================
来源：http://sj.hnjuh.cn

[M01] 读取命令行参数
来源：http://sb.chemitech.net.cn

Py:   sys.argv[1:]
来源：http://lg.gzmigu.cn

PHP:  $argv;  $argc;
来源：http://ta.szsharing.cn

JS:   process.argv.slice(2)
来源：http://wn.chemitech.net.cn

TS:   process.argv.slice(2)
来源：http://lx.szsharing.cn

Java: args 数组（main 方法参数）
来源：http://hb.lnxyls.cn

Go:   os.Args[1:]
来源：http://kp.muxihuayi.cn

Ruby: ARGV
来源：http://ns.hnjuh.cn

C#:   args 数组（Main 方法参数）
来源：http://se.huixinmuqiang.cn

[M02] 读取环境变量
来源：http://vr.shxzskj.cn

Py:   os.environ.get("HOME")
来源：http://er.wgjwhj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ij.jianghongdianzi.cn

JS:   process.env.HOME
来源：http://xd.hahajie.cn

TS:   process.env.HOME
来源：http://aj.wgjwhj.cn

Java: System.getenv("HOME")
来源：http://rs.haigaiapp.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wa.hahajie.cn

Ruby: ENV["HOME"]
来源：http://vl.shxzukj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gy.wgjwhj.cn

[M03] 执行外部命令
来源：http://hq.bjjhwx.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gj.hahajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rz.huixinmuqiang.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kf.gzmigu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mu.jctech888.com.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ub.bookmarksfly.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mh.muxihuayi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xr.hahajie.cn

C#:   Process.Start("ls", "-l");
来源：http://lu.521024.cn

[M04] 获取当前工作目录
来源：http://po.huixiangedu.cn

Py:   os.getcwd()
来源：http://ud.shxzskj.cn

PHP:  getcwd();
来源：http://qf.lnxyls.cn

JS:   process.cwd()
来源：http://hl.panjiajie.cn

TS:   process.cwd()
来源：http://ta.shtwfgs.cn

Java: Path.of("").toAbsolutePath()
来源：http://sm.jctech888.com.cn

Go:   os.Getwd()
来源：http://sw.yuntaijiaju.cn

Ruby: Dir.pwd
来源：http://vg.szxytkj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ki.chemitech.net.cn

[M05] 设置退出码
来源：http://cb.bjjhwx.cn

Py:   sys.exit(1)
来源：http://iy.huixinmuqiang.cn

PHP:  exit(1);
来源：http://du.huixinmuqiang.cn

JS:   process.exit(1)
来源：http://mn.lnxyls.cn

TS:   process.exit(1)
来源：http://as.newstarts.cn

Java: System.exit(1)
来源：http://aj.hahajie.cn

Go:   os.Exit(1)
来源：http://ax.521024.cn

Ruby: exit 1
来源：http://da.huixiangedu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://br.9csxet.cn

[M06] 向标准错误输出
来源：http://lx.haigaiapp.cn

Py:   print("err", file=sys.stderr)
来源：http://pz.hnjuh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wh.nszjky.cn

JS:   console.error("err")
来源：http://ks.muxihuayi.cn

TS:   console.error("err")
来源：http://bl.szsharing.cn

Java: System.err.println("err")
来源：http://jg.colortex.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wk.yuexingan06.cn

Ruby: warn "err"
来源：http://qf.yuexingan06.cn

C#:   Console.Error.WriteLine("err")
来源：http://vy.521024.cn

[M07] 判断是否为主入口
来源：http://zo.yuexingan06.cn


<!-- 参考信息 -->