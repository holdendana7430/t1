代发 wailian999

[J03] 字符串解析为日期
来源：http://tu.huixinmuqiang.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yq.shxzukj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ia.chemitech.net.cn

JS:   new Date("2024-01-02")
来源：http://sc.521024.cn

TS:   new Date("2024-01-02")
来源：http://iw.jctech888.com.cn

Java: LocalDate.parse("2024-01-02")
来源：http://km.shxzukj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sb.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://kq.huanxung.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://je.lnxyls.cn

[J04] 时间戳与日期互转
来源：http://rz.shtwfgs.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zp.panjiajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://za.szsharing.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://et.szsharing.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://at.hnjuh.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ao.bjjhwx.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uw.szxytkj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hu.shtwfgs.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jf.shxzskj.cn

[J05] 时间加减（加 7 天）
来源：http://lh.huixinmuqiang.cn

Py:   now + timedelta(days=7)
来源：http://nm.9csxet.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://dp.shxzukj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yt.yuntaijiaju.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ae.panjiajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://gy.jianghongdianzi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wq.bookmarksfly.cn

Ruby: Time.now + 7 * 86400
来源：http://pr.hnjuh.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rd.jctech888.com.cn

[J06] 计算两时间之差
来源：http://hl.haigaiapp.cn

Py:   (end - start).total_seconds()
来源：http://lh.huixinmuqiang.cn

PHP:  $end->diff($start)->days;
来源：http://nc.wgjwhj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dy.jctech888.com.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kc.hnjuh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ee.bjjhwx.cn

Go:   end.Sub(start).Hours()
来源：http://ic.gzmigu.cn

Ruby: end - start                 # 返回秒数
来源：http://ja.chemitech.net.cn

C#:   (end - start).TotalSeconds
来源：http://dp.huixinmuqiang.cn

[J07] 比较两个日期
来源：http://ic.yuntaijiaju.cn

Py:   d1 < d2;  d1 == d2
来源：http://rg.huixiangedu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nh.newstarts.cn

JS:   d1.getTime() < d2.getTime()
来源：http://dh.bookmarksfly.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xe.haigaiapp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ye.521024.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qu.muxihuayi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://oh.jianghongdianzi.cn

C#:   d1 < d2;  d1 == d2
来源：http://bc.szsharing.cn

[J08] 提取年月日与星期
来源：http://is.haigaiapp.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wi.wgjwhj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hw.shxzskj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sl.hnjuh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qq.hnjuh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mj.9csxet.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ts.szxytkj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://av.bookmarksfly.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yf.szsharing.cn

[J09] 时区处理
来源：http://ph.haigaiapp.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://li.bookmarksfly.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nu.nszjky.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cq.nszjky.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kp.shtwfgs.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bs.shtwfgs.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pc.hnjuh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ae.shxzukj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cd.lnxyls.cn

[J10] 取今天 / 本月第一天
来源：http://yg.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bx.szsharing.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mp.muxihuayi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bt.newstarts.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qx.hnjuh.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mj.nicolike.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nr.bjjhwx.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xz.jianghongdianzi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vw.huixiangedu.cn

================================================================================
来源：http://yi.panjiajie.cn

K. JSON 与序列化
来源：http://nc.huanxung.cn

================================================================================
来源：http://lf.newstarts.cn

[K01] 对象转 JSON 字符串
来源：http://qr.yuntaijiaju.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://aj.jctech888.com.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qk.shxzukj.cn

JS:   JSON.stringify(obj)
来源：http://wh.shtwfgs.cn

TS:   JSON.stringify(obj)
来源：http://yt.wgjwhj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gg.gzmigu.cn

Go:   json.Marshal(obj)
来源：http://of.huixinmuqiang.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zd.panjiajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wn.muxihuayi.cn

[K02] JSON 字符串转对象
来源：http://ht.nicolike.cn

Py:   json.loads(s)
来源：http://lr.lnxyls.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ir.huixinmuqiang.cn

JS:   JSON.parse(s)
来源：http://fb.shxzskj.cn

TS:   JSON.parse(s)
来源：http://su.nszjky.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://up.gzmigu.cn

Go:   json.Unmarshal(data, &v)
来源：http://rr.asd995.cn

Ruby: JSON.parse(s)
来源：http://xl.521024.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nr.asd995.cn

[K03] JSON 美化输出（带缩进）
来源：http://sm.colortex.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://of.haigaiapp.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qg.huixinmuqiang.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ka.bookmarksfly.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ya.newstarts.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bj.huixiangedu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://px.huixinmuqiang.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vi.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://my.hahajie.cn

[K04] 读取 JSON 文件
来源：http://ue.jianghongdianzi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ed.colortex.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://il.lnxyls.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fq.huixiangedu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lh.hahajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ew.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ap.hahajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://oz.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dp.bjjhwx.cn

