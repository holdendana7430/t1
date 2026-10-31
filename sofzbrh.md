代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zk.newstarts.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bq.nicolike.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mu.huanxung.cn

TS:   d.toISOString()
来源：http://lw.bookmarksfly.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hy.muxihuayi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lh.shxzskj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nw.panjiajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rv.wgjwhj.cn

[J03] 字符串解析为日期
来源：http://ks.9csxet.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wl.huanxung.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ns.hahajie.cn

JS:   new Date("2024-01-02")
来源：http://pt.huixinmuqiang.cn

TS:   new Date("2024-01-02")
来源：http://dp.huixinmuqiang.cn

Java: LocalDate.parse("2024-01-02")
来源：http://om.szsharing.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vu.hnjuh.cn

Ruby: Date.parse("2024-01-02")
来源：http://ph.shxzskj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uy.lnxyls.cn

[J04] 时间戳与日期互转
来源：http://lp.newstarts.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hs.9csxet.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xc.bookmarksfly.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://my.hahajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://yc.szxytkj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ds.bjjhwx.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hu.hnjuh.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ks.muxihuayi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dy.yuexingan06.cn

[J05] 时间加减（加 7 天）
来源：http://kv.shtwfgs.cn

Py:   now + timedelta(days=7)
来源：http://pp.jctech888.com.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zm.asd995.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gs.yuexingan06.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yy.bjjhwx.cn

Java: LocalDate.now().plusDays(7)
来源：http://wr.asd995.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://du.521024.cn

Ruby: Time.now + 7 * 86400
来源：http://de.jianghongdianzi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jp.9csxet.cn

[J06] 计算两时间之差
来源：http://kp.gzmigu.cn

Py:   (end - start).total_seconds()
来源：http://vs.asd995.cn

PHP:  $end->diff($start)->days;
来源：http://qj.haigaiapp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://di.nicolike.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wo.bookmarksfly.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vj.szxytkj.cn

Go:   end.Sub(start).Hours()
来源：http://vc.nszjky.cn

Ruby: end - start                 # 返回秒数
来源：http://ns.asd995.cn

C#:   (end - start).TotalSeconds
来源：http://de.bookmarksfly.cn

[J07] 比较两个日期
来源：http://lm.panjiajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://sf.colortex.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://iz.shxzukj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://yf.wgjwhj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ei.521024.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mr.shtwfgs.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dn.shtwfgs.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ih.newstarts.cn

C#:   d1 < d2;  d1 == d2
来源：http://aa.yuexingan06.cn

[J08] 提取年月日与星期
来源：http://pk.yuntaijiaju.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hg.colortex.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fn.nszjky.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xq.nicolike.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gn.yuexingan06.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ez.shxzskj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mz.yuexingan06.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yn.szxytkj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xc.szsharing.cn

[J09] 时区处理
来源：http://pl.haigaiapp.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://db.521024.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dm.lnxyls.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wq.muxihuayi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://it.wgjwhj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zo.bjjhwx.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kn.chemitech.net.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lj.huixinmuqiang.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dj.lnxyls.cn

[J10] 取今天 / 本月第一天
来源：http://gy.shxzskj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ja.hahajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kl.yuntaijiaju.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yl.bjjhwx.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gt.yuntaijiaju.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ce.wgjwhj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hi.jctech888.com.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rt.asd995.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pi.haigaiapp.cn

================================================================================
来源：http://tx.521024.cn

K. JSON 与序列化
来源：http://bv.jctech888.com.cn

================================================================================
来源：http://nv.asd995.cn

[K01] 对象转 JSON 字符串
来源：http://is.chemitech.net.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cp.yuexingan06.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://iq.jctech888.com.cn

JS:   JSON.stringify(obj)
来源：http://tw.panjiajie.cn

TS:   JSON.stringify(obj)
来源：http://xk.yuntaijiaju.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fq.jianghongdianzi.cn

Go:   json.Marshal(obj)
来源：http://fk.huixiangedu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vb.9csxet.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bc.nszjky.cn

[K02] JSON 字符串转对象
来源：http://ix.shxzukj.cn

Py:   json.loads(s)
来源：http://ud.lnxyls.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ft.yuntaijiaju.cn

JS:   JSON.parse(s)
来源：http://nt.colortex.cn

TS:   JSON.parse(s)
来源：http://qc.huixiangedu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tq.newstarts.cn

Go:   json.Unmarshal(data, &v)
来源：http://lz.newstarts.cn

Ruby: JSON.parse(s)
来源：http://dg.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fy.wgjwhj.cn

[K03] JSON 美化输出（带缩进）
来源：http://xp.yuexingan06.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://si.lnxyls.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vk.huixiangedu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://sx.shxzskj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ex.yuntaijiaju.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://go.panjiajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://us.jctech888.com.cn

Ruby: JSON.pretty_generate(obj)
来源：http://tf.panjiajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ph.hahajie.cn

