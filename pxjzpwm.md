代发 wailian999

[J03] 字符串解析为日期
来源：http://ye.huixiangedu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qj.wgjwhj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jx.huanxung.cn

JS:   new Date("2024-01-02")
来源：http://yq.szsharing.cn

TS:   new Date("2024-01-02")
来源：http://yq.huixiangedu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mo.yuntaijiaju.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gc.szsharing.cn

Ruby: Date.parse("2024-01-02")
来源：http://nc.gzmigu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gu.muxihuayi.cn

[J04] 时间戳与日期互转
来源：http://tj.huixiangedu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bg.haigaiapp.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nv.newstarts.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ks.szsharing.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ji.jctech888.com.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gz.9csxet.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nj.yuntaijiaju.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ii.yuntaijiaju.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rb.hnjuh.cn

[J05] 时间加减（加 7 天）
来源：http://tx.521024.cn

Py:   now + timedelta(days=7)
来源：http://iu.panjiajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://gk.asd995.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gv.szsharing.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://eu.szsharing.cn

Java: LocalDate.now().plusDays(7)
来源：http://oy.szsharing.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jn.nicolike.cn

Ruby: Time.now + 7 * 86400
来源：http://ld.hahajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://mi.521024.cn

[J06] 计算两时间之差
来源：http://fh.huixinmuqiang.cn

Py:   (end - start).total_seconds()
来源：http://bl.wgjwhj.cn

PHP:  $end->diff($start)->days;
来源：http://tw.panjiajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qk.haigaiapp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yf.huanxung.cn

Java: Duration.between(start, end).toSeconds()
来源：http://sb.szsharing.cn

Go:   end.Sub(start).Hours()
来源：http://np.szsharing.cn

Ruby: end - start                 # 返回秒数
来源：http://ut.jianghongdianzi.cn

C#:   (end - start).TotalSeconds
来源：http://ha.nszjky.cn

[J07] 比较两个日期
来源：http://lf.lnxyls.cn

Py:   d1 < d2;  d1 == d2
来源：http://rw.shxzskj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://en.bjjhwx.cn

JS:   d1.getTime() < d2.getTime()
来源：http://id.szsharing.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zv.jctech888.com.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nf.nicolike.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://za.gzmigu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://tf.panjiajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://ye.hahajie.cn

[J08] 提取年月日与星期
来源：http://ob.hnjuh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://te.newstarts.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ca.shxzukj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rw.yuexingan06.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ky.chemitech.net.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://th.nszjky.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wk.szxytkj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vr.wgjwhj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://za.jctech888.com.cn

[J09] 时区处理
来源：http://tx.9csxet.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ot.gzmigu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ip.haigaiapp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hp.jctech888.com.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vw.newstarts.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.wgjwhj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xg.521024.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://by.lnxyls.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wu.jctech888.com.cn

[J10] 取今天 / 本月第一天
来源：http://su.chemitech.net.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zv.bjjhwx.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://by.huixinmuqiang.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fw.yuexingan06.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cx.haigaiapp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lu.yuntaijiaju.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jn.hnjuh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zf.shxzukj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yx.huixiangedu.cn

================================================================================
来源：http://yf.asd995.cn

K. JSON 与序列化
来源：http://lk.chemitech.net.cn

================================================================================
来源：http://mx.jianghongdianzi.cn

[K01] 对象转 JSON 字符串
来源：http://xi.colortex.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wt.hnjuh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fz.chemitech.net.cn

JS:   JSON.stringify(obj)
来源：http://cn.jianghongdianzi.cn

TS:   JSON.stringify(obj)
来源：http://sj.bjjhwx.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ul.colortex.cn

Go:   json.Marshal(obj)
来源：http://bl.chemitech.net.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zr.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://tg.szxytkj.cn

[K02] JSON 字符串转对象
来源：http://hq.haigaiapp.cn

Py:   json.loads(s)
来源：http://il.lnxyls.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ia.newstarts.cn

JS:   JSON.parse(s)
来源：http://np.huanxung.cn

TS:   JSON.parse(s)
来源：http://at.gzmigu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gw.asd995.cn

Go:   json.Unmarshal(data, &v)
来源：http://lq.asd995.cn

Ruby: JSON.parse(s)
来源：http://do.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jg.nicolike.cn

[K03] JSON 美化输出（带缩进）
来源：http://iy.asd995.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wn.yuexingan06.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zw.yuexingan06.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ru.nicolike.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ho.muxihuayi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lf.bjjhwx.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gg.jctech888.com.cn

Ruby: JSON.pretty_generate(obj)
来源：http://su.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nd.huixinmuqiang.cn

[K04] 读取 JSON 文件
来源：http://ec.shxzukj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sg.haigaiapp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sf.bookmarksfly.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tk.huanxung.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gd.huixiangedu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xf.gzmigu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nk.huixiangedu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gu.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jq.gzmigu.cn

