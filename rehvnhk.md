代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ll.haigaiapp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yf.yuntaijiaju.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://go.yuntaijiaju.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rk.colortex.cn

[J03] 字符串解析为日期
来源：http://lz.9csxet.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uz.shtwfgs.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tk.bjjhwx.cn

JS:   new Date("2024-01-02")
来源：http://mn.gzmigu.cn

TS:   new Date("2024-01-02")
来源：http://xy.bookmarksfly.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ob.asd995.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://re.jctech888.com.cn

Ruby: Date.parse("2024-01-02")
来源：http://hm.huixinmuqiang.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ks.nszjky.cn

[J04] 时间戳与日期互转
来源：http://cl.yuntaijiaju.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ev.hahajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hn.shxzskj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fa.szxytkj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://rf.gzmigu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wd.nszjky.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vi.yuntaijiaju.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zz.hnjuh.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hb.shxzukj.cn

[J05] 时间加减（加 7 天）
来源：http://lg.bjjhwx.cn

Py:   now + timedelta(days=7)
来源：http://rq.haigaiapp.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sf.jianghongdianzi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jr.asd995.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zt.newstarts.cn

Java: LocalDate.now().plusDays(7)
来源：http://cp.9csxet.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sx.jctech888.com.cn

Ruby: Time.now + 7 * 86400
来源：http://nu.nicolike.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xd.colortex.cn

[J06] 计算两时间之差
来源：http://mv.shtwfgs.cn

Py:   (end - start).total_seconds()
来源：http://xe.hnjuh.cn

PHP:  $end->diff($start)->days;
来源：http://po.jianghongdianzi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://aq.huixinmuqiang.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yb.yuntaijiaju.cn

Java: Duration.between(start, end).toSeconds()
来源：http://kr.jctech888.com.cn

Go:   end.Sub(start).Hours()
来源：http://fc.nszjky.cn

Ruby: end - start                 # 返回秒数
来源：http://zh.shtwfgs.cn

C#:   (end - start).TotalSeconds
来源：http://se.panjiajie.cn

[J07] 比较两个日期
来源：http://lv.521024.cn

Py:   d1 < d2;  d1 == d2
来源：http://gx.9csxet.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wt.jianghongdianzi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://nl.shxzskj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://wd.nszjky.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fs.shxzskj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mj.panjiajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ht.hahajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://ex.colortex.cn

[J08] 提取年月日与星期
来源：http://sl.newstarts.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lw.chemitech.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sr.wgjwhj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ps.shxzukj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://il.hnjuh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ms.hnjuh.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ut.yuexingan06.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sg.haigaiapp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://al.haigaiapp.cn

[J09] 时区处理
来源：http://lu.bjjhwx.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://am.haigaiapp.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ur.yuexingan06.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sy.wgjwhj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://we.gzmigu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sh.newstarts.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vd.yuntaijiaju.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wm.asd995.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bj.muxihuayi.cn

[J10] 取今天 / 本月第一天
来源：http://qo.szsharing.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ky.jctech888.com.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ol.haigaiapp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tl.newstarts.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cf.newstarts.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ye.panjiajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vx.panjiajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rb.hnjuh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ma.yuexingan06.cn

================================================================================
来源：http://cy.nicolike.cn

K. JSON 与序列化
来源：http://xz.colortex.cn

================================================================================
来源：http://oi.panjiajie.cn

[K01] 对象转 JSON 字符串
来源：http://vt.shxzukj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jj.9csxet.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dp.colortex.cn

JS:   JSON.stringify(obj)
来源：http://rh.nszjky.cn

TS:   JSON.stringify(obj)
来源：http://xv.jctech888.com.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qa.bjjhwx.cn

Go:   json.Marshal(obj)
来源：http://oc.wgjwhj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://pg.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vv.9csxet.cn

[K02] JSON 字符串转对象
来源：http://ed.jctech888.com.cn

Py:   json.loads(s)
来源：http://hy.shtwfgs.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pq.haigaiapp.cn

JS:   JSON.parse(s)
来源：http://rz.asd995.cn

TS:   JSON.parse(s)
来源：http://ku.haigaiapp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bv.wgjwhj.cn

Go:   json.Unmarshal(data, &v)
来源：http://ls.nszjky.cn

Ruby: JSON.parse(s)
来源：http://ob.hnjuh.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mu.shxzskj.cn

[K03] JSON 美化输出（带缩进）
来源：http://uj.bookmarksfly.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ws.colortex.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ci.huixinmuqiang.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qy.gzmigu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wp.chemitech.net.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nu.wgjwhj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pm.szsharing.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qg.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lr.yuexingan06.cn

