代发 wailian999

[J03] 字符串解析为日期
来源：http://um.huanxung.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lu.szsharing.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gv.colortex.cn

JS:   new Date("2024-01-02")
来源：http://xu.yuntaijiaju.cn

TS:   new Date("2024-01-02")
来源：http://bi.wgjwhj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fw.asd995.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zt.shxzukj.cn

Ruby: Date.parse("2024-01-02")
来源：http://lr.haigaiapp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gq.nszjky.cn

[J04] 时间戳与日期互转
来源：http://qb.nszjky.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fk.newstarts.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://oz.huixinmuqiang.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bx.bjjhwx.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bz.huixinmuqiang.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pq.9csxet.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bp.9csxet.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://de.gzmigu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mh.panjiajie.cn

[J05] 时间加减（加 7 天）
来源：http://ab.yuntaijiaju.cn

Py:   now + timedelta(days=7)
来源：http://xq.szsharing.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ql.9csxet.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hq.colortex.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hk.bjjhwx.cn

Java: LocalDate.now().plusDays(7)
来源：http://om.jianghongdianzi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ej.huanxung.cn

Ruby: Time.now + 7 * 86400
来源：http://qy.szxytkj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://nb.asd995.cn

[J06] 计算两时间之差
来源：http://wr.wgjwhj.cn

Py:   (end - start).total_seconds()
来源：http://yc.haigaiapp.cn

PHP:  $end->diff($start)->days;
来源：http://uu.huixiangedu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jv.asd995.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kh.shtwfgs.cn

Java: Duration.between(start, end).toSeconds()
来源：http://na.huixiangedu.cn

Go:   end.Sub(start).Hours()
来源：http://hc.shxzukj.cn

Ruby: end - start                 # 返回秒数
来源：http://ol.haigaiapp.cn

C#:   (end - start).TotalSeconds
来源：http://aq.panjiajie.cn

[J07] 比较两个日期
来源：http://xw.muxihuayi.cn

Py:   d1 < d2;  d1 == d2
来源：http://gc.shxzukj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://co.huixiangedu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kh.panjiajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ys.gzmigu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ps.nicolike.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yi.bookmarksfly.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pl.9csxet.cn

C#:   d1 < d2;  d1 == d2
来源：http://rh.bjjhwx.cn

[J08] 提取年月日与星期
来源：http://fd.nicolike.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://te.huixiangedu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://za.yuntaijiaju.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://my.haigaiapp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oj.chemitech.net.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sv.panjiajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hh.szxytkj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bg.szxytkj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fk.hahajie.cn

[J09] 时区处理
来源：http://mq.huixinmuqiang.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ye.bjjhwx.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ox.szxytkj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cy.9csxet.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ja.muxihuayi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nu.muxihuayi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ch.huixinmuqiang.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://de.huixiangedu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ix.nicolike.cn

[J10] 取今天 / 本月第一天
来源：http://nf.shxzskj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://de.nszjky.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ww.jianghongdianzi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wn.hnjuh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bt.hnjuh.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sg.haigaiapp.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://da.huixiangedu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ad.chemitech.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uu.szxytkj.cn

================================================================================
来源：http://zu.shxzskj.cn

K. JSON 与序列化
来源：http://xx.shxzskj.cn

================================================================================
来源：http://zi.yuexingan06.cn

[K01] 对象转 JSON 字符串
来源：http://eb.bookmarksfly.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hj.szxytkj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ds.chemitech.net.cn

JS:   JSON.stringify(obj)
来源：http://dq.bookmarksfly.cn

TS:   JSON.stringify(obj)
来源：http://nw.bjjhwx.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ew.newstarts.cn

Go:   json.Marshal(obj)
来源：http://th.szsharing.cn

Ruby: obj.to_json                                     // require "json"
来源：http://iz.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qx.huixinmuqiang.cn

[K02] JSON 字符串转对象
来源：http://cs.szsharing.cn

Py:   json.loads(s)
来源：http://pr.shxzukj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wh.huixiangedu.cn

JS:   JSON.parse(s)
来源：http://hv.wgjwhj.cn

TS:   JSON.parse(s)
来源：http://bv.bookmarksfly.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ny.hahajie.cn

Go:   json.Unmarshal(data, &v)
来源：http://uf.panjiajie.cn

Ruby: JSON.parse(s)
来源：http://uh.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lx.hahajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://yz.lnxyls.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sh.9csxet.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gs.shxzukj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qc.newstarts.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://dd.gzmigu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nu.panjiajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nh.shxzukj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bb.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ty.nicolike.cn

[K04] 读取 JSON 文件
来源：http://np.szsharing.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rt.haigaiapp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wn.wgjwhj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bj.bjjhwx.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vq.9csxet.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qv.hnjuh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://da.jianghongdianzi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dx.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nk.huixiangedu.cn

