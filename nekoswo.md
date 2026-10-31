代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://re.szsharing.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ie.asd995.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wt.bjjhwx.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wa.gzmigu.cn

[J03] 字符串解析为日期
来源：http://hb.szxytkj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wn.nszjky.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ro.shxzukj.cn

JS:   new Date("2024-01-02")
来源：http://dq.huixiangedu.cn

TS:   new Date("2024-01-02")
来源：http://nf.szsharing.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cx.bookmarksfly.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://eu.asd995.cn

Ruby: Date.parse("2024-01-02")
来源：http://mz.huanxung.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qd.gzmigu.cn

[J04] 时间戳与日期互转
来源：http://wx.colortex.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pp.nicolike.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fn.bookmarksfly.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://os.jianghongdianzi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ty.asd995.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vi.shxzskj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ve.newstarts.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jy.haigaiapp.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cl.haigaiapp.cn

[J05] 时间加减（加 7 天）
来源：http://fn.521024.cn

Py:   now + timedelta(days=7)
来源：http://hp.wgjwhj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://he.asd995.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qn.hahajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fl.jctech888.com.cn

Java: LocalDate.now().plusDays(7)
来源：http://bs.bookmarksfly.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lc.asd995.cn

Ruby: Time.now + 7 * 86400
来源：http://un.shxzukj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rm.bookmarksfly.cn

[J06] 计算两时间之差
来源：http://ql.huanxung.cn

Py:   (end - start).total_seconds()
来源：http://ar.asd995.cn

PHP:  $end->diff($start)->days;
来源：http://mw.gzmigu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wm.colortex.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qy.nszjky.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rp.szxytkj.cn

Go:   end.Sub(start).Hours()
来源：http://uk.jctech888.com.cn

Ruby: end - start                 # 返回秒数
来源：http://el.shtwfgs.cn

C#:   (end - start).TotalSeconds
来源：http://iw.jianghongdianzi.cn

[J07] 比较两个日期
来源：http://uv.szxytkj.cn

Py:   d1 < d2;  d1 == d2
来源：http://wn.szsharing.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://it.huixiangedu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://cj.yuntaijiaju.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ns.lnxyls.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://at.muxihuayi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nf.newstarts.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fj.bjjhwx.cn

C#:   d1 < d2;  d1 == d2
来源：http://rc.asd995.cn

[J08] 提取年月日与星期
来源：http://rc.shtwfgs.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ga.haigaiapp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ca.9csxet.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bh.bjjhwx.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ks.hnjuh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hl.szsharing.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qk.lnxyls.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qi.huixiangedu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ud.newstarts.cn

[J09] 时区处理
来源：http://qn.521024.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fv.haigaiapp.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hu.yuexingan06.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aj.jianghongdianzi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qg.hahajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ka.asd995.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kt.hnjuh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://nx.bookmarksfly.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vf.muxihuayi.cn

[J10] 取今天 / 本月第一天
来源：http://bj.shxzskj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jw.chemitech.net.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wk.gzmigu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vd.nszjky.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://oq.jctech888.com.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qh.huixiangedu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ee.jianghongdianzi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mt.huixiangedu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zv.jctech888.com.cn

================================================================================
来源：http://xf.huixinmuqiang.cn

K. JSON 与序列化
来源：http://gf.panjiajie.cn

================================================================================
来源：http://jz.yuexingan06.cn

[K01] 对象转 JSON 字符串
来源：http://oc.521024.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fp.szxytkj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ed.nszjky.cn

JS:   JSON.stringify(obj)
来源：http://sc.nszjky.cn

TS:   JSON.stringify(obj)
来源：http://vz.bjjhwx.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fz.shxzskj.cn

Go:   json.Marshal(obj)
来源：http://vz.newstarts.cn

Ruby: obj.to_json                                     // require "json"
来源：http://pa.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lo.9csxet.cn

[K02] JSON 字符串转对象
来源：http://gz.bjjhwx.cn

Py:   json.loads(s)
来源：http://vs.shxzukj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nx.yuexingan06.cn

JS:   JSON.parse(s)
来源：http://vn.huixiangedu.cn

TS:   JSON.parse(s)
来源：http://eg.szsharing.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cf.yuexingan06.cn

Go:   json.Unmarshal(data, &v)
来源：http://qj.nicolike.cn

Ruby: JSON.parse(s)
来源：http://te.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kj.huixinmuqiang.cn

[K03] JSON 美化输出（带缩进）
来源：http://lg.yuexingan06.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qy.szxytkj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://la.yuexingan06.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://aj.huixiangedu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ul.haigaiapp.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://se.chemitech.net.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dd.huanxung.cn

Ruby: JSON.pretty_generate(obj)
来源：http://np.shxzskj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tz.szxytkj.cn

