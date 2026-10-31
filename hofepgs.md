代发 wailian999

[J03] 字符串解析为日期
来源：http://uk.hnjuh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pr.9csxet.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yj.hnjuh.cn

JS:   new Date("2024-01-02")
来源：http://ga.jctech888.com.cn

TS:   new Date("2024-01-02")
来源：http://ib.colortex.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ti.gzmigu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mk.yuexingan06.cn

Ruby: Date.parse("2024-01-02")
来源：http://jz.yuntaijiaju.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jn.jctech888.com.cn

[J04] 时间戳与日期互转
来源：http://xk.hahajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ps.bjjhwx.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://iw.szxytkj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fd.asd995.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://oa.jctech888.com.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pj.bookmarksfly.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vp.huanxung.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tq.shtwfgs.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yh.huixiangedu.cn

[J05] 时间加减（加 7 天）
来源：http://wh.newstarts.cn

Py:   now + timedelta(days=7)
来源：http://sg.lnxyls.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://md.muxihuayi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ry.huixinmuqiang.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fl.521024.cn

Java: LocalDate.now().plusDays(7)
来源：http://jv.huanxung.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fj.huixinmuqiang.cn

Ruby: Time.now + 7 * 86400
来源：http://ot.haigaiapp.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gw.muxihuayi.cn

[J06] 计算两时间之差
来源：http://ry.hnjuh.cn

Py:   (end - start).total_seconds()
来源：http://cv.bjjhwx.cn

PHP:  $end->diff($start)->days;
来源：http://df.panjiajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.huanxung.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qo.9csxet.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bz.hahajie.cn

Go:   end.Sub(start).Hours()
来源：http://jv.huixinmuqiang.cn

Ruby: end - start                 # 返回秒数
来源：http://yw.wgjwhj.cn

C#:   (end - start).TotalSeconds
来源：http://iv.huixinmuqiang.cn

[J07] 比较两个日期
来源：http://ej.szxytkj.cn

Py:   d1 < d2;  d1 == d2
来源：http://uq.9csxet.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xu.gzmigu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://os.muxihuayi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://id.gzmigu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qt.huixinmuqiang.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ku.9csxet.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ha.muxihuayi.cn

C#:   d1 < d2;  d1 == d2
来源：http://kn.jianghongdianzi.cn

[J08] 提取年月日与星期
来源：http://rr.haigaiapp.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://td.lnxyls.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zr.gzmigu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://px.szsharing.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://eu.haigaiapp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dz.9csxet.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xy.haigaiapp.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uh.colortex.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vq.huanxung.cn

[J09] 时区处理
来源：http://bp.jctech888.com.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ri.szsharing.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dt.szsharing.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ma.muxihuayi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zg.521024.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zh.hahajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qk.nicolike.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zp.nicolike.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xo.bookmarksfly.cn

[J10] 取今天 / 本月第一天
来源：http://um.muxihuayi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://nd.huixiangedu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nw.hnjuh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gz.huixinmuqiang.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fc.jianghongdianzi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://eb.panjiajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nm.hnjuh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ip.yuntaijiaju.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yd.yuntaijiaju.cn

================================================================================
来源：http://yd.asd995.cn

K. JSON 与序列化
来源：http://ll.yuntaijiaju.cn

================================================================================
来源：http://nr.gzmigu.cn

[K01] 对象转 JSON 字符串
来源：http://sr.muxihuayi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gr.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ab.huixinmuqiang.cn

JS:   JSON.stringify(obj)
来源：http://oj.huixinmuqiang.cn

TS:   JSON.stringify(obj)
来源：http://ys.jctech888.com.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pk.9csxet.cn

Go:   json.Marshal(obj)
来源：http://ll.hahajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ij.9csxet.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://nv.gzmigu.cn

[K02] JSON 字符串转对象
来源：http://ku.bookmarksfly.cn

Py:   json.loads(s)
来源：http://fc.jctech888.com.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gx.szsharing.cn

JS:   JSON.parse(s)
来源：http://fq.colortex.cn

TS:   JSON.parse(s)
来源：http://ai.nszjky.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zw.shxzukj.cn

Go:   json.Unmarshal(data, &v)
来源：http://do.szxytkj.cn

Ruby: JSON.parse(s)
来源：http://km.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ll.9csxet.cn

[K03] JSON 美化输出（带缩进）
来源：http://eb.muxihuayi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://oc.haigaiapp.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://el.shxzskj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://az.9csxet.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mu.szsharing.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pj.huanxung.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://eq.nszjky.cn

Ruby: JSON.pretty_generate(obj)
来源：http://tu.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bg.asd995.cn

[K04] 读取 JSON 文件
来源：http://kt.lnxyls.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dd.nszjky.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lm.521024.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bm.shtwfgs.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vo.gzmigu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yd.nicolike.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tk.bjjhwx.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://my.colortex.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gt.bjjhwx.cn

