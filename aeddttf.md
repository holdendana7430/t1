代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fy.hahajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://us.wgjwhj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nq.colortex.cn

TS:   d.toISOString()
来源：http://dn.panjiajie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dc.gzmigu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ja.shxzskj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mz.gzmigu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://go.yuexingan06.cn

[J03] 字符串解析为日期
来源：http://yq.shxzukj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fp.shtwfgs.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://eb.muxihuayi.cn

JS:   new Date("2024-01-02")
来源：http://wa.yuexingan06.cn

TS:   new Date("2024-01-02")
来源：http://fz.shxzukj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wr.muxihuayi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ki.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://nn.haigaiapp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lb.jianghongdianzi.cn

[J04] 时间戳与日期互转
来源：http://mi.newstarts.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gd.huixiangedu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kn.lnxyls.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://id.newstarts.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ft.jctech888.com.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qp.panjiajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ru.huixinmuqiang.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bd.bookmarksfly.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cg.hnjuh.cn

[J05] 时间加减（加 7 天）
来源：http://ji.9csxet.cn

Py:   now + timedelta(days=7)
来源：http://ti.521024.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xo.jctech888.com.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pu.9csxet.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://py.gzmigu.cn

Java: LocalDate.now().plusDays(7)
来源：http://jv.szxytkj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ii.muxihuayi.cn

Ruby: Time.now + 7 * 86400
来源：http://xo.nszjky.cn

C#:   DateTime.Now.AddDays(7)
来源：http://da.szsharing.cn

[J06] 计算两时间之差
来源：http://hj.nicolike.cn

Py:   (end - start).total_seconds()
来源：http://cr.huixinmuqiang.cn

PHP:  $end->diff($start)->days;
来源：http://qh.521024.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ca.nszjky.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gw.colortex.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xk.haigaiapp.cn

Go:   end.Sub(start).Hours()
来源：http://bo.gzmigu.cn

Ruby: end - start                 # 返回秒数
来源：http://cv.nicolike.cn

C#:   (end - start).TotalSeconds
来源：http://qb.yuexingan06.cn

[J07] 比较两个日期
来源：http://ce.hahajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://di.nszjky.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vb.szxytkj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xd.colortex.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qf.huanxung.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ms.jianghongdianzi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ig.szsharing.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pc.newstarts.cn

C#:   d1 < d2;  d1 == d2
来源：http://go.yuexingan06.cn

[J08] 提取年月日与星期
来源：http://ea.colortex.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tn.wgjwhj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xe.newstarts.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ke.nszjky.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://my.wgjwhj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rf.yuntaijiaju.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gs.nszjky.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tv.panjiajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ls.9csxet.cn

[J09] 时区处理
来源：http://zs.szxytkj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ts.yuexingan06.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://db.huixiangedu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xq.colortex.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uz.nicolike.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ym.521024.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tj.chemitech.net.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ph.yuexingan06.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yg.chemitech.net.cn

[J10] 取今天 / 本月第一天
来源：http://hp.521024.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rg.shxzukj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xj.9csxet.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gz.shxzskj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kf.hahajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://aa.lnxyls.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bv.9csxet.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bw.szxytkj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://om.jianghongdianzi.cn

================================================================================
来源：http://cv.huixiangedu.cn

K. JSON 与序列化
来源：http://ma.haigaiapp.cn

================================================================================
来源：http://ur.colortex.cn

[K01] 对象转 JSON 字符串
来源：http://sg.huanxung.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dj.nicolike.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cp.muxihuayi.cn

JS:   JSON.stringify(obj)
来源：http://ha.nszjky.cn

TS:   JSON.stringify(obj)
来源：http://lm.haigaiapp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uc.nicolike.cn

Go:   json.Marshal(obj)
来源：http://sa.yuexingan06.cn

Ruby: obj.to_json                                     // require "json"
来源：http://kj.nszjky.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jm.nicolike.cn

[K02] JSON 字符串转对象
来源：http://nv.yuntaijiaju.cn

Py:   json.loads(s)
来源：http://ck.hahajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ri.colortex.cn

JS:   JSON.parse(s)
来源：http://sz.bjjhwx.cn

TS:   JSON.parse(s)
来源：http://dc.hnjuh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ds.lnxyls.cn

Go:   json.Unmarshal(data, &v)
来源：http://nb.nicolike.cn

Ruby: JSON.parse(s)
来源：http://ov.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://aa.hahajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://wv.hahajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ep.shxzskj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jm.shxzukj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bi.nicolike.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ng.panjiajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://je.haigaiapp.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jx.shtwfgs.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hy.lnxyls.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qc.nicolike.cn

