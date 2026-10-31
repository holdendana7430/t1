代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ag.panjiajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rm.hnjuh.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qz.chemitech.net.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rs.shxzukj.cn

[J03] 字符串解析为日期
来源：http://zp.wgjwhj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bf.yuntaijiaju.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fg.asd995.cn

JS:   new Date("2024-01-02")
来源：http://kf.shxzukj.cn

TS:   new Date("2024-01-02")
来源：http://wb.asd995.cn

Java: LocalDate.parse("2024-01-02")
来源：http://le.asd995.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ie.szxytkj.cn

Ruby: Date.parse("2024-01-02")
来源：http://gq.shxzukj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pn.colortex.cn

[J04] 时间戳与日期互转
来源：http://nq.lnxyls.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qf.lnxyls.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hh.wgjwhj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ib.nszjky.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ug.szsharing.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ts.szsharing.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://my.haigaiapp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dq.nszjky.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gn.jctech888.com.cn

[J05] 时间加减（加 7 天）
来源：http://xm.gzmigu.cn

Py:   now + timedelta(days=7)
来源：http://wa.jctech888.com.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yo.huanxung.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dy.huixinmuqiang.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wm.hahajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://he.bjjhwx.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://js.521024.cn

Ruby: Time.now + 7 * 86400
来源：http://gr.panjiajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ej.hahajie.cn

[J06] 计算两时间之差
来源：http://ln.9csxet.cn

Py:   (end - start).total_seconds()
来源：http://ee.muxihuayi.cn

PHP:  $end->diff($start)->days;
来源：http://gu.yuntaijiaju.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sa.szxytkj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bj.yuntaijiaju.cn

Java: Duration.between(start, end).toSeconds()
来源：http://uu.szxytkj.cn

Go:   end.Sub(start).Hours()
来源：http://nr.shxzukj.cn

Ruby: end - start                 # 返回秒数
来源：http://ps.bjjhwx.cn

C#:   (end - start).TotalSeconds
来源：http://qq.shxzskj.cn

[J07] 比较两个日期
来源：http://ya.newstarts.cn

Py:   d1 < d2;  d1 == d2
来源：http://hu.hahajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zs.szsharing.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ts.szsharing.cn

TS:   d1.getTime() < d2.getTime()
来源：http://sa.bookmarksfly.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dd.shtwfgs.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ub.jianghongdianzi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://dg.nszjky.cn

C#:   d1 < d2;  d1 == d2
来源：http://ju.asd995.cn

[J08] 提取年月日与星期
来源：http://ab.hnjuh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cj.shtwfgs.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yd.haigaiapp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yd.yuexingan06.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pn.asd995.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dn.nicolike.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kk.521024.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mo.jianghongdianzi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vz.lnxyls.cn

[J09] 时区处理
来源：http://yv.bookmarksfly.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nn.nicolike.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yw.jctech888.com.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iy.colortex.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jf.huixiangedu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zj.newstarts.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qb.wgjwhj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://sj.lnxyls.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ne.huixiangedu.cn

[J10] 取今天 / 本月第一天
来源：http://ki.haigaiapp.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://oi.jianghongdianzi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://px.nszjky.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tr.bjjhwx.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hw.asd995.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fn.nszjky.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gl.nszjky.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gf.chemitech.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://me.szxytkj.cn

================================================================================
来源：http://rd.shxzukj.cn

K. JSON 与序列化
来源：http://dj.wgjwhj.cn

================================================================================
来源：http://ju.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://jo.yuntaijiaju.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tz.lnxyls.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qg.haigaiapp.cn

JS:   JSON.stringify(obj)
来源：http://ze.szxytkj.cn

TS:   JSON.stringify(obj)
来源：http://mj.wgjwhj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kp.huixinmuqiang.cn

Go:   json.Marshal(obj)
来源：http://rf.huixiangedu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://kx.szxytkj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yz.colortex.cn

[K02] JSON 字符串转对象
来源：http://vs.hahajie.cn

Py:   json.loads(s)
来源：http://xk.9csxet.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ci.shxzskj.cn

JS:   JSON.parse(s)
来源：http://xc.chemitech.net.cn

TS:   JSON.parse(s)
来源：http://yx.huixinmuqiang.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qy.hahajie.cn

Go:   json.Unmarshal(data, &v)
来源：http://gz.asd995.cn

Ruby: JSON.parse(s)
来源：http://aj.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qz.yuntaijiaju.cn

[K03] JSON 美化输出（带缩进）
来源：http://sw.wgjwhj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cy.bookmarksfly.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wd.panjiajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bx.szsharing.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://su.shxzukj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pf.huixiangedu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gz.szsharing.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ly.gzmigu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://os.yuexingan06.cn

[K04] 读取 JSON 文件
来源：http://cf.gzmigu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uf.bjjhwx.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://el.9csxet.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oy.521024.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mp.yuntaijiaju.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rl.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jw.9csxet.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://lc.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xq.shxzukj.cn