[K05] 深拷贝对象
来源：http://au.huanxung.cn

Py:   copy.deepcopy(obj)
来源：http://jo.szxytkj.cn

PHP:  unserialize(serialize($obj));
来源：http://ls.chemitech.net.cn

JS:   structuredClone(obj)
来源：http://vs.bjjhwx.cn

TS:   structuredClone(obj)
来源：http://zr.asd995.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ia.haigaiapp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hd.huixinmuqiang.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pp.bjjhwx.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://jw.yuntaijiaju.cn

[K06] 解析 URL 查询串
来源：http://db.521024.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kg.bjjhwx.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mr.colortex.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wv.szsharing.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sd.panjiajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fc.521024.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sk.nicolike.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bn.yuntaijiaju.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ih.wgjwhj.cn

[K07] 进制转换
来源：http://yb.colortex.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ss.shxzukj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cr.nszjky.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tn.huixiangedu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ns.panjiajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dn.521024.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fk.huixiangedu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ma.521024.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mo.gzmigu.cn

[K08] 二进制序列化（非 JSON）
来源：http://uc.yuexingan06.cn

Py:   pickle.dumps(obj)
来源：http://lz.nicolike.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vk.szxytkj.cn

JS:   v8.serialize(obj)        // Node
来源：http://qg.jianghongdianzi.cn

TS:   v8.serialize(obj)        // Node
来源：http://qi.newstarts.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://oq.jianghongdianzi.cn

Go:   encoding/gob
来源：http://bu.shtwfgs.cn

Ruby: Marshal.dump(obj)
来源：http://yy.nicolike.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ac.huanxung.cn

================================================================================
来源：http://gc.lnxyls.cn

L. 网络请求
来源：http://bp.szsharing.cn

================================================================================
来源：http://yz.jctech888.com.cn

[L01] 发送 GET 请求
来源：http://ns.gzmigu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vk.jctech888.com.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://li.chemitech.net.cn

JS:   await fetch(url)
来源：http://zn.yuntaijiaju.cn

TS:   await fetch(url)
来源：http://ct.chemitech.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yc.bjjhwx.cn

Go:   resp, err := http.Get(url)
来源：http://aa.hahajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jf.shxzskj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://er.shtwfgs.cn

[L02] 发送 POST JSON
来源：http://rc.hahajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fa.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qu.yuexingan06.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pc.bjjhwx.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qy.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ir.hnjuh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pq.szsharing.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://re.lnxyls.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ee.9csxet.cn

[L03] 设置自定义请求头
来源：http://qp.bjjhwx.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kz.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vj.huanxung.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tk.asd995.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rv.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gb.wgjwhj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ob.hnjuh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://aq.huixinmuqiang.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vr.bjjhwx.cn

[L04] 设置超时
来源：http://qz.yuexingan06.cn

Py:   requests.get(url, timeout=5)
来源：http://us.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sl.colortex.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wk.huanxung.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://km.yuexingan06.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://iz.haigaiapp.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cu.shxzskj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nd.huanxung.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ej.yuexingan06.cn

[L05] 上传文件（multipart）
来源：http://vp.nszjky.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://od.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cy.jianghongdianzi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pk.shtwfgs.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sy.lnxyls.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://eg.gzmigu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://eu.yuntaijiaju.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lg.huixiangedu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ou.521024.cn

[L06] 解析响应为 JSON
来源：http://hg.yuntaijiaju.cn

Py:   resp.json()
来源：http://qp.shxzukj.cn

PHP:  json_decode($body, true);
来源：http://lt.chemitech.net.cn

JS:   await resp.json()
来源：http://oa.nszjky.cn

TS:   await resp.json()
来源：http://tm.haigaiapp.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uf.asd995.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ne.panjiajie.cn

Ruby: JSON.parse(resp.body)
来源：http://ro.haigaiapp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zl.jctech888.com.cn

[L07] 处理 HTTP 状态码
来源：http://ed.haigaiapp.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xa.gzmigu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ay.gzmigu.cn

JS:   resp.ok;  resp.status
来源：http://te.hnjuh.cn

TS:   resp.ok;  resp.status
来源：http://ca.szsharing.cn

Java: resp.statusCode()
来源：http://tk.wgjwhj.cn

Go:   resp.StatusCode
来源：http://xa.wgjwhj.cn

Ruby: resp.code.to_i
来源：http://gk.panjiajie.cn

C#:   (int)resp.StatusCode
来源：http://zt.yuexingan06.cn

[L08] 并发请求多个地址
来源：http://ar.yuexingan06.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://la.bookmarksfly.cn

PHP:  curl_multi_init() 系列
来源：http://pi.jctech888.com.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yx.wgjwhj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://md.szxytkj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gz.9csxet.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jf.huixiangedu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wt.szsharing.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ky.hahajie.cn

