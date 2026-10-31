代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://un.huixiangedu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bs.yuexingan06.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rq.asd995.cn

TS:   d.toISOString()
来源：http://oa.huixiangedu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sc.jctech888.com.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ps.szsharing.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sm.yuexingan06.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://in.yuntaijiaju.cn

[J03] 字符串解析为日期
来源：http://ku.haigaiapp.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cu.newstarts.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rm.newstarts.cn

JS:   new Date("2024-01-02")
来源：http://iu.bjjhwx.cn

TS:   new Date("2024-01-02")
来源：http://fu.colortex.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jj.jianghongdianzi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sp.wgjwhj.cn

Ruby: Date.parse("2024-01-02")
来源：http://je.hahajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cz.jianghongdianzi.cn

[J04] 时间戳与日期互转
来源：http://hh.lnxyls.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://an.chemitech.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mv.shxzskj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cj.gzmigu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qw.huanxung.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ep.jctech888.com.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://va.521024.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://br.wgjwhj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gh.nszjky.cn

[J05] 时间加减（加 7 天）
来源：http://hc.huixiangedu.cn

Py:   now + timedelta(days=7)
来源：http://yf.shxzukj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://fr.lnxyls.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gf.shtwfgs.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gc.nicolike.cn

Java: LocalDate.now().plusDays(7)
来源：http://fa.521024.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sv.nicolike.cn

Ruby: Time.now + 7 * 86400
来源：http://be.newstarts.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ww.szxytkj.cn

[J06] 计算两时间之差
来源：http://cn.wgjwhj.cn

Py:   (end - start).total_seconds()
来源：http://vu.huanxung.cn

PHP:  $end->diff($start)->days;
来源：http://dn.shtwfgs.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ug.haigaiapp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://oy.nszjky.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hb.yuexingan06.cn

Go:   end.Sub(start).Hours()
来源：http://be.huixinmuqiang.cn

Ruby: end - start                 # 返回秒数
来源：http://eq.szxytkj.cn

C#:   (end - start).TotalSeconds
来源：http://mx.huixinmuqiang.cn

[J07] 比较两个日期
来源：http://gr.shtwfgs.cn

Py:   d1 < d2;  d1 == d2
来源：http://st.hnjuh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ww.lnxyls.cn

JS:   d1.getTime() < d2.getTime()
来源：http://an.9csxet.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ir.yuntaijiaju.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mq.yuntaijiaju.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vb.huixinmuqiang.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ts.gzmigu.cn

C#:   d1 < d2;  d1 == d2
来源：http://uv.shxzskj.cn

[J08] 提取年月日与星期
来源：http://qg.szxytkj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sa.szxytkj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oi.newstarts.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dt.521024.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://od.yuexingan06.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://er.huanxung.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vg.szxytkj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tr.hahajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://te.wgjwhj.cn

[J09] 时区处理
来源：http://hs.jctech888.com.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qh.szsharing.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lw.shxzukj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://df.huanxung.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sp.huixiangedu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fw.9csxet.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jv.colortex.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jg.chemitech.net.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zo.huanxung.cn

[J10] 取今天 / 本月第一天
来源：http://bh.nszjky.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xf.shxzukj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ue.newstarts.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bs.jianghongdianzi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ds.szxytkj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://po.newstarts.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://oz.asd995.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://la.521024.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qu.colortex.cn

================================================================================
来源：http://fi.521024.cn

K. JSON 与序列化
来源：http://un.muxihuayi.cn

================================================================================
来源：http://lt.wgjwhj.cn

[K01] 对象转 JSON 字符串
来源：http://mj.newstarts.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ig.521024.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gn.haigaiapp.cn

JS:   JSON.stringify(obj)
来源：http://fs.muxihuayi.cn

TS:   JSON.stringify(obj)
来源：http://tg.nszjky.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nz.9csxet.cn

Go:   json.Marshal(obj)
来源：http://zu.jctech888.com.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ez.panjiajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yc.asd995.cn

[K02] JSON 字符串转对象
来源：http://sg.bjjhwx.cn

Py:   json.loads(s)
来源：http://cj.shtwfgs.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tf.chemitech.net.cn

JS:   JSON.parse(s)
来源：http://qs.chemitech.net.cn

TS:   JSON.parse(s)
来源：http://qs.asd995.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cn.bjjhwx.cn

Go:   json.Unmarshal(data, &v)
来源：http://ld.jctech888.com.cn

Ruby: JSON.parse(s)
来源：http://oz.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ob.521024.cn

[K03] JSON 美化输出（带缩进）
来源：http://vr.9csxet.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uc.hahajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wd.chemitech.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zg.newstarts.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fd.9csxet.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wa.nszjky.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://td.nicolike.cn

Ruby: JSON.pretty_generate(obj)
来源：http://iq.shxzukj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fj.yuntaijiaju.cn