[K04] 读取 JSON 文件
来源：http://vh.haigaiapp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dn.hnjuh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qv.huixinmuqiang.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ny.szxytkj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bl.huixiangedu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rt.shxzukj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ey.hahajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://sb.colortex.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zd.nszjky.cn

[K05] 深拷贝对象
来源：http://ay.bjjhwx.cn

Py:   copy.deepcopy(obj)
来源：http://ex.colortex.cn

PHP:  unserialize(serialize($obj));
来源：http://ad.newstarts.cn

JS:   structuredClone(obj)
来源：http://cy.nszjky.cn

TS:   structuredClone(obj)
来源：http://gv.521024.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ku.shtwfgs.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qc.huanxung.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ig.colortex.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fb.nszjky.cn

[K06] 解析 URL 查询串
来源：http://iv.shxzskj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xw.jctech888.com.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hs.huixinmuqiang.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://of.bookmarksfly.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lb.huanxung.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hm.shxzskj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ie.huixinmuqiang.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ac.bookmarksfly.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://or.lnxyls.cn

[K07] 进制转换
来源：http://lx.haigaiapp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ie.szsharing.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dl.shxzukj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gv.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qb.hnjuh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ce.shtwfgs.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ix.huixinmuqiang.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://am.panjiajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pj.9csxet.cn

[K08] 二进制序列化（非 JSON）
来源：http://rp.huixinmuqiang.cn

Py:   pickle.dumps(obj)
来源：http://iv.lnxyls.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bo.wgjwhj.cn

JS:   v8.serialize(obj)        // Node
来源：http://dy.9csxet.cn

TS:   v8.serialize(obj)        // Node
来源：http://xe.nszjky.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ul.muxihuayi.cn

Go:   encoding/gob
来源：http://ql.szsharing.cn

Ruby: Marshal.dump(obj)
来源：http://on.asd995.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cc.szxytkj.cn

================================================================================
来源：http://ml.haigaiapp.cn

L. 网络请求
来源：http://ss.huixinmuqiang.cn

================================================================================
来源：http://pf.bookmarksfly.cn

[L01] 发送 GET 请求
来源：http://os.hnjuh.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lx.521024.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zr.chemitech.net.cn

JS:   await fetch(url)
来源：http://ad.haigaiapp.cn

TS:   await fetch(url)
来源：http://ju.yuntaijiaju.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ur.nszjky.cn

Go:   resp, err := http.Get(url)
来源：http://vm.muxihuayi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://vt.yuntaijiaju.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hi.gzmigu.cn

[L02] 发送 POST JSON
来源：http://tg.jianghongdianzi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cz.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uw.bookmarksfly.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ni.nicolike.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sn.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ir.szsharing.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wz.jianghongdianzi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sm.huixinmuqiang.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.wgjwhj.cn

[L03] 设置自定义请求头
来源：http://nc.newstarts.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kk.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ra.szxytkj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xm.colortex.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ha.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ko.asd995.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bg.shxzskj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fq.asd995.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://io.bjjhwx.cn

[L04] 设置超时
来源：http://il.lnxyls.cn

Py:   requests.get(url, timeout=5)
来源：http://ox.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fb.muxihuayi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sw.gzmigu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://on.shxzskj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://aw.shtwfgs.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wx.shtwfgs.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zx.muxihuayi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nh.huixinmuqiang.cn

[L05] 上传文件（multipart）
来源：http://fo.asd995.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pk.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cl.huanxung.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ev.szxytkj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vv.szxytkj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://eh.bookmarksfly.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://go.muxihuayi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nw.yuntaijiaju.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ok.huixinmuqiang.cn

[L06] 解析响应为 JSON
来源：http://mi.lnxyls.cn

Py:   resp.json()
来源：http://tx.asd995.cn

PHP:  json_decode($body, true);
来源：http://ma.wgjwhj.cn

JS:   await resp.json()
来源：http://yo.shxzskj.cn

TS:   await resp.json()
来源：http://rw.jctech888.com.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ci.yuexingan06.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://sh.chemitech.net.cn

Ruby: JSON.parse(resp.body)
来源：http://ut.521024.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gp.gzmigu.cn

[L07] 处理 HTTP 状态码
来源：http://xx.asd995.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nt.hnjuh.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fl.panjiajie.cn

JS:   resp.ok;  resp.status
来源：http://rh.gzmigu.cn

TS:   resp.ok;  resp.status
来源：http://nc.shxzskj.cn

Java: resp.statusCode()
来源：http://pd.yuntaijiaju.cn

Go:   resp.StatusCode
来源：http://dc.jctech888.com.cn

Ruby: resp.code.to_i
来源：http://yy.panjiajie.cn

C#:   (int)resp.StatusCode
来源：http://xu.huixinmuqiang.cn

[L08] 并发请求多个地址
来源：http://ih.bjjhwx.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tz.yuexingan06.cn