[K04] 读取 JSON 文件
来源：http://gw.chemitech.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ae.chemitech.net.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nd.asd995.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ls.shtwfgs.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lk.colortex.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pg.asd995.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cn.muxihuayi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zj.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gc.szxytkj.cn

[K05] 深拷贝对象
来源：http://wd.wgjwhj.cn

Py:   copy.deepcopy(obj)
来源：http://wv.haigaiapp.cn

PHP:  unserialize(serialize($obj));
来源：http://vu.hahajie.cn

JS:   structuredClone(obj)
来源：http://fp.hahajie.cn

TS:   structuredClone(obj)
来源：http://al.asd995.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gq.huixiangedu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://th.jianghongdianzi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jf.shxzukj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mb.muxihuayi.cn

[K06] 解析 URL 查询串
来源：http://dq.hahajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ag.newstarts.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qb.bjjhwx.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wt.colortex.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pj.521024.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dt.chemitech.net.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://kl.yuntaijiaju.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://iw.wgjwhj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pb.newstarts.cn

[K07] 进制转换
来源：http://ae.hahajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://od.gzmigu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pg.lnxyls.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://aj.bjjhwx.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wv.nszjky.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ba.hahajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fb.panjiajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yd.gzmigu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://az.szsharing.cn

[K08] 二进制序列化（非 JSON）
来源：http://jt.hahajie.cn

Py:   pickle.dumps(obj)
来源：http://lw.colortex.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bh.wgjwhj.cn

JS:   v8.serialize(obj)        // Node
来源：http://nu.huanxung.cn

TS:   v8.serialize(obj)        // Node
来源：http://zw.jctech888.com.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xg.hnjuh.cn

Go:   encoding/gob
来源：http://rd.muxihuayi.cn

Ruby: Marshal.dump(obj)
来源：http://tw.yuntaijiaju.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xj.wgjwhj.cn

================================================================================
来源：http://ej.szxytkj.cn

L. 网络请求
来源：http://sa.yuntaijiaju.cn

================================================================================
来源：http://hw.bookmarksfly.cn

[L01] 发送 GET 请求
来源：http://bu.asd995.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wd.521024.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kh.yuexingan06.cn

JS:   await fetch(url)
来源：http://dp.huixinmuqiang.cn

TS:   await fetch(url)
来源：http://yg.panjiajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mp.asd995.cn

Go:   resp, err := http.Get(url)
来源：http://ot.shtwfgs.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://lm.huanxung.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zy.shxzukj.cn

[L02] 发送 POST JSON
来源：http://oy.nszjky.cn

Py:   requests.post(url, json={"a": 1})
来源：http://if.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wt.bookmarksfly.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jm.wgjwhj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uv.asd995.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rx.huanxung.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sj.hnjuh.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://us.huixiangedu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fr.lnxyls.cn

[L03] 设置自定义请求头
来源：http://hm.colortex.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xu.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fd.gzmigu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tc.szsharing.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ft.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cf.bjjhwx.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dr.chemitech.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ol.lnxyls.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wj.shxzukj.cn

[L04] 设置超时
来源：http://di.huixinmuqiang.cn

Py:   requests.get(url, timeout=5)
来源：http://xi.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://eh.panjiajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://je.szxytkj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dy.yuexingan06.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wz.jianghongdianzi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://je.yuexingan06.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zq.huixiangedu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jr.yuexingan06.cn

[L05] 上传文件（multipart）
来源：http://my.shxzukj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zq.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rt.gzmigu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xe.szsharing.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kb.wgjwhj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ln.chemitech.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qo.nicolike.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wv.huixiangedu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bm.panjiajie.cn

[L06] 解析响应为 JSON
来源：http://hj.shxzskj.cn

Py:   resp.json()
来源：http://tj.asd995.cn

PHP:  json_decode($body, true);
来源：http://bj.huixiangedu.cn

JS:   await resp.json()
来源：http://bb.newstarts.cn

TS:   await resp.json()
来源：http://pf.jianghongdianzi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://de.521024.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://aa.nszjky.cn

Ruby: JSON.parse(resp.body)
来源：http://kp.yuntaijiaju.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rx.chemitech.net.cn

[L07] 处理 HTTP 状态码
来源：http://gr.huixiangedu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jf.shtwfgs.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://by.lnxyls.cn

JS:   resp.ok;  resp.status
来源：http://hj.huixinmuqiang.cn

TS:   resp.ok;  resp.status
来源：http://mw.huixinmuqiang.cn

Java: resp.statusCode()
来源：http://tu.huixinmuqiang.cn

Go:   resp.StatusCode
来源：http://wc.jianghongdianzi.cn

Ruby: resp.code.to_i
来源：http://zw.nszjky.cn

C#:   (int)resp.StatusCode
来源：http://vt.yuexingan06.cn

[L08] 并发请求多个地址
来源：http://xm.hnjuh.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ey.panjiajie.cn