[K05] 深拷贝对象
来源：http://yi.yuntaijiaju.cn

Py:   copy.deepcopy(obj)
来源：http://kz.szsharing.cn

PHP:  unserialize(serialize($obj));
来源：http://wf.haigaiapp.cn

JS:   structuredClone(obj)
来源：http://im.chemitech.net.cn

TS:   structuredClone(obj)
来源：http://fw.newstarts.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xg.yuntaijiaju.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wv.chemitech.net.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://da.huixinmuqiang.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fr.jctech888.com.cn

[K06] 解析 URL 查询串
来源：http://oq.hahajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gr.wgjwhj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ub.nicolike.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eb.haigaiapp.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vp.gzmigu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://es.gzmigu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mv.asd995.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pj.panjiajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fa.szsharing.cn

[K07] 进制转换
来源：http://tg.shxzukj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://so.colortex.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wl.9csxet.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dh.yuntaijiaju.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zp.lnxyls.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xz.yuexingan06.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dt.shxzukj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dl.huixinmuqiang.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dh.panjiajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://if.9csxet.cn

Py:   pickle.dumps(obj)
来源：http://yk.colortex.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vk.huanxung.cn

JS:   v8.serialize(obj)        // Node
来源：http://dp.lnxyls.cn

TS:   v8.serialize(obj)        // Node
来源：http://zi.521024.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://es.hahajie.cn

Go:   encoding/gob
来源：http://da.hnjuh.cn

Ruby: Marshal.dump(obj)
来源：http://aa.szxytkj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jx.shtwfgs.cn

================================================================================
来源：http://ay.wgjwhj.cn

L. 网络请求
来源：http://uw.szxytkj.cn

================================================================================
来源：http://hb.yuntaijiaju.cn

[L01] 发送 GET 请求
来源：http://zg.jctech888.com.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nz.yuexingan06.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rt.shxzukj.cn

JS:   await fetch(url)
来源：http://dn.colortex.cn

TS:   await fetch(url)
来源：http://vy.haigaiapp.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wn.bookmarksfly.cn

Go:   resp, err := http.Get(url)
来源：http://qv.panjiajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fi.521024.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gv.jianghongdianzi.cn

[L02] 发送 POST JSON
来源：http://vl.newstarts.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bu.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hl.bookmarksfly.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://px.yuexingan06.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kr.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ha.szsharing.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ji.huixiangedu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rc.hnjuh.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bw.newstarts.cn

[L03] 设置自定义请求头
来源：http://mu.nszjky.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nj.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nf.jianghongdianzi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ux.huixiangedu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zg.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ye.haigaiapp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ru.bjjhwx.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ks.9csxet.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ga.yuntaijiaju.cn

[L04] 设置超时
来源：http://lg.hnjuh.cn

Py:   requests.get(url, timeout=5)
来源：http://no.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xp.chemitech.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gv.huanxung.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xf.hahajie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gd.haigaiapp.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tv.hnjuh.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://na.gzmigu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zo.szxytkj.cn

[L05] 上传文件（multipart）
来源：http://vd.chemitech.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nj.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gh.yuntaijiaju.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ta.wgjwhj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://oo.haigaiapp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ts.chemitech.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ap.szxytkj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vd.jianghongdianzi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pw.521024.cn

[L06] 解析响应为 JSON
来源：http://vh.nszjky.cn

Py:   resp.json()
来源：http://er.huixinmuqiang.cn

PHP:  json_decode($body, true);
来源：http://mj.szsharing.cn

JS:   await resp.json()
来源：http://oa.huixinmuqiang.cn

TS:   await resp.json()
来源：http://xp.huixiangedu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ui.gzmigu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yo.muxihuayi.cn

Ruby: JSON.parse(resp.body)
来源：http://wu.nicolike.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://he.asd995.cn

[L07] 处理 HTTP 状态码
来源：http://qp.shxzskj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qf.colortex.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rn.gzmigu.cn

JS:   resp.ok;  resp.status
来源：http://kj.bookmarksfly.cn

TS:   resp.ok;  resp.status
来源：http://xa.panjiajie.cn

Java: resp.statusCode()
来源：http://ga.bjjhwx.cn

Go:   resp.StatusCode
来源：http://to.colortex.cn

Ruby: resp.code.to_i
来源：http://vh.521024.cn

C#:   (int)resp.StatusCode
来源：http://vk.bookmarksfly.cn

[L08] 并发请求多个地址
来源：http://do.muxihuayi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://oy.huanxung.cn

PHP:  curl_multi_init() 系列
来源：http://qy.huanxung.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nj.chemitech.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qf.huanxung.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ce.newstarts.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ch.muxihuayi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kd.lnxyls.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uw.szsharing.cn

================================================================================
来源：http://lr.shxzukj.cn