[K05] 深拷贝对象
来源：http://jw.bjjhwx.cn

Py:   copy.deepcopy(obj)
来源：http://ep.chemitech.net.cn

PHP:  unserialize(serialize($obj));
来源：http://di.haigaiapp.cn

JS:   structuredClone(obj)
来源：http://it.wgjwhj.cn

TS:   structuredClone(obj)
来源：http://ch.jctech888.com.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wx.nicolike.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dn.521024.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://st.chemitech.net.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://nu.haigaiapp.cn

[K06] 解析 URL 查询串
来源：http://da.bjjhwx.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sn.jianghongdianzi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pv.hahajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dh.huixinmuqiang.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sc.newstarts.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sy.newstarts.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qr.colortex.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rm.huanxung.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zm.nicolike.cn

[K07] 进制转换
来源：http://dy.colortex.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zt.bookmarksfly.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gz.haigaiapp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xy.huixiangedu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hf.bjjhwx.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xy.521024.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gh.jctech888.com.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ym.nszjky.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hf.szsharing.cn

[K08] 二进制序列化（非 JSON）
来源：http://st.huixiangedu.cn

Py:   pickle.dumps(obj)
来源：http://ch.jctech888.com.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pu.gzmigu.cn

JS:   v8.serialize(obj)        // Node
来源：http://jx.newstarts.cn

TS:   v8.serialize(obj)        // Node
来源：http://iq.panjiajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fq.lnxyls.cn

Go:   encoding/gob
来源：http://gl.yuexingan06.cn

Ruby: Marshal.dump(obj)
来源：http://yq.bookmarksfly.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zr.shxzskj.cn

================================================================================
来源：http://ar.hnjuh.cn

L. 网络请求
来源：http://sn.shtwfgs.cn

================================================================================
来源：http://qb.asd995.cn

[L01] 发送 GET 请求
来源：http://fj.9csxet.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lg.chemitech.net.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nc.huixinmuqiang.cn

JS:   await fetch(url)
来源：http://ib.szsharing.cn

TS:   await fetch(url)
来源：http://ss.colortex.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fm.huanxung.cn

Go:   resp, err := http.Get(url)
来源：http://rb.huixinmuqiang.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ek.nszjky.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wa.panjiajie.cn

[L02] 发送 POST JSON
来源：http://js.nicolike.cn

Py:   requests.post(url, json={"a": 1})
来源：http://tb.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dq.yuexingan06.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nl.nszjky.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jb.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vt.asd995.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ey.huixiangedu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ox.521024.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gs.jianghongdianzi.cn

[L03] 设置自定义请求头
来源：http://vg.szxytkj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rr.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cp.yuntaijiaju.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ds.hnjuh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ji.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ww.nicolike.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://it.chemitech.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yu.nicolike.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yr.muxihuayi.cn

[L04] 设置超时
来源：http://yn.colortex.cn

Py:   requests.get(url, timeout=5)
来源：http://bm.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://al.colortex.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aq.nicolike.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ks.wgjwhj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lg.panjiajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rt.asd995.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lc.haigaiapp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ts.jianghongdianzi.cn

[L05] 上传文件（multipart）
来源：http://hz.panjiajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qd.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://op.jianghongdianzi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://az.haigaiapp.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gp.chemitech.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zq.lnxyls.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jj.muxihuayi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mp.bookmarksfly.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ra.chemitech.net.cn

[L06] 解析响应为 JSON
来源：http://vd.bjjhwx.cn

Py:   resp.json()
来源：http://uu.szsharing.cn

PHP:  json_decode($body, true);
来源：http://tu.shtwfgs.cn

JS:   await resp.json()
来源：http://gg.hnjuh.cn

TS:   await resp.json()
来源：http://dk.shtwfgs.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dr.asd995.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yl.haigaiapp.cn

Ruby: JSON.parse(resp.body)
来源：http://wh.hahajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wj.9csxet.cn

[L07] 处理 HTTP 状态码
来源：http://lp.shxzskj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gg.9csxet.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vv.shtwfgs.cn

JS:   resp.ok;  resp.status
来源：http://wb.jctech888.com.cn

TS:   resp.ok;  resp.status
来源：http://nd.huixiangedu.cn

Java: resp.statusCode()
来源：http://oq.szsharing.cn

Go:   resp.StatusCode
来源：http://tp.huixiangedu.cn

Ruby: resp.code.to_i
来源：http://cy.nicolike.cn

C#:   (int)resp.StatusCode
来源：http://nu.hahajie.cn

[L08] 并发请求多个地址
来源：http://be.wgjwhj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ii.asd995.cn

PHP:  curl_multi_init() 系列
来源：http://lu.hahajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aa.newstarts.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ub.hahajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jr.chemitech.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qy.hnjuh.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://di.hahajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fj.szsharing.cn

================================================================================
来源：http://bp.szxytkj.cn

