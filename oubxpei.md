代发 wailian999

Go:   time.Now()
来源：http://ok.huixinmuqiang.cn

Ruby: Time.now
来源：http://ss.chemitech.net.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://df.huanxung.cn

[J02] 格式化输出
来源：http://ti.hahajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xh.huixinmuqiang.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tg.wgjwhj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pu.shtwfgs.cn

TS:   d.toISOString()
来源：http://vu.bookmarksfly.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dx.huixiangedu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wj.newstarts.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://df.jctech888.com.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://eo.szsharing.cn

[J03] 字符串解析为日期
来源：http://dx.szsharing.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gd.szxytkj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tj.asd995.cn

JS:   new Date("2024-01-02")
来源：http://fr.bjjhwx.cn

TS:   new Date("2024-01-02")
来源：http://rd.lnxyls.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fj.hahajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ad.yuntaijiaju.cn

Ruby: Date.parse("2024-01-02")
来源：http://in.shtwfgs.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wa.521024.cn

[J04] 时间戳与日期互转
来源：http://ao.shxzukj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zr.haigaiapp.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zp.haigaiapp.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kh.lnxyls.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qy.shtwfgs.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://js.jianghongdianzi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gj.yuexingan06.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uq.huanxung.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vd.panjiajie.cn

[J05] 时间加减（加 7 天）
来源：http://xz.huixiangedu.cn

Py:   now + timedelta(days=7)
来源：http://wh.panjiajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://at.shxzskj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hd.panjiajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vm.jctech888.com.cn

Java: LocalDate.now().plusDays(7)
来源：http://ah.shxzukj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pc.chemitech.net.cn

Ruby: Time.now + 7 * 86400
来源：http://ww.muxihuayi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://sj.yuntaijiaju.cn

[J06] 计算两时间之差
来源：http://wc.hahajie.cn

Py:   (end - start).total_seconds()
来源：http://ax.haigaiapp.cn

PHP:  $end->diff($start)->days;
来源：http://bz.jctech888.com.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lu.nicolike.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wn.hnjuh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://cu.huixinmuqiang.cn

Go:   end.Sub(start).Hours()
来源：http://wi.521024.cn

Ruby: end - start                 # 返回秒数
来源：http://ms.bookmarksfly.cn

C#:   (end - start).TotalSeconds
来源：http://ec.nszjky.cn

[J07] 比较两个日期
来源：http://iw.huixinmuqiang.cn

Py:   d1 < d2;  d1 == d2
来源：http://nl.szxytkj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ew.newstarts.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wn.shtwfgs.cn

TS:   d1.getTime() < d2.getTime()
来源：http://cv.lnxyls.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://oj.yuntaijiaju.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bn.newstarts.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bl.yuexingan06.cn

C#:   d1 < d2;  d1 == d2
来源：http://ny.nicolike.cn

[J08] 提取年月日与星期
来源：http://ws.lnxyls.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jp.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nu.shxzukj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yg.nicolike.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oi.wgjwhj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ca.bjjhwx.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yy.haigaiapp.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ka.bjjhwx.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tl.wgjwhj.cn

[J09] 时区处理
来源：http://si.huixinmuqiang.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ls.yuntaijiaju.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cm.521024.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fi.huixiangedu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ur.nicolike.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bv.shxzskj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uk.panjiajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://nl.nszjky.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dx.shtwfgs.cn

[J10] 取今天 / 本月第一天
来源：http://mx.szsharing.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ay.jctech888.com.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xs.asd995.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://da.shxzukj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hm.shtwfgs.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wa.huixiangedu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ju.newstarts.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tk.asd995.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cs.szxytkj.cn

================================================================================
来源：http://vg.521024.cn

K. JSON 与序列化
来源：http://fx.szxytkj.cn

================================================================================
来源：http://lu.gzmigu.cn

[K01] 对象转 JSON 字符串
来源：http://ev.521024.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jh.panjiajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mm.newstarts.cn

JS:   JSON.stringify(obj)
来源：http://sd.muxihuayi.cn

TS:   JSON.stringify(obj)
来源：http://sx.szxytkj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qd.gzmigu.cn

Go:   json.Marshal(obj)
来源：http://qt.szxytkj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zt.szsharing.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://kt.huixiangedu.cn

[K02] JSON 字符串转对象
来源：http://ax.bjjhwx.cn

Py:   json.loads(s)
来源：http://zz.colortex.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://st.haigaiapp.cn

JS:   JSON.parse(s)
来源：http://xz.bookmarksfly.cn

TS:   JSON.parse(s)
来源：http://uu.yuexingan06.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tr.jianghongdianzi.cn

Go:   json.Unmarshal(data, &v)
来源：http://fs.nicolike.cn