[K05] 深拷贝对象
来源：http://sc.szxytkj.cn

Py:   copy.deepcopy(obj)
来源：http://mh.newstarts.cn

PHP:  unserialize(serialize($obj));
来源：http://lu.haigaiapp.cn

JS:   structuredClone(obj)
来源：http://yz.haigaiapp.cn

TS:   structuredClone(obj)
来源：http://io.bjjhwx.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zo.jctech888.com.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ig.colortex.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ni.hnjuh.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://kt.yuntaijiaju.cn

[K06] 解析 URL 查询串
来源：http://wb.haigaiapp.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lk.9csxet.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qw.jctech888.com.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eg.chemitech.net.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nk.colortex.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jk.gzmigu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xc.wgjwhj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://na.lnxyls.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://em.huanxung.cn

[K07] 进制转换
来源：http://hp.asd995.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ot.huixinmuqiang.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://io.hnjuh.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ot.newstarts.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hn.nszjky.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jc.9csxet.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vv.shtwfgs.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zz.panjiajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vv.haigaiapp.cn

[K08] 二进制序列化（非 JSON）
来源：http://nf.newstarts.cn

Py:   pickle.dumps(obj)
来源：http://ur.szxytkj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://jq.yuexingan06.cn

JS:   v8.serialize(obj)        // Node
来源：http://nc.huanxung.cn

TS:   v8.serialize(obj)        // Node
来源：http://kk.huixinmuqiang.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yr.nszjky.cn

Go:   encoding/gob
来源：http://ad.szsharing.cn

Ruby: Marshal.dump(obj)
来源：http://yk.jctech888.com.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fb.huanxung.cn

================================================================================
来源：http://bk.huixinmuqiang.cn

L. 网络请求
来源：http://ff.nszjky.cn

================================================================================
来源：http://ue.szxytkj.cn

[L01] 发送 GET 请求
来源：http://yo.lnxyls.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tl.haigaiapp.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ab.shtwfgs.cn

JS:   await fetch(url)
来源：http://vw.9csxet.cn

TS:   await fetch(url)
来源：http://xc.shxzukj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tq.asd995.cn

Go:   resp, err := http.Get(url)
来源：http://yo.huixinmuqiang.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xp.asd995.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://li.9csxet.cn

[L02] 发送 POST JSON
来源：http://at.huanxung.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cw.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ev.szxytkj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jh.haigaiapp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fq.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pk.huixiangedu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dr.nszjky.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cz.gzmigu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mi.shxzukj.cn

[L03] 设置自定义请求头
来源：http://ki.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://og.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xu.haigaiapp.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vi.9csxet.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cd.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rp.shtwfgs.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mf.hahajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ot.9csxet.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ag.shxzskj.cn

[L04] 设置超时
来源：http://rh.yuexingan06.cn

Py:   requests.get(url, timeout=5)
来源：http://qt.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lk.colortex.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mo.gzmigu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ry.yuexingan06.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://px.huanxung.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tu.szxytkj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qz.gzmigu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bn.huixiangedu.cn

[L05] 上传文件（multipart）
来源：http://zk.shxzskj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vx.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hb.gzmigu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pd.colortex.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yw.shtwfgs.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ji.yuntaijiaju.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cc.chemitech.net.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ep.shtwfgs.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sd.jianghongdianzi.cn

[L06] 解析响应为 JSON
来源：http://jb.bookmarksfly.cn

Py:   resp.json()
来源：http://aj.huixinmuqiang.cn

PHP:  json_decode($body, true);
来源：http://cl.shxzukj.cn

JS:   await resp.json()
来源：http://lj.asd995.cn

TS:   await resp.json()
来源：http://ev.bjjhwx.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://da.yuexingan06.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zk.jianghongdianzi.cn

Ruby: JSON.parse(resp.body)
来源：http://yq.9csxet.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zc.jianghongdianzi.cn

[L07] 处理 HTTP 状态码
来源：http://xz.bjjhwx.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ei.huixiangedu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cw.bjjhwx.cn

JS:   resp.ok;  resp.status
来源：http://rr.chemitech.net.cn

TS:   resp.ok;  resp.status
来源：http://ud.jctech888.com.cn

Java: resp.statusCode()
来源：http://ds.shtwfgs.cn

Go:   resp.StatusCode
来源：http://ms.szsharing.cn

Ruby: resp.code.to_i
来源：http://nn.bookmarksfly.cn

C#:   (int)resp.StatusCode
来源：http://nk.nicolike.cn

[L08] 并发请求多个地址
来源：http://wk.jianghongdianzi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://og.huanxung.cn

PHP:  curl_multi_init() 系列
来源：http://av.shtwfgs.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uy.newstarts.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wq.shtwfgs.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ak.nicolike.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tz.huanxung.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ws.521024.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qo.hnjuh.cn