M. 命令行 / 进程 / 环境
来源：http://up.bjjhwx.cn

================================================================================
来源：http://wf.huixinmuqiang.cn

[M01] 读取命令行参数
来源：http://id.chemitech.net.cn

Py:   sys.argv[1:]
来源：http://kd.yuntaijiaju.cn

PHP:  $argv;  $argc;
来源：http://cx.panjiajie.cn

JS:   process.argv.slice(2)
来源：http://vo.yuexingan06.cn

TS:   process.argv.slice(2)
来源：http://qk.nicolike.cn

Java: args 数组（main 方法参数）
来源：http://fv.wgjwhj.cn

Go:   os.Args[1:]
来源：http://wm.muxihuayi.cn

Ruby: ARGV
来源：http://tl.yuexingan06.cn

C#:   args 数组（Main 方法参数）
来源：http://cm.nicolike.cn

[M02] 读取环境变量
来源：http://wx.yuntaijiaju.cn

Py:   os.environ.get("HOME")
来源：http://zh.huixinmuqiang.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vq.lnxyls.cn

JS:   process.env.HOME
来源：http://uy.colortex.cn

TS:   process.env.HOME
来源：http://oj.newstarts.cn

Java: System.getenv("HOME")
来源：http://lr.wgjwhj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bb.hahajie.cn

Ruby: ENV["HOME"]
来源：http://vj.shxzukj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fc.muxihuayi.cn

[M03] 执行外部命令
来源：http://et.huixinmuqiang.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hs.huixinmuqiang.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zw.hnjuh.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://rw.haigaiapp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://je.lnxyls.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vw.szxytkj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xg.huanxung.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rq.shxzskj.cn

C#:   Process.Start("ls", "-l");
来源：http://fw.wgjwhj.cn

[M04] 获取当前工作目录
来源：http://vw.jianghongdianzi.cn

Py:   os.getcwd()
来源：http://ow.muxihuayi.cn

PHP:  getcwd();
来源：http://nx.asd995.cn

JS:   process.cwd()
来源：http://ff.asd995.cn

TS:   process.cwd()
来源：http://td.shxzukj.cn

Java: Path.of("").toAbsolutePath()
来源：http://gt.huixiangedu.cn

Go:   os.Getwd()
来源：http://px.nicolike.cn

Ruby: Dir.pwd
来源：http://jf.bjjhwx.cn

C#:   Directory.GetCurrentDirectory()
来源：http://um.szxytkj.cn

[M05] 设置退出码
来源：http://fe.szxytkj.cn

Py:   sys.exit(1)
来源：http://wq.huanxung.cn

PHP:  exit(1);
来源：http://vq.gzmigu.cn

JS:   process.exit(1)
来源：http://tb.huixinmuqiang.cn

TS:   process.exit(1)
来源：http://ag.newstarts.cn

Java: System.exit(1)
来源：http://gl.521024.cn

Go:   os.Exit(1)
来源：http://xj.shxzukj.cn

Ruby: exit 1
来源：http://td.jctech888.com.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hi.huixinmuqiang.cn

[M06] 向标准错误输出
来源：http://gc.hnjuh.cn

Py:   print("err", file=sys.stderr)
来源：http://zk.shxzukj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ua.yuexingan06.cn

JS:   console.error("err")
来源：http://vt.lnxyls.cn

TS:   console.error("err")
来源：http://yu.shxzukj.cn

Java: System.err.println("err")
来源：http://ui.gzmigu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ob.shtwfgs.cn

Ruby: warn "err"
来源：http://mg.huixiangedu.cn

C#:   Console.Error.WriteLine("err")
来源：http://ss.jctech888.com.cn

[M07] 判断是否为主入口
来源：http://ue.shtwfgs.cn

Py:   if __name__ == "__main__":
来源：http://my.jctech888.com.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uq.huanxung.cn

JS:   require.main === module
来源：http://bl.szsharing.cn

TS:   require.main === module
来源：http://gs.nszjky.cn

Java: public static void main(String[] args)
来源：http://ph.wgjwhj.cn

Go:   func main()
来源：http://cd.newstarts.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zx.jctech888.com.cn

C#:   static void Main(string[] args)
来源：http://pw.newstarts.cn

[M08] 获取系统与运行时信息
来源：http://df.gzmigu.cn

Py:   platform.system();  platform.python_version()
来源：http://bo.panjiajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://eh.521024.cn

JS:   process.platform;  process.version
来源：http://pl.bookmarksfly.cn

TS:   process.platform;  process.version
来源：http://cy.shxzskj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yr.szxytkj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gi.muxihuayi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jn.bjjhwx.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://lv.521024.cn

================================================================================
来源：http://sf.gzmigu.cn

N. 数据结构与算法
来源：http://pn.lnxyls.cn

================================================================================
来源：http://bu.newstarts.cn


<!-- 参考信息 -->