Ruby: JSON.parse(s)
来源：http://ew.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ej.huixinmuqiang.cn

[K03] JSON 美化输出（带缩进）
来源：http://if.wgjwhj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gs.asd995.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sd.shtwfgs.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ks.colortex.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://kr.wgjwhj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pu.521024.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cm.huixinmuqiang.cn

Ruby: JSON.pretty_generate(obj)
来源：http://cf.hnjuh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://la.muxihuayi.cn

[K04] 读取 JSON 文件
来源：http://vh.szsharing.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dm.hahajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kc.yuntaijiaju.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ft.shtwfgs.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ma.nicolike.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cu.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://eg.huixinmuqiang.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jz.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lp.newstarts.cn

[K05] 深拷贝对象
来源：http://xc.huixiangedu.cn

Py:   copy.deepcopy(obj)
来源：http://ej.panjiajie.cn

PHP:  unserialize(serialize($obj));
来源：http://lh.wgjwhj.cn

JS:   structuredClone(obj)
来源：http://nc.wgjwhj.cn

TS:   structuredClone(obj)
来源：http://qy.nicolike.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://pu.colortex.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rn.shxzukj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bi.shxzukj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://kg.panjiajie.cn

[K06] 解析 URL 查询串
来源：http://or.colortex.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rx.szsharing.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sl.gzmigu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oy.521024.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oe.newstarts.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kn.shxzskj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qu.nszjky.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qy.shxzukj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zj.chemitech.net.cn

[K07] 进制转换
来源：http://qr.chemitech.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dh.521024.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kg.asd995.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cd.yuexingan06.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qq.nicolike.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ho.jctech888.com.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dk.huixiangedu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hm.lnxyls.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jq.gzmigu.cn

[K08] 二进制序列化（非 JSON）
来源：http://xy.bookmarksfly.cn

Py:   pickle.dumps(obj)
来源：http://cv.lnxyls.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cp.jctech888.com.cn

JS:   v8.serialize(obj)        // Node
来源：http://no.521024.cn

TS:   v8.serialize(obj)        // Node
来源：http://wm.hahajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pd.bjjhwx.cn

Go:   encoding/gob
来源：http://tb.521024.cn

Ruby: Marshal.dump(obj)
来源：http://gy.nszjky.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gj.haigaiapp.cn

================================================================================
来源：http://wp.521024.cn

L. 网络请求
来源：http://xi.muxihuayi.cn

================================================================================
来源：http://nm.huanxung.cn

[L01] 发送 GET 请求
来源：http://vp.yuntaijiaju.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mg.jianghongdianzi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xo.shtwfgs.cn

JS:   await fetch(url)
来源：http://zt.jctech888.com.cn

TS:   await fetch(url)
来源：http://sd.hnjuh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jo.521024.cn

Go:   resp, err := http.Get(url)
来源：http://rg.9csxet.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://vy.9csxet.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tw.nicolike.cn

[L02] 发送 POST JSON
来源：http://mo.newstarts.cn

Py:   requests.post(url, json={"a": 1})
来源：http://la.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jh.szxytkj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gz.yuntaijiaju.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gl.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ev.nicolike.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ht.shxzukj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lv.shtwfgs.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ll.szsharing.cn

[L03] 设置自定义请求头
来源：http://wo.bjjhwx.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dw.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fl.huanxung.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jt.colortex.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://es.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://us.9csxet.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bf.hnjuh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://au.szsharing.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hr.haigaiapp.cn

[L04] 设置超时
来源：http://dk.shxzskj.cn

Py:   requests.get(url, timeout=5)
来源：http://eg.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ox.gzmigu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gk.szxytkj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pk.jianghongdianzi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ef.panjiajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ae.lnxyls.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://av.lnxyls.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://da.shxzukj.cn

[L05] 上传文件（multipart）
来源：http://fl.chemitech.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mp.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ql.jianghongdianzi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ia.hnjuh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pm.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cu.newstarts.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gt.shxzukj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pk.shxzukj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pz.nszjky.cn

[L06] 解析响应为 JSON
来源：http://xw.jianghongdianzi.cn

Py:   resp.json()
来源：http://qz.chemitech.net.cn

PHP:  json_decode($body, true);
来源：http://fv.muxihuayi.cn

JS:   await resp.json()
来源：http://la.hahajie.cn

TS:   await resp.json()
来源：http://it.nszjky.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dq.wgjwhj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uq.szsharing.cn

Ruby: JSON.parse(resp.body)
来源：http://qk.521024.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xu.jctech888.com.cn

[L07] 处理 HTTP 状态码
来源：http://la.shxzukj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://do.jctech888.com.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ft.shxzukj.cn

JS:   resp.ok;  resp.status
来源：http://jk.jianghongdianzi.cn

TS:   resp.ok;  resp.status
来源：http://ua.hnjuh.cn

