代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://np.newstarts.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mk.huixinmuqiang.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cc.haigaiapp.cn

TS:   d.toISOString()
来源：http://si.huanxung.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lj.hnjuh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vw.asd995.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://db.wgjwhj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://it.gzmigu.cn

[J03] 字符串解析为日期
来源：http://ak.szsharing.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sr.haigaiapp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gc.bookmarksfly.cn

JS:   new Date("2024-01-02")
来源：http://bd.shxzukj.cn

TS:   new Date("2024-01-02")
来源：http://nn.bjjhwx.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mp.bookmarksfly.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kk.nszjky.cn

Ruby: Date.parse("2024-01-02")
来源：http://ho.huixinmuqiang.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gc.jianghongdianzi.cn

[J04] 时间戳与日期互转
来源：http://gv.gzmigu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ga.jctech888.com.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tn.szsharing.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rg.yuexingan06.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://un.hnjuh.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xb.9csxet.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vm.hahajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fn.szsharing.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fx.shxzskj.cn

[J05] 时间加减（加 7 天）
来源：http://zz.huixiangedu.cn

Py:   now + timedelta(days=7)
来源：http://cm.gzmigu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bq.hnjuh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nv.huixiangedu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ly.yuexingan06.cn

Java: LocalDate.now().plusDays(7)
来源：http://wz.hnjuh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bb.jianghongdianzi.cn

Ruby: Time.now + 7 * 86400
来源：http://nf.hahajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://fz.asd995.cn

[J06] 计算两时间之差
来源：http://jz.521024.cn

Py:   (end - start).total_seconds()
来源：http://yf.hnjuh.cn

PHP:  $end->diff($start)->days;
来源：http://xf.wgjwhj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xx.lnxyls.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uz.asd995.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hs.shtwfgs.cn

Go:   end.Sub(start).Hours()
来源：http://zp.huixiangedu.cn

Ruby: end - start                 # 返回秒数
来源：http://kc.hnjuh.cn

C#:   (end - start).TotalSeconds
来源：http://qa.newstarts.cn

[J07] 比较两个日期
来源：http://kk.gzmigu.cn

Py:   d1 < d2;  d1 == d2
来源：http://rc.newstarts.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kg.colortex.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xj.colortex.cn

TS:   d1.getTime() < d2.getTime()
来源：http://pt.huanxung.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xi.hahajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gn.hahajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://dw.jianghongdianzi.cn

C#:   d1 < d2;  d1 == d2
来源：http://fa.panjiajie.cn

[J08] 提取年月日与星期
来源：http://oy.gzmigu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tk.colortex.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bp.wgjwhj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yp.jctech888.com.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oq.hnjuh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gy.9csxet.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rs.muxihuayi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sg.chemitech.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yc.haigaiapp.cn

[J09] 时区处理
来源：http://ro.asd995.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lj.muxihuayi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gp.newstarts.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wk.bjjhwx.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kj.hahajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ng.shxzukj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ht.521024.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lv.yuntaijiaju.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zc.yuexingan06.cn

[J10] 取今天 / 本月第一天
来源：http://zw.szsharing.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kx.wgjwhj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://iz.huixinmuqiang.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fs.panjiajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zg.521024.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rk.hahajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://da.hahajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ij.bookmarksfly.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lk.haigaiapp.cn

================================================================================
来源：http://if.521024.cn

K. JSON 与序列化
来源：http://ih.szsharing.cn

================================================================================
来源：http://xo.newstarts.cn

[K01] 对象转 JSON 字符串
来源：http://ff.colortex.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gb.colortex.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ew.muxihuayi.cn

JS:   JSON.stringify(obj)
来源：http://md.huixinmuqiang.cn

TS:   JSON.stringify(obj)
来源：http://ga.shxzskj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nq.nszjky.cn

Go:   json.Marshal(obj)
来源：http://jj.9csxet.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dx.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bk.wgjwhj.cn

[K02] JSON 字符串转对象
来源：http://lz.lnxyls.cn

Py:   json.loads(s)
来源：http://nh.hahajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gg.muxihuayi.cn

JS:   JSON.parse(s)
来源：http://io.wgjwhj.cn

TS:   JSON.parse(s)
来源：http://bm.shtwfgs.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zg.521024.cn

Go:   json.Unmarshal(data, &v)
来源：http://zj.hnjuh.cn

Ruby: JSON.parse(s)
来源：http://um.colortex.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zf.haigaiapp.cn

[K03] JSON 美化输出（带缩进）
来源：http://hl.bjjhwx.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hc.panjiajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hc.huixinmuqiang.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ml.bookmarksfly.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sd.bjjhwx.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rw.huixinmuqiang.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uj.newstarts.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ew.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vn.asd995.cn