[K05] 深拷贝对象
来源：http://np.jianghongdianzi.cn

Py:   copy.deepcopy(obj)
来源：http://ao.jctech888.com.cn

PHP:  unserialize(serialize($obj));
来源：http://ui.shtwfgs.cn

JS:   structuredClone(obj)
来源：http://hj.jianghongdianzi.cn

TS:   structuredClone(obj)
来源：http://pm.huixiangedu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xt.9csxet.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xe.colortex.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://aw.shtwfgs.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ib.haigaiapp.cn

[K06] 解析 URL 查询串
来源：http://yh.shtwfgs.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ag.hnjuh.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jl.shxzukj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mg.colortex.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://df.asd995.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lp.jctech888.com.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cj.haigaiapp.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cm.jctech888.com.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cf.huixinmuqiang.cn

[K07] 进制转换
来源：http://es.muxihuayi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vj.huixiangedu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mq.jianghongdianzi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hj.shxzukj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wr.shxzskj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wv.huixiangedu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uo.shxzukj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ti.jianghongdianzi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xj.nicolike.cn

[K08] 二进制序列化（非 JSON）
来源：http://qe.nicolike.cn

Py:   pickle.dumps(obj)
来源：http://wi.newstarts.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ia.bookmarksfly.cn

JS:   v8.serialize(obj)        // Node
来源：http://zj.muxihuayi.cn

TS:   v8.serialize(obj)        // Node
来源：http://ns.bookmarksfly.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://in.hnjuh.cn

Go:   encoding/gob
来源：http://qa.jianghongdianzi.cn

Ruby: Marshal.dump(obj)
来源：http://nq.yuntaijiaju.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ej.szxytkj.cn

================================================================================
来源：http://nx.panjiajie.cn

L. 网络请求
来源：http://os.bookmarksfly.cn

================================================================================
来源：http://bg.yuntaijiaju.cn

[L01] 发送 GET 请求
来源：http://ok.jctech888.com.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cv.gzmigu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yw.asd995.cn

JS:   await fetch(url)
来源：http://gy.nszjky.cn

TS:   await fetch(url)
来源：http://pt.wgjwhj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bn.huixiangedu.cn

Go:   resp, err := http.Get(url)
来源：http://ch.nszjky.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://tv.yuntaijiaju.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pe.nszjky.cn

[L02] 发送 POST JSON
来源：http://hj.chemitech.net.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nr.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rt.nszjky.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ye.huixinmuqiang.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yl.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vh.asd995.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wp.newstarts.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jk.bookmarksfly.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pc.yuntaijiaju.cn

[L03] 设置自定义请求头
来源：http://nf.nicolike.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qt.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bc.asd995.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vu.lnxyls.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bz.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nw.szxytkj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://le.hahajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xz.huixiangedu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cs.shtwfgs.cn

[L04] 设置超时
来源：http://we.haigaiapp.cn

Py:   requests.get(url, timeout=5)
来源：http://nb.521024.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ul.bookmarksfly.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ht.huanxung.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ib.huixiangedu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pm.yuexingan06.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xv.asd995.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://te.muxihuayi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lm.panjiajie.cn

[L05] 上传文件（multipart）
来源：http://ts.shxzukj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ns.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://oy.muxihuayi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rx.nszjky.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sr.chemitech.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ua.haigaiapp.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://eh.hnjuh.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ya.hnjuh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yy.bjjhwx.cn

[L06] 解析响应为 JSON
来源：http://ld.colortex.cn

Py:   resp.json()
来源：http://tu.hnjuh.cn

PHP:  json_decode($body, true);
来源：http://qg.bookmarksfly.cn

JS:   await resp.json()
来源：http://rp.newstarts.cn

TS:   await resp.json()
来源：http://os.hnjuh.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nt.huixinmuqiang.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ec.nszjky.cn

Ruby: JSON.parse(resp.body)
来源：http://aq.lnxyls.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yo.huanxung.cn

[L07] 处理 HTTP 状态码
来源：http://zc.asd995.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ou.jianghongdianzi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lb.jctech888.com.cn

JS:   resp.ok;  resp.status
来源：http://ei.bjjhwx.cn

TS:   resp.ok;  resp.status
来源：http://yg.9csxet.cn

Java: resp.statusCode()
来源：http://ci.9csxet.cn

Go:   resp.StatusCode
来源：http://ry.yuntaijiaju.cn

Ruby: resp.code.to_i
来源：http://fl.asd995.cn

C#:   (int)resp.StatusCode
来源：http://mb.newstarts.cn

[L08] 并发请求多个地址
来源：http://lw.jianghongdianzi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ue.gzmigu.cn