================================================================================
来源：http://oh.lnxyls.cn

M. 命令行 / 进程 / 环境
来源：http://lp.shtwfgs.cn

================================================================================
来源：http://zd.bjjhwx.cn

[M01] 读取命令行参数
来源：http://po.haigaiapp.cn

Py:   sys.argv[1:]
来源：http://ct.chemitech.net.cn

PHP:  $argv;  $argc;
来源：http://jc.panjiajie.cn

JS:   process.argv.slice(2)
来源：http://qk.gzmigu.cn

TS:   process.argv.slice(2)
来源：http://ln.yuexingan06.cn

Java: args 数组（main 方法参数）
来源：http://do.szsharing.cn

Go:   os.Args[1:]
来源：http://oa.nszjky.cn

Ruby: ARGV
来源：http://lo.bjjhwx.cn

C#:   args 数组（Main 方法参数）
来源：http://sm.nszjky.cn

[M02] 读取环境变量
来源：http://df.huixiangedu.cn

Py:   os.environ.get("HOME")
来源：http://cv.chemitech.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ra.huixiangedu.cn

JS:   process.env.HOME
来源：http://pb.bjjhwx.cn

TS:   process.env.HOME
来源：http://nw.huixiangedu.cn

Java: System.getenv("HOME")
来源：http://ji.chemitech.net.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://au.huixinmuqiang.cn

Ruby: ENV["HOME"]
来源：http://ri.bookmarksfly.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jr.hahajie.cn

[M03] 执行外部命令
来源：http://jv.9csxet.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://st.gzmigu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bi.asd995.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://tt.shtwfgs.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ky.muxihuayi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://oa.lnxyls.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://iz.hahajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ht.panjiajie.cn

C#:   Process.Start("ls", "-l");
来源：http://ua.521024.cn

[M04] 获取当前工作目录
来源：http://un.bjjhwx.cn

Py:   os.getcwd()
来源：http://fe.muxihuayi.cn

PHP:  getcwd();
来源：http://pf.huanxung.cn

JS:   process.cwd()
来源：http://qj.bjjhwx.cn

TS:   process.cwd()
来源：http://un.shxzukj.cn

Java: Path.of("").toAbsolutePath()
来源：http://md.newstarts.cn

Go:   os.Getwd()
来源：http://zu.szsharing.cn

Ruby: Dir.pwd
来源：http://pk.colortex.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qg.muxihuayi.cn

[M05] 设置退出码
来源：http://kd.521024.cn

Py:   sys.exit(1)
来源：http://dj.9csxet.cn

PHP:  exit(1);
来源：http://hb.jctech888.com.cn

JS:   process.exit(1)
来源：http://ye.colortex.cn

TS:   process.exit(1)
来源：http://wm.hnjuh.cn

Java: System.exit(1)
来源：http://jz.newstarts.cn

Go:   os.Exit(1)
来源：http://lk.yuntaijiaju.cn

Ruby: exit 1
来源：http://sa.asd995.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ek.shxzukj.cn

[M06] 向标准错误输出
来源：http://pa.chemitech.net.cn

Py:   print("err", file=sys.stderr)
来源：http://rb.shxzukj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://uk.nicolike.cn

JS:   console.error("err")
来源：http://lj.hnjuh.cn

TS:   console.error("err")
来源：http://rf.huixinmuqiang.cn

Java: System.err.println("err")
来源：http://gs.hahajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mb.hahajie.cn

Ruby: warn "err"
来源：http://on.panjiajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://wf.panjiajie.cn

[M07] 判断是否为主入口
来源：http://qk.wgjwhj.cn

Py:   if __name__ == "__main__":
来源：http://tc.szsharing.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jn.9csxet.cn

JS:   require.main === module
来源：http://qs.szsharing.cn

TS:   require.main === module
来源：http://ib.shxzukj.cn

Java: public static void main(String[] args)
来源：http://mt.huanxung.cn

Go:   func main()
来源：http://zv.haigaiapp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ci.asd995.cn

C#:   static void Main(string[] args)
来源：http://sl.chemitech.net.cn

[M08] 获取系统与运行时信息
来源：http://vd.szxytkj.cn

Py:   platform.system();  platform.python_version()
来源：http://cf.asd995.cn

PHP:  PHP_OS;  phpversion();
来源：http://zx.nszjky.cn

JS:   process.platform;  process.version
来源：http://sp.jctech888.com.cn

TS:   process.platform;  process.version
来源：http://ce.yuexingan06.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://aa.bookmarksfly.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://nz.9csxet.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rh.wgjwhj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ty.yuexingan06.cn

================================================================================
来源：http://tm.huixinmuqiang.cn

N. 数据结构与算法
来源：http://jz.muxihuayi.cn

================================================================================
来源：http://uu.hnjuh.cn


<!-- 参考信息 -->