M. 命令行 / 进程 / 环境
来源：http://bk.9csxet.cn

================================================================================
来源：http://sf.nszjky.cn

[M01] 读取命令行参数
来源：http://rv.wgjwhj.cn

Py:   sys.argv[1:]
来源：http://yq.hahajie.cn

PHP:  $argv;  $argc;
来源：http://sv.colortex.cn

JS:   process.argv.slice(2)
来源：http://by.521024.cn

TS:   process.argv.slice(2)
来源：http://gc.haigaiapp.cn

Java: args 数组（main 方法参数）
来源：http://tn.521024.cn

Go:   os.Args[1:]
来源：http://ey.asd995.cn

Ruby: ARGV
来源：http://px.haigaiapp.cn

C#:   args 数组（Main 方法参数）
来源：http://am.shxzukj.cn

[M02] 读取环境变量
来源：http://ly.shxzukj.cn

Py:   os.environ.get("HOME")
来源：http://pi.nszjky.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nb.bookmarksfly.cn

JS:   process.env.HOME
来源：http://gp.huanxung.cn

TS:   process.env.HOME
来源：http://ku.huanxung.cn

Java: System.getenv("HOME")
来源：http://zi.huixinmuqiang.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mw.shxzskj.cn

Ruby: ENV["HOME"]
来源：http://un.hnjuh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zq.nszjky.cn

[M03] 执行外部命令
来源：http://kn.jctech888.com.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rq.colortex.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kk.9csxet.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jk.jctech888.com.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fv.nicolike.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uc.gzmigu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://sb.colortex.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ol.nicolike.cn

C#:   Process.Start("ls", "-l");
来源：http://yl.bookmarksfly.cn

[M04] 获取当前工作目录
来源：http://tm.wgjwhj.cn

Py:   os.getcwd()
来源：http://hs.shtwfgs.cn

PHP:  getcwd();
来源：http://xg.521024.cn

JS:   process.cwd()
来源：http://zs.shxzukj.cn

TS:   process.cwd()
来源：http://ss.jctech888.com.cn

Java: Path.of("").toAbsolutePath()
来源：http://wg.9csxet.cn

Go:   os.Getwd()
来源：http://sw.chemitech.net.cn

Ruby: Dir.pwd
来源：http://up.shxzukj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qb.bookmarksfly.cn

[M05] 设置退出码
来源：http://ag.shxzskj.cn

Py:   sys.exit(1)
来源：http://wx.bookmarksfly.cn

PHP:  exit(1);
来源：http://lm.gzmigu.cn

JS:   process.exit(1)
来源：http://sn.hnjuh.cn

TS:   process.exit(1)
来源：http://bl.shxzskj.cn

Java: System.exit(1)
来源：http://ve.chemitech.net.cn

Go:   os.Exit(1)
来源：http://pe.newstarts.cn

Ruby: exit 1
来源：http://gi.colortex.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://js.521024.cn

[M06] 向标准错误输出
来源：http://jy.gzmigu.cn

Py:   print("err", file=sys.stderr)
来源：http://ut.wgjwhj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://sm.9csxet.cn

JS:   console.error("err")
来源：http://rg.bookmarksfly.cn

TS:   console.error("err")
来源：http://uz.nicolike.cn

Java: System.err.println("err")
来源：http://eg.huixiangedu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://no.bookmarksfly.cn

Ruby: warn "err"
来源：http://vi.shxzskj.cn

C#:   Console.Error.WriteLine("err")
来源：http://fp.hnjuh.cn

[M07] 判断是否为主入口
来源：http://ew.bjjhwx.cn

Py:   if __name__ == "__main__":
来源：http://ka.hahajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cc.hahajie.cn

JS:   require.main === module
来源：http://ar.lnxyls.cn

TS:   require.main === module
来源：http://sg.chemitech.net.cn

Java: public static void main(String[] args)
来源：http://gp.szxytkj.cn

Go:   func main()
来源：http://yk.521024.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://il.hahajie.cn

C#:   static void Main(string[] args)
来源：http://rm.colortex.cn

[M08] 获取系统与运行时信息
来源：http://nx.yuntaijiaju.cn

Py:   platform.system();  platform.python_version()
来源：http://dd.jianghongdianzi.cn

PHP:  PHP_OS;  phpversion();
来源：http://if.huixiangedu.cn

JS:   process.platform;  process.version
来源：http://hm.chemitech.net.cn

TS:   process.platform;  process.version
来源：http://ag.szxytkj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lq.muxihuayi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://uf.bjjhwx.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://id.nszjky.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://hc.haigaiapp.cn

================================================================================
来源：http://eb.bookmarksfly.cn

N. 数据结构与算法
来源：http://gg.bookmarksfly.cn

================================================================================
来源：http://bs.nszjky.cn


<!-- 参考信息 -->