PHP:  curl_multi_init() 系列
来源：http://oc.shxzskj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ca.huixinmuqiang.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jq.yuexingan06.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zx.newstarts.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ub.colortex.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ss.muxihuayi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cj.huixinmuqiang.cn

================================================================================
来源：http://ws.asd995.cn

M. 命令行 / 进程 / 环境
来源：http://qy.szxytkj.cn

================================================================================
来源：http://nn.lnxyls.cn

[M01] 读取命令行参数
来源：http://dk.yuexingan06.cn

Py:   sys.argv[1:]
来源：http://gt.9csxet.cn

PHP:  $argv;  $argc;
来源：http://yg.521024.cn

JS:   process.argv.slice(2)
来源：http://hc.haigaiapp.cn

TS:   process.argv.slice(2)
来源：http://yh.szxytkj.cn

Java: args 数组（main 方法参数）
来源：http://uy.nicolike.cn

Go:   os.Args[1:]
来源：http://hy.shxzskj.cn

Ruby: ARGV
来源：http://mk.nszjky.cn

C#:   args 数组（Main 方法参数）
来源：http://wn.colortex.cn

[M02] 读取环境变量
来源：http://mp.nicolike.cn

Py:   os.environ.get("HOME")
来源：http://ad.panjiajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jr.newstarts.cn

JS:   process.env.HOME
来源：http://mj.bjjhwx.cn

TS:   process.env.HOME
来源：http://qv.colortex.cn

Java: System.getenv("HOME")
来源：http://bd.jctech888.com.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ex.521024.cn

Ruby: ENV["HOME"]
来源：http://lv.hnjuh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wk.521024.cn

[M03] 执行外部命令
来源：http://gd.panjiajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gp.haigaiapp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gk.hahajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://at.panjiajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qf.panjiajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qw.chemitech.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wi.jctech888.com.cn

Ruby: system("ls -l");  `ls -l`
来源：http://oj.huixinmuqiang.cn

C#:   Process.Start("ls", "-l");
来源：http://ym.panjiajie.cn

[M04] 获取当前工作目录
来源：http://rr.yuntaijiaju.cn

Py:   os.getcwd()
来源：http://wf.szsharing.cn

PHP:  getcwd();
来源：http://fb.521024.cn

JS:   process.cwd()
来源：http://ro.hahajie.cn

TS:   process.cwd()
来源：http://jh.newstarts.cn

Java: Path.of("").toAbsolutePath()
来源：http://cz.9csxet.cn

Go:   os.Getwd()
来源：http://yp.9csxet.cn

Ruby: Dir.pwd
来源：http://ck.521024.cn

C#:   Directory.GetCurrentDirectory()
来源：http://cw.asd995.cn

[M05] 设置退出码
来源：http://yq.jianghongdianzi.cn

Py:   sys.exit(1)
来源：http://da.shxzskj.cn

PHP:  exit(1);
来源：http://xe.gzmigu.cn

JS:   process.exit(1)
来源：http://of.hnjuh.cn

TS:   process.exit(1)
来源：http://ho.szxytkj.cn

Java: System.exit(1)
来源：http://ql.huixinmuqiang.cn

Go:   os.Exit(1)
来源：http://sa.panjiajie.cn

Ruby: exit 1
来源：http://et.szsharing.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ui.huanxung.cn

[M06] 向标准错误输出
来源：http://bt.asd995.cn

Py:   print("err", file=sys.stderr)
来源：http://ho.yuexingan06.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jq.muxihuayi.cn

JS:   console.error("err")
来源：http://np.bjjhwx.cn

TS:   console.error("err")
来源：http://au.muxihuayi.cn

Java: System.err.println("err")
来源：http://ou.hahajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bg.newstarts.cn

Ruby: warn "err"
来源：http://se.asd995.cn

C#:   Console.Error.WriteLine("err")
来源：http://py.huixinmuqiang.cn

[M07] 判断是否为主入口
来源：http://pe.hahajie.cn

Py:   if __name__ == "__main__":
来源：http://ma.newstarts.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gm.huanxung.cn

JS:   require.main === module
来源：http://zg.shxzukj.cn

TS:   require.main === module
来源：http://bn.gzmigu.cn

Java: public static void main(String[] args)
来源：http://gn.newstarts.cn

Go:   func main()
来源：http://xa.haigaiapp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cn.colortex.cn

C#:   static void Main(string[] args)
来源：http://ja.huixinmuqiang.cn

[M08] 获取系统与运行时信息
来源：http://xx.jctech888.com.cn

Py:   platform.system();  platform.python_version()
来源：http://mn.521024.cn

PHP:  PHP_OS;  phpversion();
来源：http://hm.hahajie.cn

JS:   process.platform;  process.version
来源：http://tz.shtwfgs.cn

TS:   process.platform;  process.version
来源：http://oj.jianghongdianzi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://py.lnxyls.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://rz.9csxet.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gz.haigaiapp.cn


<!-- 参考信息 -->