================================================================================
来源：http://be.jctech888.com.cn

M. 命令行 / 进程 / 环境
来源：http://ko.szsharing.cn

================================================================================
来源：http://zv.muxihuayi.cn

[M01] 读取命令行参数
来源：http://df.9csxet.cn

Py:   sys.argv[1:]
来源：http://oe.chemitech.net.cn

PHP:  $argv;  $argc;
来源：http://wv.nicolike.cn

JS:   process.argv.slice(2)
来源：http://wq.muxihuayi.cn

TS:   process.argv.slice(2)
来源：http://uf.hnjuh.cn

Java: args 数组（main 方法参数）
来源：http://hv.yuexingan06.cn

Go:   os.Args[1:]
来源：http://um.haigaiapp.cn

Ruby: ARGV
来源：http://bv.gzmigu.cn

C#:   args 数组（Main 方法参数）
来源：http://gg.jctech888.com.cn

[M02] 读取环境变量
来源：http://xe.hahajie.cn

Py:   os.environ.get("HOME")
来源：http://ix.shxzskj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ix.gzmigu.cn

JS:   process.env.HOME
来源：http://zt.newstarts.cn

TS:   process.env.HOME
来源：http://mj.jianghongdianzi.cn

Java: System.getenv("HOME")
来源：http://nn.asd995.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pd.yuexingan06.cn

Ruby: ENV["HOME"]
来源：http://gl.jianghongdianzi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nb.asd995.cn

[M03] 执行外部命令
来源：http://me.lnxyls.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zo.bjjhwx.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://no.haigaiapp.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xe.bookmarksfly.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://lf.huanxung.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rk.yuntaijiaju.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://iv.huixiangedu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://le.nszjky.cn

C#:   Process.Start("ls", "-l");
来源：http://mc.521024.cn

[M04] 获取当前工作目录
来源：http://dn.9csxet.cn

Py:   os.getcwd()
来源：http://im.muxihuayi.cn

PHP:  getcwd();
来源：http://uh.colortex.cn

JS:   process.cwd()
来源：http://ph.newstarts.cn

TS:   process.cwd()
来源：http://fd.muxihuayi.cn

Java: Path.of("").toAbsolutePath()
来源：http://rf.yuntaijiaju.cn

Go:   os.Getwd()
来源：http://nw.muxihuayi.cn

Ruby: Dir.pwd
来源：http://ld.shxzukj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zl.521024.cn

[M05] 设置退出码
来源：http://sd.muxihuayi.cn

Py:   sys.exit(1)
来源：http://we.szsharing.cn

PHP:  exit(1);
来源：http://kg.newstarts.cn

JS:   process.exit(1)
来源：http://gk.shxzukj.cn

TS:   process.exit(1)
来源：http://ad.bjjhwx.cn

Java: System.exit(1)
来源：http://lk.hahajie.cn

Go:   os.Exit(1)
来源：http://ew.9csxet.cn

Ruby: exit 1
来源：http://iz.shtwfgs.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wu.huixinmuqiang.cn

[M06] 向标准错误输出
来源：http://je.521024.cn

Py:   print("err", file=sys.stderr)
来源：http://un.huixinmuqiang.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://uv.yuexingan06.cn

JS:   console.error("err")
来源：http://lr.yuntaijiaju.cn

TS:   console.error("err")
来源：http://hm.shxzukj.cn

Java: System.err.println("err")
来源：http://uq.bjjhwx.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ej.yuexingan06.cn

Ruby: warn "err"
来源：http://pc.yuexingan06.cn

C#:   Console.Error.WriteLine("err")
来源：http://aa.wgjwhj.cn

[M07] 判断是否为主入口
来源：http://lt.haigaiapp.cn

Py:   if __name__ == "__main__":
来源：http://wm.huixiangedu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://os.huanxung.cn

JS:   require.main === module
来源：http://ke.jctech888.com.cn

TS:   require.main === module
来源：http://la.muxihuayi.cn

Java: public static void main(String[] args)
来源：http://jo.yuntaijiaju.cn

Go:   func main()
来源：http://ip.shxzukj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xd.hnjuh.cn

C#:   static void Main(string[] args)
来源：http://ud.hnjuh.cn

[M08] 获取系统与运行时信息
来源：http://bt.lnxyls.cn

Py:   platform.system();  platform.python_version()
来源：http://ye.panjiajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://qn.shxzukj.cn

JS:   process.platform;  process.version
来源：http://ds.huixinmuqiang.cn

TS:   process.platform;  process.version
来源：http://zx.szsharing.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hk.chemitech.net.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ay.szsharing.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zh.gzmigu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bn.colortex.cn

================================================================================
来源：http://ic.huixiangedu.cn

N. 数据结构与算法
来源：http://yc.nicolike.cn

================================================================================
来源：http://wy.bookmarksfly.cn


<!-- 参考信息 -->