[K04] 读取 JSON 文件
来源：http://bd.hahajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gi.lnxyls.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ou.yuntaijiaju.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://de.shxzskj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://og.nicolike.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cs.521024.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ja.lnxyls.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://it.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pn.hahajie.cn

[K05] 深拷贝对象
来源：http://bm.huixiangedu.cn

Py:   copy.deepcopy(obj)
来源：http://wt.bjjhwx.cn

PHP:  unserialize(serialize($obj));
来源：http://ae.nszjky.cn

JS:   structuredClone(obj)
来源：http://di.lnxyls.cn

TS:   structuredClone(obj)
来源：http://ti.shxzukj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://iu.hahajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tk.panjiajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jy.shtwfgs.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tu.9csxet.cn

[K06] 解析 URL 查询串
来源：http://ei.shxzukj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uo.muxihuayi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bs.haigaiapp.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ml.jianghongdianzi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://la.huixiangedu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://le.shtwfgs.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mj.huixiangedu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bs.chemitech.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vs.521024.cn

[K07] 进制转换
来源：http://wp.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yg.yuexingan06.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ng.asd995.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cn.hnjuh.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tp.bookmarksfly.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vc.chemitech.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pr.yuntaijiaju.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ig.yuntaijiaju.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ar.yuexingan06.cn

[K08] 二进制序列化（非 JSON）
来源：http://pl.9csxet.cn

Py:   pickle.dumps(obj)
来源：http://tr.jctech888.com.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cw.szxytkj.cn

JS:   v8.serialize(obj)        // Node
来源：http://ze.asd995.cn

TS:   v8.serialize(obj)        // Node
来源：http://ut.hnjuh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ep.shxzskj.cn

Go:   encoding/gob
来源：http://zv.huixiangedu.cn

Ruby: Marshal.dump(obj)
来源：http://mt.shxzskj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kq.521024.cn

================================================================================
来源：http://ko.chemitech.net.cn

L. 网络请求
来源：http://ad.panjiajie.cn

================================================================================
来源：http://fr.nicolike.cn

[L01] 发送 GET 请求
来源：http://wn.newstarts.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://as.9csxet.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zo.newstarts.cn

JS:   await fetch(url)
来源：http://pn.521024.cn

TS:   await fetch(url)
来源：http://jv.gzmigu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lt.9csxet.cn

Go:   resp, err := http.Get(url)
来源：http://dc.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://nv.yuntaijiaju.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jd.panjiajie.cn

[L02] 发送 POST JSON
来源：http://zc.jianghongdianzi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://tk.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ko.hahajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://me.colortex.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kt.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ht.muxihuayi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://eh.gzmigu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bj.huixinmuqiang.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://og.nicolike.cn

[L03] 设置自定义请求头
来源：http://hk.chemitech.net.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bx.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qu.hnjuh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zb.chemitech.net.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dl.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cq.muxihuayi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uj.shtwfgs.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fy.szxytkj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lr.nszjky.cn

[L04] 设置超时
来源：http://lr.nicolike.cn

Py:   requests.get(url, timeout=5)
来源：http://th.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ss.nicolike.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jd.szxytkj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wx.yuexingan06.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ga.lnxyls.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://my.bookmarksfly.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://od.gzmigu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hx.yuntaijiaju.cn

[L05] 上传文件（multipart）
来源：http://dl.nicolike.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vd.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://oi.newstarts.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ku.hahajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gt.hahajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zz.hahajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lh.lnxyls.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tq.lnxyls.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bm.huanxung.cn

[L06] 解析响应为 JSON
来源：http://nd.shtwfgs.cn

Py:   resp.json()
来源：http://ff.huixiangedu.cn

PHP:  json_decode($body, true);
来源：http://gd.asd995.cn

JS:   await resp.json()
来源：http://ld.newstarts.cn

TS:   await resp.json()
来源：http://mz.chemitech.net.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mg.asd995.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vd.hnjuh.cn

Ruby: JSON.parse(resp.body)
来源：http://vd.9csxet.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qm.chemitech.net.cn

[L07] 处理 HTTP 状态码
来源：http://id.huixinmuqiang.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dj.huixiangedu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bx.haigaiapp.cn

JS:   resp.ok;  resp.status
来源：http://pu.panjiajie.cn

TS:   resp.ok;  resp.status
来源：http://fl.newstarts.cn

Java: resp.statusCode()
来源：http://rc.colortex.cn

Go:   resp.StatusCode
来源：http://ni.nicolike.cn

Ruby: resp.code.to_i
来源：http://bu.bookmarksfly.cn

C#:   (int)resp.StatusCode
来源：http://ic.szsharing.cn

[L08] 并发请求多个地址
来源：http://js.jianghongdianzi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jf.521024.cn