[K04] 读取 JSON 文件
来源：http://sk.9csxet.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ds.colortex.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ff.nicolike.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ft.panjiajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lc.yuntaijiaju.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ed.szxytkj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ez.521024.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wi.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xo.hnjuh.cn

[K05] 深拷贝对象
来源：http://uc.hnjuh.cn

Py:   copy.deepcopy(obj)
来源：http://og.lnxyls.cn

PHP:  unserialize(serialize($obj));
来源：http://df.gzmigu.cn

JS:   structuredClone(obj)
来源：http://pp.gzmigu.cn

TS:   structuredClone(obj)
来源：http://an.nicolike.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://lr.yuexingan06.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kh.bjjhwx.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sj.nszjky.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tg.shxzukj.cn

[K06] 解析 URL 查询串
来源：http://wt.hnjuh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xi.hahajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nc.lnxyls.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qh.hahajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yj.jctech888.com.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://na.huixiangedu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://yg.chemitech.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mb.huixiangedu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://od.muxihuayi.cn

[K07] 进制转换
来源：http://fw.hnjuh.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rb.9csxet.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pl.nszjky.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vw.huanxung.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ji.nszjky.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ml.shxzukj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dt.chemitech.net.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ct.shxzukj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yr.9csxet.cn

[K08] 二进制序列化（非 JSON）
来源：http://hw.jianghongdianzi.cn

Py:   pickle.dumps(obj)
来源：http://tv.hahajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cf.hnjuh.cn

JS:   v8.serialize(obj)        // Node
来源：http://sl.shtwfgs.cn

TS:   v8.serialize(obj)        // Node
来源：http://gz.huixiangedu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gn.hahajie.cn

Go:   encoding/gob
来源：http://ck.lnxyls.cn

Ruby: Marshal.dump(obj)
来源：http://rs.newstarts.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bm.chemitech.net.cn

================================================================================
来源：http://af.yuexingan06.cn

L. 网络请求
来源：http://wm.szsharing.cn

================================================================================
来源：http://eq.bjjhwx.cn

[L01] 发送 GET 请求
来源：http://ku.nicolike.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zm.jianghongdianzi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nm.szxytkj.cn

JS:   await fetch(url)
来源：http://ru.jianghongdianzi.cn

TS:   await fetch(url)
来源：http://ge.bookmarksfly.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ae.521024.cn

Go:   resp, err := http.Get(url)
来源：http://ee.szsharing.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://sc.hahajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nj.nszjky.cn

[L02] 发送 POST JSON
来源：http://id.shtwfgs.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fn.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bx.hnjuh.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yy.haigaiapp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xa.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hc.lnxyls.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zk.hnjuh.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fs.szsharing.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://re.wgjwhj.cn

[L03] 设置自定义请求头
来源：http://ad.yuntaijiaju.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://de.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://md.gzmigu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bz.haigaiapp.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xc.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sr.lnxyls.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://am.bookmarksfly.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://id.bookmarksfly.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xn.9csxet.cn

[L04] 设置超时
来源：http://mj.wgjwhj.cn

Py:   requests.get(url, timeout=5)
来源：http://ww.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bb.muxihuayi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hj.asd995.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uh.asd995.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ra.asd995.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fp.newstarts.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rf.muxihuayi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ad.huixinmuqiang.cn

[L05] 上传文件（multipart）
来源：http://sk.huanxung.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kj.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ix.shxzukj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lm.muxihuayi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hq.9csxet.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tg.hnjuh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://td.jctech888.com.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ga.shtwfgs.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ku.521024.cn

[L06] 解析响应为 JSON
来源：http://ne.colortex.cn

Py:   resp.json()
来源：http://ws.colortex.cn

PHP:  json_decode($body, true);
来源：http://ra.colortex.cn

JS:   await resp.json()
来源：http://mm.szxytkj.cn

TS:   await resp.json()
来源：http://is.9csxet.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jk.szxytkj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://sm.yuntaijiaju.cn

Ruby: JSON.parse(resp.body)
来源：http://ww.wgjwhj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://se.yuntaijiaju.cn

[L07] 处理 HTTP 状态码
来源：http://vc.newstarts.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://co.yuexingan06.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uh.wgjwhj.cn

JS:   resp.ok;  resp.status
来源：http://pq.yuexingan06.cn

TS:   resp.ok;  resp.status
来源：http://kl.szxytkj.cn

Java: resp.statusCode()
来源：http://qv.hahajie.cn

Go:   resp.StatusCode
来源：http://sa.nszjky.cn

Ruby: resp.code.to_i
来源：http://sj.shtwfgs.cn

C#:   (int)resp.StatusCode
来源：http://ru.huixinmuqiang.cn

[L08] 并发请求多个地址
来源：http://ne.hnjuh.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yj.muxihuayi.cn