PHP:  curl_multi_init() 系列
来源：http://rb.chemitech.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nh.521024.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://st.szsharing.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ra.szsharing.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gt.szsharing.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://co.9csxet.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kg.szsharing.cn

================================================================================
来源：http://uv.gzmigu.cn

M. 命令行 / 进程 / 环境
来源：http://bu.panjiajie.cn

================================================================================
来源：http://ol.gzmigu.cn

[M01] 读取命令行参数
来源：http://gj.haigaiapp.cn

Py:   sys.argv[1:]
来源：http://ah.yuexingan06.cn

PHP:  $argv;  $argc;
来源：http://cp.colortex.cn

JS:   process.argv.slice(2)
来源：http://yc.hnjuh.cn

TS:   process.argv.slice(2)
来源：http://bq.haigaiapp.cn

Java: args 数组（main 方法参数）
来源：http://qq.shtwfgs.cn

Go:   os.Args[1:]
来源：http://wd.9csxet.cn

Ruby: ARGV
来源：http://je.szxytkj.cn

C#:   args 数组（Main 方法参数）
来源：http://xg.9csxet.cn

[M02] 读取环境变量
来源：http://ah.bookmarksfly.cn

Py:   os.environ.get("HOME")
来源：http://rd.shtwfgs.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jq.shtwfgs.cn

JS:   process.env.HOME
来源：http://dt.panjiajie.cn

TS:   process.env.HOME
来源：http://cd.huixiangedu.cn

Java: System.getenv("HOME")
来源：http://nw.shtwfgs.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hq.bookmarksfly.cn

Ruby: ENV["HOME"]
来源：http://pr.newstarts.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mr.bjjhwx.cn

[M03] 执行外部命令
来源：http://fz.szsharing.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wj.yuexingan06.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bw.hnjuh.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vi.bookmarksfly.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ht.yuexingan06.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vd.lnxyls.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xw.bookmarksfly.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kz.gzmigu.cn

C#:   Process.Start("ls", "-l");
来源：http://kf.panjiajie.cn

[M04] 获取当前工作目录
来源：http://cy.lnxyls.cn

Py:   os.getcwd()
来源：http://lo.chemitech.net.cn

PHP:  getcwd();
来源：http://bb.nszjky.cn

JS:   process.cwd()
来源：http://qh.nicolike.cn

TS:   process.cwd()
来源：http://bl.yuntaijiaju.cn

Java: Path.of("").toAbsolutePath()
来源：http://us.wgjwhj.cn

Go:   os.Getwd()
来源：http://yl.hnjuh.cn

Ruby: Dir.pwd
来源：http://yv.nicolike.cn

C#:   Directory.GetCurrentDirectory()
来源：http://le.chemitech.net.cn

[M05] 设置退出码
来源：http://uj.szsharing.cn

Py:   sys.exit(1)
来源：http://tc.jianghongdianzi.cn

PHP:  exit(1);
来源：http://jl.wgjwhj.cn

JS:   process.exit(1)
来源：http://vm.haigaiapp.cn

TS:   process.exit(1)
来源：http://er.jianghongdianzi.cn

Java: System.exit(1)
来源：http://dc.newstarts.cn

Go:   os.Exit(1)
来源：http://im.haigaiapp.cn

Ruby: exit 1
来源：http://tb.yuntaijiaju.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qp.yuexingan06.cn

[M06] 向标准错误输出
来源：http://qp.gzmigu.cn

Py:   print("err", file=sys.stderr)
来源：http://cg.bjjhwx.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://au.muxihuayi.cn

JS:   console.error("err")
来源：http://ks.colortex.cn

TS:   console.error("err")
来源：http://vl.wgjwhj.cn

Java: System.err.println("err")
来源：http://xk.bjjhwx.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bi.panjiajie.cn

Ruby: warn "err"
来源：http://or.521024.cn

C#:   Console.Error.WriteLine("err")
来源：http://gt.chemitech.net.cn

[M07] 判断是否为主入口
来源：http://nf.lnxyls.cn

Py:   if __name__ == "__main__":
来源：http://cx.newstarts.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ud.jctech888.com.cn

JS:   require.main === module
来源：http://mw.shxzskj.cn

TS:   require.main === module
来源：http://ue.colortex.cn

Java: public static void main(String[] args)
来源：http://bk.shxzskj.cn

Go:   func main()
来源：http://uk.huixiangedu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nf.jctech888.com.cn

C#:   static void Main(string[] args)
来源：http://vt.yuntaijiaju.cn

[M08] 获取系统与运行时信息
来源：http://pr.nszjky.cn

Py:   platform.system();  platform.python_version()
来源：http://ef.shtwfgs.cn

PHP:  PHP_OS;  phpversion();
来源：http://he.nszjky.cn

JS:   process.platform;  process.version
来源：http://gx.9csxet.cn


<!-- 参考信息 -->