PHP:  curl_multi_init() 系列
来源：http://mq.panjiajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ir.9csxet.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tj.521024.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lt.hnjuh.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ek.szxytkj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uc.newstarts.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://eo.hahajie.cn

================================================================================
来源：http://ji.newstarts.cn

M. 命令行 / 进程 / 环境
来源：http://qu.shxzukj.cn

================================================================================
来源：http://ph.yuntaijiaju.cn

[M01] 读取命令行参数
来源：http://lf.newstarts.cn

Py:   sys.argv[1:]
来源：http://sd.bjjhwx.cn

PHP:  $argv;  $argc;
来源：http://mb.shtwfgs.cn

JS:   process.argv.slice(2)
来源：http://vd.hahajie.cn

TS:   process.argv.slice(2)
来源：http://qy.yuexingan06.cn

Java: args 数组（main 方法参数）
来源：http://cq.nicolike.cn

Go:   os.Args[1:]
来源：http://fv.haigaiapp.cn

Ruby: ARGV
来源：http://dw.newstarts.cn

C#:   args 数组（Main 方法参数）
来源：http://xf.yuntaijiaju.cn

[M02] 读取环境变量
来源：http://mq.wgjwhj.cn

Py:   os.environ.get("HOME")
来源：http://dl.yuexingan06.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tp.shxzukj.cn

JS:   process.env.HOME
来源：http://wi.9csxet.cn

TS:   process.env.HOME
来源：http://xm.shtwfgs.cn

Java: System.getenv("HOME")
来源：http://hc.wgjwhj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://aq.yuexingan06.cn

Ruby: ENV["HOME"]
来源：http://po.yuexingan06.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bl.shxzukj.cn

[M03] 执行外部命令
来源：http://yq.yuexingan06.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bt.shtwfgs.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kt.asd995.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://is.huixiangedu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vi.shxzukj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://va.nicolike.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wm.yuexingan06.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ee.lnxyls.cn

C#:   Process.Start("ls", "-l");
来源：http://wr.shxzskj.cn

[M04] 获取当前工作目录
来源：http://ow.shtwfgs.cn

Py:   os.getcwd()
来源：http://ie.chemitech.net.cn

PHP:  getcwd();
来源：http://od.bookmarksfly.cn

JS:   process.cwd()
来源：http://bc.newstarts.cn

TS:   process.cwd()
来源：http://ro.shxzskj.cn

Java: Path.of("").toAbsolutePath()
来源：http://dq.asd995.cn

Go:   os.Getwd()
来源：http://vv.haigaiapp.cn

Ruby: Dir.pwd
来源：http://sz.huixiangedu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rq.szsharing.cn

[M05] 设置退出码
来源：http://px.yuntaijiaju.cn

Py:   sys.exit(1)
来源：http://gp.panjiajie.cn

PHP:  exit(1);
来源：http://ir.lnxyls.cn

JS:   process.exit(1)
来源：http://sj.shxzukj.cn

TS:   process.exit(1)
来源：http://wt.shxzukj.cn

Java: System.exit(1)
来源：http://fk.yuntaijiaju.cn

Go:   os.Exit(1)
来源：http://ut.szxytkj.cn

Ruby: exit 1
来源：http://fi.newstarts.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ep.521024.cn

[M06] 向标准错误输出
来源：http://bo.bjjhwx.cn

Py:   print("err", file=sys.stderr)
来源：http://gn.muxihuayi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://uc.bookmarksfly.cn

JS:   console.error("err")
来源：http://ju.colortex.cn

TS:   console.error("err")
来源：http://nu.chemitech.net.cn

Java: System.err.println("err")
来源：http://sz.huixiangedu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yw.yuexingan06.cn

Ruby: warn "err"
来源：http://og.huixiangedu.cn

C#:   Console.Error.WriteLine("err")
来源：http://gj.haigaiapp.cn

[M07] 判断是否为主入口
来源：http://eo.wgjwhj.cn

Py:   if __name__ == "__main__":
来源：http://zh.nszjky.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ai.nicolike.cn

JS:   require.main === module
来源：http://kg.lnxyls.cn

TS:   require.main === module
来源：http://yi.newstarts.cn

Java: public static void main(String[] args)
来源：http://ac.wgjwhj.cn

Go:   func main()
来源：http://eo.panjiajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://go.colortex.cn

C#:   static void Main(string[] args)
来源：http://sm.shxzskj.cn

[M08] 获取系统与运行时信息
来源：http://na.yuexingan06.cn

Py:   platform.system();  platform.python_version()
来源：http://vh.nicolike.cn

PHP:  PHP_OS;  phpversion();
来源：http://mp.yuexingan06.cn

JS:   process.platform;  process.version
来源：http://wg.521024.cn


<!-- 参考信息 -->