PHP:  curl_multi_init() 系列
来源：http://xq.asd995.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sy.haigaiapp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xl.szsharing.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://at.huanxung.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hn.muxihuayi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lo.bookmarksfly.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://li.bjjhwx.cn

================================================================================
来源：http://vp.yuntaijiaju.cn

M. 命令行 / 进程 / 环境
来源：http://nc.521024.cn

================================================================================
来源：http://tu.wgjwhj.cn

[M01] 读取命令行参数
来源：http://gq.jctech888.com.cn

Py:   sys.argv[1:]
来源：http://hn.jctech888.com.cn

PHP:  $argv;  $argc;
来源：http://pv.colortex.cn

JS:   process.argv.slice(2)
来源：http://xo.9csxet.cn

TS:   process.argv.slice(2)
来源：http://vf.jctech888.com.cn

Java: args 数组（main 方法参数）
来源：http://vi.haigaiapp.cn

Go:   os.Args[1:]
来源：http://rh.huixinmuqiang.cn

Ruby: ARGV
来源：http://ip.newstarts.cn

C#:   args 数组（Main 方法参数）
来源：http://zv.521024.cn

[M02] 读取环境变量
来源：http://pp.haigaiapp.cn

Py:   os.environ.get("HOME")
来源：http://va.bjjhwx.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://av.panjiajie.cn

JS:   process.env.HOME
来源：http://xk.nszjky.cn

TS:   process.env.HOME
来源：http://lm.wgjwhj.cn

Java: System.getenv("HOME")
来源：http://cd.huixinmuqiang.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nl.bjjhwx.cn

Ruby: ENV["HOME"]
来源：http://jn.hahajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xf.yuntaijiaju.cn

[M03] 执行外部命令
来源：http://ko.521024.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mm.9csxet.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ml.shxzskj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ur.wgjwhj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://iv.shxzukj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vo.szsharing.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://sh.hahajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zk.bjjhwx.cn

C#:   Process.Start("ls", "-l");
来源：http://im.newstarts.cn

[M04] 获取当前工作目录
来源：http://xe.bookmarksfly.cn

Py:   os.getcwd()
来源：http://av.haigaiapp.cn

PHP:  getcwd();
来源：http://er.wgjwhj.cn

JS:   process.cwd()
来源：http://bu.huanxung.cn

TS:   process.cwd()
来源：http://zu.shxzskj.cn

Java: Path.of("").toAbsolutePath()
来源：http://ar.muxihuayi.cn

Go:   os.Getwd()
来源：http://vc.shxzukj.cn

Ruby: Dir.pwd
来源：http://pe.shxzskj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://tf.shxzskj.cn

[M05] 设置退出码
来源：http://dh.bookmarksfly.cn

Py:   sys.exit(1)
来源：http://ez.hahajie.cn

PHP:  exit(1);
来源：http://kq.newstarts.cn

JS:   process.exit(1)
来源：http://mf.szxytkj.cn

TS:   process.exit(1)
来源：http://sx.asd995.cn

Java: System.exit(1)
来源：http://wo.haigaiapp.cn

Go:   os.Exit(1)
来源：http://cy.wgjwhj.cn

Ruby: exit 1
来源：http://ia.hahajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ek.bjjhwx.cn

[M06] 向标准错误输出
来源：http://om.bjjhwx.cn

Py:   print("err", file=sys.stderr)
来源：http://ta.bjjhwx.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ow.huanxung.cn

JS:   console.error("err")
来源：http://cv.muxihuayi.cn

TS:   console.error("err")
来源：http://fb.muxihuayi.cn

Java: System.err.println("err")
来源：http://lp.nszjky.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://eu.chemitech.net.cn

Ruby: warn "err"
来源：http://ib.colortex.cn

C#:   Console.Error.WriteLine("err")
来源：http://rp.nicolike.cn

[M07] 判断是否为主入口
来源：http://mn.hahajie.cn

Py:   if __name__ == "__main__":
来源：http://nu.huixinmuqiang.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xo.shtwfgs.cn

JS:   require.main === module
来源：http://gm.shxzskj.cn

TS:   require.main === module
来源：http://gs.asd995.cn

Java: public static void main(String[] args)
来源：http://fk.huixinmuqiang.cn

Go:   func main()
来源：http://ud.muxihuayi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jy.shtwfgs.cn

C#:   static void Main(string[] args)
来源：http://uo.huanxung.cn

[M08] 获取系统与运行时信息
来源：http://yu.yuntaijiaju.cn

Py:   platform.system();  platform.python_version()
来源：http://re.newstarts.cn

PHP:  PHP_OS;  phpversion();
来源：http://pf.bookmarksfly.cn

JS:   process.platform;  process.version
来源：http://xd.nicolike.cn


<!-- 参考信息 -->