[K04] 读取 JSON 文件
来源：http://mg.newstarts.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://el.newstarts.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fx.shxzukj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ur.hnjuh.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dq.jianghongdianzi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cj.hahajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gx.nicolike.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ar.521024.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qe.nicolike.cn

[K05] 深拷贝对象
来源：http://ry.huixiangedu.cn

Py:   copy.deepcopy(obj)
来源：http://ae.wgjwhj.cn

PHP:  unserialize(serialize($obj));
来源：http://hl.nszjky.cn

JS:   structuredClone(obj)
来源：http://zh.huixinmuqiang.cn

TS:   structuredClone(obj)
来源：http://tx.colortex.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://al.newstarts.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ad.asd995.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jo.huixiangedu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://bi.nszjky.cn

[K06] 解析 URL 查询串
来源：http://ip.newstarts.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jb.szxytkj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://de.szxytkj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ql.muxihuayi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oz.huanxung.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xq.yuexingan06.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://le.bjjhwx.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ft.hahajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tp.wgjwhj.cn

[K07] 进制转换
来源：http://ft.hahajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pe.huanxung.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cr.bjjhwx.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://up.521024.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wk.huixiangedu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vp.gzmigu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yv.huixiangedu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jt.bookmarksfly.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kn.gzmigu.cn

[K08] 二进制序列化（非 JSON）
来源：http://mw.lnxyls.cn

Py:   pickle.dumps(obj)
来源：http://nj.nicolike.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zs.hnjuh.cn

JS:   v8.serialize(obj)        // Node
来源：http://cc.panjiajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://rw.9csxet.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qg.wgjwhj.cn

Go:   encoding/gob
来源：http://kx.huixiangedu.cn

Ruby: Marshal.dump(obj)
来源：http://eo.asd995.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tn.bjjhwx.cn

================================================================================
来源：http://mm.szsharing.cn

L. 网络请求
来源：http://ij.yuexingan06.cn

================================================================================
来源：http://ke.hahajie.cn

[L01] 发送 GET 请求
来源：http://wj.gzmigu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://iu.jianghongdianzi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://se.szxytkj.cn

JS:   await fetch(url)
来源：http://zt.9csxet.cn

TS:   await fetch(url)
来源：http://pf.wgjwhj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yv.hnjuh.cn

Go:   resp, err := http.Get(url)
来源：http://eb.hahajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qi.panjiajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://iy.shxzskj.cn

[L02] 发送 POST JSON
来源：http://yx.hahajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nq.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cq.jianghongdianzi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vy.muxihuayi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xp.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ym.shxzskj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qi.hahajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kc.panjiajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tr.chemitech.net.cn

[L03] 设置自定义请求头
来源：http://ab.muxihuayi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zo.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qs.hahajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qh.shtwfgs.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vm.colortex.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ry.bookmarksfly.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ka.shxzukj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nn.huanxung.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sr.haigaiapp.cn

[L04] 设置超时
来源：http://ls.huanxung.cn

Py:   requests.get(url, timeout=5)
来源：http://yp.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kf.haigaiapp.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://et.nszjky.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cz.nicolike.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fc.521024.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://iw.yuexingan06.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dg.nicolike.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xh.asd995.cn

[L05] 上传文件（multipart）
来源：http://fn.wgjwhj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sv.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gr.hnjuh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rz.huanxung.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ic.colortex.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ud.521024.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bn.asd995.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ai.chemitech.net.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kd.colortex.cn

[L06] 解析响应为 JSON
来源：http://gu.bookmarksfly.cn

Py:   resp.json()
来源：http://cb.hnjuh.cn

PHP:  json_decode($body, true);
来源：http://es.shxzukj.cn

JS:   await resp.json()
来源：http://by.szsharing.cn

TS:   await resp.json()
来源：http://sg.bookmarksfly.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hm.521024.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ju.muxihuayi.cn

Ruby: JSON.parse(resp.body)
来源：http://ep.haigaiapp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qy.jctech888.com.cn

[L07] 处理 HTTP 状态码
来源：http://ie.521024.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://av.panjiajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://su.nicolike.cn

JS:   resp.ok;  resp.status
来源：http://vh.haigaiapp.cn

TS:   resp.ok;  resp.status
来源：http://jp.chemitech.net.cn

Java: resp.statusCode()
来源：http://mk.bookmarksfly.cn

Go:   resp.StatusCode
来源：http://xj.hahajie.cn

Ruby: resp.code.to_i
来源：http://hw.szsharing.cn

C#:   (int)resp.StatusCode
来源：http://yi.shxzukj.cn

[L08] 并发请求多个地址
来源：http://xi.szxytkj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://oj.colortex.cn

PHP:  curl_multi_init() 系列
来源：http://fm.bookmarksfly.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fu.bookmarksfly.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gi.bjjhwx.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rs.nszjky.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dd.jianghongdianzi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://db.chemitech.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nw.huixiangedu.cn