[K04] 读取 JSON 文件
来源：http://op.yuntaijiaju.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://eg.gzmigu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kj.bookmarksfly.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ac.haigaiapp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ks.nicolike.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sq.shxzukj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ag.shxzskj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vt.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://li.huanxung.cn

[K05] 深拷贝对象
来源：http://pf.haigaiapp.cn

Py:   copy.deepcopy(obj)
来源：http://nq.huixiangedu.cn

PHP:  unserialize(serialize($obj));
来源：http://rd.panjiajie.cn

JS:   structuredClone(obj)
来源：http://mk.haigaiapp.cn

TS:   structuredClone(obj)
来源：http://ll.huanxung.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mo.9csxet.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tl.colortex.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zp.yuexingan06.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://jj.huixinmuqiang.cn

[K06] 解析 URL 查询串
来源：http://fd.newstarts.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cr.szsharing.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gc.szxytkj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bl.newstarts.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://df.521024.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zb.nszjky.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ey.nicolike.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lk.hnjuh.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tq.wgjwhj.cn

[K07] 进制转换
来源：http://ts.haigaiapp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://an.hnjuh.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sy.yuexingan06.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://op.shxzukj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fj.shtwfgs.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ks.hnjuh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ga.shxzukj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zj.szsharing.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://my.shtwfgs.cn

[K08] 二进制序列化（非 JSON）
来源：http://tf.yuexingan06.cn

Py:   pickle.dumps(obj)
来源：http://oc.521024.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://aq.shtwfgs.cn

JS:   v8.serialize(obj)        // Node
来源：http://ux.szxytkj.cn

TS:   v8.serialize(obj)        // Node
来源：http://bb.nszjky.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xc.9csxet.cn

Go:   encoding/gob
来源：http://ix.szsharing.cn

Ruby: Marshal.dump(obj)
来源：http://bh.yuexingan06.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nc.muxihuayi.cn

================================================================================
来源：http://tv.hnjuh.cn

L. 网络请求
来源：http://cg.bookmarksfly.cn

================================================================================
来源：http://jw.gzmigu.cn

[L01] 发送 GET 请求
来源：http://np.huixinmuqiang.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bd.huixinmuqiang.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://aa.nszjky.cn

JS:   await fetch(url)
来源：http://ee.wgjwhj.cn

TS:   await fetch(url)
来源：http://uy.shxzukj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ev.asd995.cn

Go:   resp, err := http.Get(url)
来源：http://zh.hnjuh.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pi.jctech888.com.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yi.9csxet.cn

[L02] 发送 POST JSON
来源：http://iu.521024.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zs.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://eg.yuntaijiaju.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://en.newstarts.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ov.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yl.chemitech.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bd.hnjuh.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bo.shtwfgs.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yk.muxihuayi.cn

[L03] 设置自定义请求头
来源：http://zr.shxzukj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://oe.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rm.chemitech.net.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dy.shxzukj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ch.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ri.huixiangedu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nt.asd995.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vj.9csxet.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gs.colortex.cn

[L04] 设置超时
来源：http://hh.hnjuh.cn

Py:   requests.get(url, timeout=5)
来源：http://fz.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vr.wgjwhj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tm.yuexingan06.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://er.colortex.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nt.jianghongdianzi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xo.jianghongdianzi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ff.gzmigu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xg.shxzukj.cn

[L05] 上传文件（multipart）
来源：http://zs.chemitech.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ni.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lk.asd995.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://op.hnjuh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zl.szxytkj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ri.newstarts.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ye.nszjky.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://st.szxytkj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://it.haigaiapp.cn

[L06] 解析响应为 JSON
来源：http://lf.shxzukj.cn

Py:   resp.json()
来源：http://dp.yuexingan06.cn

PHP:  json_decode($body, true);
来源：http://zf.huanxung.cn

JS:   await resp.json()
来源：http://mj.lnxyls.cn

TS:   await resp.json()
来源：http://dq.bookmarksfly.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uj.nszjky.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dl.chemitech.net.cn

Ruby: JSON.parse(resp.body)
来源：http://zg.nicolike.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://as.huixiangedu.cn

[L07] 处理 HTTP 状态码
来源：http://qm.lnxyls.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fz.bookmarksfly.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zj.yuexingan06.cn

JS:   resp.ok;  resp.status
来源：http://eq.haigaiapp.cn

TS:   resp.ok;  resp.status
来源：http://ny.panjiajie.cn

Java: resp.statusCode()
来源：http://zp.colortex.cn

Go:   resp.StatusCode
来源：http://dg.jctech888.com.cn

Ruby: resp.code.to_i
来源：http://ht.newstarts.cn

C#:   (int)resp.StatusCode
来源：http://pm.szsharing.cn

[L08] 并发请求多个地址
来源：http://so.hnjuh.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wm.shtwfgs.cn