PHP:  curl_multi_init() 系列
来源：http://fl.haigaiapp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jd.chemitech.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cf.521024.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rj.hahajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zk.shxzskj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://en.shtwfgs.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qz.chemitech.net.cn

================================================================================
来源：http://nd.521024.cn

M. 命令行 / 进程 / 环境
来源：http://pc.yuexingan06.cn

================================================================================
来源：http://bq.chemitech.net.cn

[M01] 读取命令行参数
来源：http://bl.nicolike.cn

Py:   sys.argv[1:]
来源：http://sl.szsharing.cn

PHP:  $argv;  $argc;
来源：http://jj.lnxyls.cn

JS:   process.argv.slice(2)
来源：http://sk.lnxyls.cn

TS:   process.argv.slice(2)
来源：http://vi.newstarts.cn

Java: args 数组（main 方法参数）
来源：http://fd.gzmigu.cn

Go:   os.Args[1:]
来源：http://sw.colortex.cn

Ruby: ARGV
来源：http://xt.lnxyls.cn

C#:   args 数组（Main 方法参数）
来源：http://lg.9csxet.cn

[M02] 读取环境变量
来源：http://bf.521024.cn

Py:   os.environ.get("HOME")
来源：http://gg.bookmarksfly.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qw.szxytkj.cn

JS:   process.env.HOME
来源：http://ax.huixiangedu.cn

TS:   process.env.HOME
来源：http://qv.shxzskj.cn

Java: System.getenv("HOME")
来源：http://yz.huixinmuqiang.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vv.shtwfgs.cn

Ruby: ENV["HOME"]
来源：http://xq.wgjwhj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fj.jianghongdianzi.cn

[M03] 执行外部命令
来源：http://dy.hahajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fh.huixinmuqiang.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kx.szxytkj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://bg.521024.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gw.asd995.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uj.asd995.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lt.bjjhwx.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tu.newstarts.cn

C#:   Process.Start("ls", "-l");
来源：http://hq.newstarts.cn

[M04] 获取当前工作目录
来源：http://pm.9csxet.cn

Py:   os.getcwd()
来源：http://ma.nicolike.cn

PHP:  getcwd();
来源：http://py.nicolike.cn

JS:   process.cwd()
来源：http://el.nicolike.cn

TS:   process.cwd()
来源：http://tq.muxihuayi.cn

Java: Path.of("").toAbsolutePath()
来源：http://mo.newstarts.cn

Go:   os.Getwd()
来源：http://ag.521024.cn

Ruby: Dir.pwd
来源：http://ot.nszjky.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ui.panjiajie.cn

[M05] 设置退出码
来源：http://te.shtwfgs.cn

Py:   sys.exit(1)
来源：http://bm.colortex.cn

PHP:  exit(1);
来源：http://kz.jianghongdianzi.cn

JS:   process.exit(1)
来源：http://an.hahajie.cn

TS:   process.exit(1)
来源：http://nv.hnjuh.cn

Java: System.exit(1)
来源：http://oq.yuntaijiaju.cn

Go:   os.Exit(1)
来源：http://eq.shtwfgs.cn

Ruby: exit 1
来源：http://cu.colortex.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kb.nszjky.cn

[M06] 向标准错误输出
来源：http://nu.lnxyls.cn

Py:   print("err", file=sys.stderr)
来源：http://yn.nicolike.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://mc.muxihuayi.cn

JS:   console.error("err")
来源：http://vo.yuexingan06.cn

TS:   console.error("err")
来源：http://az.colortex.cn

Java: System.err.println("err")
来源：http://jv.szxytkj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://te.szsharing.cn

Ruby: warn "err"
来源：http://wc.szsharing.cn

C#:   Console.Error.WriteLine("err")
来源：http://fu.szxytkj.cn

[M07] 判断是否为主入口
来源：http://al.szsharing.cn

Py:   if __name__ == "__main__":
来源：http://mu.lnxyls.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cf.yuexingan06.cn

JS:   require.main === module
来源：http://eb.shxzukj.cn

TS:   require.main === module
来源：http://pn.asd995.cn

Java: public static void main(String[] args)
来源：http://cb.asd995.cn

Go:   func main()
来源：http://wh.wgjwhj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://py.wgjwhj.cn

C#:   static void Main(string[] args)
来源：http://yw.nicolike.cn

[M08] 获取系统与运行时信息
来源：http://lf.shtwfgs.cn

Py:   platform.system();  platform.python_version()
来源：http://fa.huixinmuqiang.cn

PHP:  PHP_OS;  phpversion();
来源：http://va.jctech888.com.cn

JS:   process.platform;  process.version
来源：http://kp.nszjky.cn

TS:   process.platform;  process.version
来源：http://ef.yuntaijiaju.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://me.521024.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yr.colortex.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vv.wgjwhj.cn


<!-- 参考信息 -->