Java: resp.statusCode()
来源：http://th.colortex.cn

Go:   resp.StatusCode
来源：http://yp.szxytkj.cn

Ruby: resp.code.to_i
来源：http://ia.huanxung.cn

C#:   (int)resp.StatusCode
来源：http://kk.gzmigu.cn

[L08] 并发请求多个地址
来源：http://ea.haigaiapp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zp.szsharing.cn

PHP:  curl_multi_init() 系列
来源：http://fi.colortex.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qa.yuntaijiaju.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qk.gzmigu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://je.shxzskj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nx.gzmigu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ey.huixiangedu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vs.lnxyls.cn

================================================================================
来源：http://fc.newstarts.cn

M. 命令行 / 进程 / 环境
来源：http://rz.yuntaijiaju.cn

================================================================================
来源：http://fl.shxzukj.cn

[M01] 读取命令行参数
来源：http://ga.yuexingan06.cn

Py:   sys.argv[1:]
来源：http://io.colortex.cn

PHP:  $argv;  $argc;
来源：http://mk.shxzukj.cn

JS:   process.argv.slice(2)
来源：http://uq.hahajie.cn

TS:   process.argv.slice(2)
来源：http://hw.bjjhwx.cn

Java: args 数组（main 方法参数）
来源：http://fg.hahajie.cn

Go:   os.Args[1:]
来源：http://fw.9csxet.cn

Ruby: ARGV
来源：http://to.9csxet.cn

C#:   args 数组（Main 方法参数）
来源：http://uh.panjiajie.cn

[M02] 读取环境变量
来源：http://hy.szsharing.cn

Py:   os.environ.get("HOME")
来源：http://vy.nicolike.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jj.huixinmuqiang.cn

JS:   process.env.HOME
来源：http://lx.muxihuayi.cn

TS:   process.env.HOME
来源：http://zc.521024.cn

Java: System.getenv("HOME")
来源：http://gu.lnxyls.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yi.newstarts.cn

Ruby: ENV["HOME"]
来源：http://ro.huanxung.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zw.shxzukj.cn

[M03] 执行外部命令
来源：http://hs.muxihuayi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ga.newstarts.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jc.szxytkj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://tx.newstarts.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wl.yuexingan06.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lj.shtwfgs.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://pb.jctech888.com.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yq.jianghongdianzi.cn

C#:   Process.Start("ls", "-l");
来源：http://mw.lnxyls.cn

[M04] 获取当前工作目录
来源：http://cq.shxzskj.cn

Py:   os.getcwd()
来源：http://fa.muxihuayi.cn

PHP:  getcwd();
来源：http://yt.521024.cn

JS:   process.cwd()
来源：http://hi.yuntaijiaju.cn

TS:   process.cwd()
来源：http://ld.huixiangedu.cn

Java: Path.of("").toAbsolutePath()
来源：http://uu.9csxet.cn

Go:   os.Getwd()
来源：http://ui.huixiangedu.cn

Ruby: Dir.pwd
来源：http://xy.muxihuayi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://eq.bjjhwx.cn

[M05] 设置退出码
来源：http://af.szsharing.cn

Py:   sys.exit(1)
来源：http://is.szsharing.cn

PHP:  exit(1);
来源：http://xq.521024.cn

JS:   process.exit(1)
来源：http://on.asd995.cn

TS:   process.exit(1)
来源：http://ga.bookmarksfly.cn

Java: System.exit(1)
来源：http://gp.panjiajie.cn

Go:   os.Exit(1)
来源：http://gr.wgjwhj.cn

Ruby: exit 1
来源：http://ho.szsharing.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ti.muxihuayi.cn

[M06] 向标准错误输出
来源：http://vs.shtwfgs.cn

Py:   print("err", file=sys.stderr)
来源：http://gj.521024.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qy.huixinmuqiang.cn

JS:   console.error("err")
来源：http://us.bjjhwx.cn

TS:   console.error("err")
来源：http://kn.jctech888.com.cn

Java: System.err.println("err")
来源：http://wg.bjjhwx.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hr.gzmigu.cn

Ruby: warn "err"
来源：http://hp.hahajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://ae.hahajie.cn

[M07] 判断是否为主入口
来源：http://ns.bookmarksfly.cn

Py:   if __name__ == "__main__":
来源：http://jm.gzmigu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://eg.gzmigu.cn

JS:   require.main === module
来源：http://az.521024.cn

TS:   require.main === module
来源：http://we.jianghongdianzi.cn

Java: public static void main(String[] args)
来源：http://am.hahajie.cn

Go:   func main()
来源：http://sw.lnxyls.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kw.nicolike.cn

C#:   static void Main(string[] args)
来源：http://up.colortex.cn


<!-- 参考信息 -->