PHP:  curl_multi_init() 系列
来源：http://hs.shxzukj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iy.bookmarksfly.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tx.lnxyls.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://el.panjiajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nr.nicolike.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://us.yuntaijiaju.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vv.asd995.cn

================================================================================
来源：http://ec.huixiangedu.cn

M. 命令行 / 进程 / 环境
来源：http://xh.gzmigu.cn

================================================================================
来源：http://rb.huanxung.cn

[M01] 读取命令行参数
来源：http://cj.jctech888.com.cn

Py:   sys.argv[1:]
来源：http://wy.jianghongdianzi.cn

PHP:  $argv;  $argc;
来源：http://oe.yuntaijiaju.cn

JS:   process.argv.slice(2)
来源：http://tc.bjjhwx.cn

TS:   process.argv.slice(2)
来源：http://kf.bjjhwx.cn

Java: args 数组（main 方法参数）
来源：http://yb.nszjky.cn

Go:   os.Args[1:]
来源：http://rg.chemitech.net.cn

Ruby: ARGV
来源：http://br.haigaiapp.cn

C#:   args 数组（Main 方法参数）
来源：http://vm.lnxyls.cn

[M02] 读取环境变量
来源：http://up.shtwfgs.cn

Py:   os.environ.get("HOME")
来源：http://sw.nicolike.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fl.bjjhwx.cn

JS:   process.env.HOME
来源：http://cv.yuexingan06.cn

TS:   process.env.HOME
来源：http://sm.nszjky.cn

Java: System.getenv("HOME")
来源：http://jx.lnxyls.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zp.newstarts.cn

Ruby: ENV["HOME"]
来源：http://re.hnjuh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nn.hahajie.cn

[M03] 执行外部命令
来源：http://pw.haigaiapp.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ou.asd995.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zz.521024.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://oc.jctech888.com.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wz.colortex.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ho.lnxyls.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://du.bjjhwx.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yv.muxihuayi.cn

C#:   Process.Start("ls", "-l");
来源：http://zb.yuexingan06.cn

[M04] 获取当前工作目录
来源：http://ha.bookmarksfly.cn

Py:   os.getcwd()
来源：http://qj.chemitech.net.cn

PHP:  getcwd();
来源：http://qb.yuntaijiaju.cn

JS:   process.cwd()
来源：http://dx.wgjwhj.cn

TS:   process.cwd()
来源：http://sz.yuntaijiaju.cn

Java: Path.of("").toAbsolutePath()
来源：http://hx.wgjwhj.cn

Go:   os.Getwd()
来源：http://nh.chemitech.net.cn

Ruby: Dir.pwd
来源：http://ck.shxzskj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://bm.hnjuh.cn

[M05] 设置退出码
来源：http://yz.panjiajie.cn

Py:   sys.exit(1)
来源：http://wg.9csxet.cn

PHP:  exit(1);
来源：http://jp.yuntaijiaju.cn

JS:   process.exit(1)
来源：http://xi.521024.cn

TS:   process.exit(1)
来源：http://yo.huanxung.cn

Java: System.exit(1)
来源：http://sq.bjjhwx.cn

Go:   os.Exit(1)
来源：http://pa.521024.cn

Ruby: exit 1
来源：http://mn.shxzskj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zf.521024.cn

[M06] 向标准错误输出
来源：http://sp.colortex.cn

Py:   print("err", file=sys.stderr)
来源：http://kb.521024.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bw.nszjky.cn

JS:   console.error("err")
来源：http://da.huanxung.cn

TS:   console.error("err")
来源：http://mr.jctech888.com.cn

Java: System.err.println("err")
来源：http://uv.panjiajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ip.newstarts.cn

Ruby: warn "err"
来源：http://sb.bookmarksfly.cn

C#:   Console.Error.WriteLine("err")
来源：http://ua.wgjwhj.cn

[M07] 判断是否为主入口
来源：http://fh.jianghongdianzi.cn

Py:   if __name__ == "__main__":
来源：http://cv.hahajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://oh.szsharing.cn

JS:   require.main === module
来源：http://dr.szxytkj.cn

TS:   require.main === module
来源：http://uc.szxytkj.cn

Java: public static void main(String[] args)
来源：http://wu.hahajie.cn

Go:   func main()
来源：http://ty.521024.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dh.shxzskj.cn

C#:   static void Main(string[] args)
来源：http://ml.colortex.cn

[M08] 获取系统与运行时信息
来源：http://qi.gzmigu.cn

Py:   platform.system();  platform.python_version()
来源：http://im.huixiangedu.cn

PHP:  PHP_OS;  phpversion();
来源：http://qo.9csxet.cn

JS:   process.platform;  process.version
来源：http://xx.muxihuayi.cn


<!-- 参考信息 -->