================================================================================
来源：http://cp.nszjky.cn

M. 命令行 / 进程 / 环境
来源：http://gk.jctech888.com.cn

================================================================================
来源：http://lm.panjiajie.cn

[M01] 读取命令行参数
来源：http://co.nicolike.cn

Py:   sys.argv[1:]
来源：http://ay.shxzskj.cn

PHP:  $argv;  $argc;
来源：http://kx.521024.cn

JS:   process.argv.slice(2)
来源：http://fl.panjiajie.cn

TS:   process.argv.slice(2)
来源：http://gg.nicolike.cn

Java: args 数组（main 方法参数）
来源：http://aj.hnjuh.cn

Go:   os.Args[1:]
来源：http://rh.shxzskj.cn

Ruby: ARGV
来源：http://ag.colortex.cn

C#:   args 数组（Main 方法参数）
来源：http://da.szsharing.cn

[M02] 读取环境变量
来源：http://ak.shtwfgs.cn

Py:   os.environ.get("HOME")
来源：http://ld.jianghongdianzi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cz.chemitech.net.cn

JS:   process.env.HOME
来源：http://me.bjjhwx.cn

TS:   process.env.HOME
来源：http://dx.nicolike.cn

Java: System.getenv("HOME")
来源：http://ya.shtwfgs.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://on.huixinmuqiang.cn

Ruby: ENV["HOME"]
来源：http://kf.hnjuh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hv.panjiajie.cn

[M03] 执行外部命令
来源：http://uj.hnjuh.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gq.huixiangedu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://np.gzmigu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ji.huanxung.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rg.jianghongdianzi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kg.hnjuh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mg.huixinmuqiang.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yn.nszjky.cn

C#:   Process.Start("ls", "-l");
来源：http://ng.huixinmuqiang.cn

[M04] 获取当前工作目录
来源：http://me.hahajie.cn

Py:   os.getcwd()
来源：http://oh.jctech888.com.cn

PHP:  getcwd();
来源：http://nw.haigaiapp.cn

JS:   process.cwd()
来源：http://tb.colortex.cn

TS:   process.cwd()
来源：http://on.nszjky.cn

Java: Path.of("").toAbsolutePath()
来源：http://sc.muxihuayi.cn

Go:   os.Getwd()
来源：http://su.huixinmuqiang.cn

Ruby: Dir.pwd
来源：http://wk.haigaiapp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://bm.haigaiapp.cn

[M05] 设置退出码
来源：http://xn.yuntaijiaju.cn

Py:   sys.exit(1)
来源：http://xo.shtwfgs.cn

PHP:  exit(1);
来源：http://bo.szsharing.cn

JS:   process.exit(1)
来源：http://ss.shxzukj.cn

TS:   process.exit(1)
来源：http://hs.lnxyls.cn

Java: System.exit(1)
来源：http://wj.wgjwhj.cn

Go:   os.Exit(1)
来源：http://dt.chemitech.net.cn

Ruby: exit 1
来源：http://nx.asd995.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ez.gzmigu.cn

[M06] 向标准错误输出
来源：http://ih.hnjuh.cn

Py:   print("err", file=sys.stderr)
来源：http://mb.bookmarksfly.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lq.huixiangedu.cn

JS:   console.error("err")
来源：http://fr.yuntaijiaju.cn

TS:   console.error("err")
来源：http://dm.shxzukj.cn

Java: System.err.println("err")
来源：http://ci.9csxet.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qo.yuexingan06.cn

Ruby: warn "err"
来源：http://xa.huanxung.cn

C#:   Console.Error.WriteLine("err")
来源：http://jp.newstarts.cn

[M07] 判断是否为主入口
来源：http://pf.shxzukj.cn

Py:   if __name__ == "__main__":
来源：http://un.nszjky.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hh.hnjuh.cn

JS:   require.main === module
来源：http://md.muxihuayi.cn

TS:   require.main === module
来源：http://pj.huanxung.cn

Java: public static void main(String[] args)
来源：http://vh.bjjhwx.cn

Go:   func main()
来源：http://jf.huixinmuqiang.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://uw.panjiajie.cn

C#:   static void Main(string[] args)
来源：http://rt.newstarts.cn

[M08] 获取系统与运行时信息
来源：http://hz.bookmarksfly.cn

Py:   platform.system();  platform.python_version()
来源：http://bl.szsharing.cn

PHP:  PHP_OS;  phpversion();
来源：http://at.szsharing.cn

JS:   process.platform;  process.version
来源：http://fe.hahajie.cn

TS:   process.platform;  process.version
来源：http://dm.haigaiapp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jc.lnxyls.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://je.szsharing.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gv.nszjky.cn


<!-- 参考信息 -->