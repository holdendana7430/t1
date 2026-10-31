代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ev.jianghongdianzi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cm.shtwfgs.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ds.nicolike.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://io.gzmigu.cn

[J03] 字符串解析为日期
来源：http://ts.jianghongdianzi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fo.colortex.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qr.shxzukj.cn

JS:   new Date("2024-01-02")
来源：http://hh.colortex.cn

TS:   new Date("2024-01-02")
来源：http://rx.jianghongdianzi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://np.haigaiapp.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gk.haigaiapp.cn

Ruby: Date.parse("2024-01-02")
来源：http://km.huixinmuqiang.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xf.jctech888.com.cn

[J04] 时间戳与日期互转
来源：http://mp.yuntaijiaju.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wz.haigaiapp.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://eh.lnxyls.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mk.szxytkj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://eh.huixinmuqiang.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dw.jctech888.com.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://th.colortex.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zb.gzmigu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sx.9csxet.cn

[J05] 时间加减（加 7 天）
来源：http://dv.asd995.cn

Py:   now + timedelta(days=7)
来源：http://fa.huixiangedu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wm.shxzukj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dq.lnxyls.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fs.jctech888.com.cn

Java: LocalDate.now().plusDays(7)
来源：http://nl.huixiangedu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vd.newstarts.cn

Ruby: Time.now + 7 * 86400
来源：http://pp.shxzskj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ng.shxzskj.cn

[J06] 计算两时间之差
来源：http://od.colortex.cn

Py:   (end - start).total_seconds()
来源：http://ek.shxzskj.cn

PHP:  $end->diff($start)->days;
来源：http://nr.chemitech.net.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mb.huanxung.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pg.huanxung.cn

Java: Duration.between(start, end).toSeconds()
来源：http://tc.yuexingan06.cn

Go:   end.Sub(start).Hours()
来源：http://hf.shxzukj.cn

Ruby: end - start                 # 返回秒数
来源：http://bq.hahajie.cn

C#:   (end - start).TotalSeconds
来源：http://kf.huanxung.cn

[J07] 比较两个日期
来源：http://rb.9csxet.cn

Py:   d1 < d2;  d1 == d2
来源：http://ym.colortex.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jj.shtwfgs.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jk.haigaiapp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ze.chemitech.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dm.asd995.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mf.shtwfgs.cn

Ruby: d1 < d2;  d1 == d2
来源：http://df.hahajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://oq.jianghongdianzi.cn

[J08] 提取年月日与星期
来源：http://dy.nicolike.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tv.jctech888.com.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oy.bookmarksfly.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://do.haigaiapp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cn.newstarts.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pw.hnjuh.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ro.lnxyls.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://in.yuexingan06.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vy.muxihuayi.cn

[J09] 时区处理
来源：http://zh.newstarts.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://di.huixinmuqiang.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://aj.9csxet.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sf.9csxet.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zr.asd995.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xk.nicolike.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wh.szxytkj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://dn.bjjhwx.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pq.bjjhwx.cn

[J10] 取今天 / 本月第一天
来源：http://sp.hnjuh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ps.wgjwhj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://eh.haigaiapp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ic.lnxyls.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kb.wgjwhj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://eb.9csxet.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://de.gzmigu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tl.yuntaijiaju.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qp.9csxet.cn

================================================================================
来源：http://fb.yuexingan06.cn

K. JSON 与序列化
来源：http://xm.yuntaijiaju.cn

================================================================================
来源：http://ra.muxihuayi.cn

[K01] 对象转 JSON 字符串
来源：http://cx.huixiangedu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rp.chemitech.net.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ld.huixiangedu.cn

JS:   JSON.stringify(obj)
来源：http://uh.hahajie.cn

TS:   JSON.stringify(obj)
来源：http://on.shxzskj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://eb.colortex.cn

Go:   json.Marshal(obj)
来源：http://yv.haigaiapp.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fg.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fw.haigaiapp.cn

[K02] JSON 字符串转对象
来源：http://fe.bookmarksfly.cn

Py:   json.loads(s)
来源：http://os.hahajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://in.9csxet.cn

JS:   JSON.parse(s)
来源：http://mb.shxzskj.cn

TS:   JSON.parse(s)
来源：http://tj.newstarts.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://st.szxytkj.cn

Go:   json.Unmarshal(data, &v)
来源：http://fa.yuntaijiaju.cn

Ruby: JSON.parse(s)
来源：http://xa.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hd.yuexingan06.cn

[K03] JSON 美化输出（带缩进）
来源：http://ak.jianghongdianzi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qb.bookmarksfly.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zl.panjiajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://es.shxzukj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://oz.bjjhwx.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kh.yuntaijiaju.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gl.hnjuh.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dt.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xp.shxzskj.cn

[K04] 读取 JSON 文件
来源：http://hb.jctech888.com.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dz.szsharing.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fj.yuntaijiaju.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oa.szsharing.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wl.jianghongdianzi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bw.colortex.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yh.jianghongdianzi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qr.asd995.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jh.haigaiapp.cn

[K05] 深拷贝对象
来源：http://vo.yuntaijiaju.cn

Py:   copy.deepcopy(obj)
来源：http://qo.muxihuayi.cn

PHP:  unserialize(serialize($obj));
来源：http://tl.muxihuayi.cn

JS:   structuredClone(obj)
来源：http://ye.jctech888.com.cn

TS:   structuredClone(obj)
来源：http://de.521024.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ux.wgjwhj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dv.jianghongdianzi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uo.huixinmuqiang.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xz.hnjuh.cn

[K06] 解析 URL 查询串
来源：http://co.shxzskj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ww.hahajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mb.asd995.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://be.huixinmuqiang.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xw.szsharing.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zj.szsharing.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cv.newstarts.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ab.hahajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ak.panjiajie.cn

[K07] 进制转换
来源：http://la.jianghongdianzi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vl.bookmarksfly.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bb.huixiangedu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://am.hahajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ku.bjjhwx.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kv.huixinmuqiang.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fe.haigaiapp.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lw.shtwfgs.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rg.jctech888.com.cn

[K08] 二进制序列化（非 JSON）
来源：http://vz.yuexingan06.cn

Py:   pickle.dumps(obj)
来源：http://wd.chemitech.net.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fl.huixinmuqiang.cn

JS:   v8.serialize(obj)        // Node
来源：http://yy.yuntaijiaju.cn

TS:   v8.serialize(obj)        // Node
来源：http://jw.wgjwhj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nj.hahajie.cn

Go:   encoding/gob
来源：http://cf.hnjuh.cn

Ruby: Marshal.dump(obj)
来源：http://zt.nicolike.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wz.yuntaijiaju.cn

================================================================================
来源：http://ep.asd995.cn

L. 网络请求
来源：http://nr.shxzskj.cn

================================================================================
来源：http://nd.muxihuayi.cn

[L01] 发送 GET 请求
来源：http://ju.shxzskj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sp.nszjky.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jk.hahajie.cn

JS:   await fetch(url)
来源：http://bk.hahajie.cn

TS:   await fetch(url)
来源：http://kl.bookmarksfly.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://du.huanxung.cn

Go:   resp, err := http.Get(url)
来源：http://ov.yuntaijiaju.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dt.shtwfgs.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rt.colortex.cn

[L02] 发送 POST JSON
来源：http://me.szsharing.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cs.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dp.szsharing.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fc.nszjky.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vv.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rf.521024.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uu.hnjuh.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.shxzskj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://se.shtwfgs.cn

[L03] 设置自定义请求头
来源：http://jy.nszjky.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gx.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gy.newstarts.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kd.shtwfgs.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kp.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qy.yuexingan06.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wm.muxihuayi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://aq.hahajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uy.muxihuayi.cn

[L04] 设置超时
来源：http://px.jctech888.com.cn

Py:   requests.get(url, timeout=5)
来源：http://yi.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yq.lnxyls.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yc.panjiajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://do.gzmigu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tj.huixiangedu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mf.hahajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://th.huanxung.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://is.huanxung.cn

[L05] 上传文件（multipart）
来源：http://ea.huixiangedu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fg.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ch.nszjky.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ra.jctech888.com.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://iq.muxihuayi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gn.gzmigu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bt.shxzskj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gg.9csxet.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rx.haigaiapp.cn

[L06] 解析响应为 JSON
来源：http://rq.huixiangedu.cn

Py:   resp.json()
来源：http://nl.521024.cn

PHP:  json_decode($body, true);
来源：http://ut.colortex.cn

JS:   await resp.json()
来源：http://ig.521024.cn

TS:   await resp.json()
来源：http://gp.nszjky.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gj.lnxyls.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ry.szsharing.cn

Ruby: JSON.parse(resp.body)
来源：http://vr.jianghongdianzi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jb.9csxet.cn

[L07] 处理 HTTP 状态码
来源：http://ra.huixiangedu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ep.bookmarksfly.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ed.shxzukj.cn

JS:   resp.ok;  resp.status
来源：http://nc.wgjwhj.cn

TS:   resp.ok;  resp.status
来源：http://vu.hnjuh.cn

Java: resp.statusCode()
来源：http://qj.newstarts.cn

Go:   resp.StatusCode
来源：http://uk.yuntaijiaju.cn

Ruby: resp.code.to_i
来源：http://st.huixiangedu.cn

C#:   (int)resp.StatusCode
来源：http://ub.lnxyls.cn

[L08] 并发请求多个地址
来源：http://bw.hahajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dz.asd995.cn

PHP:  curl_multi_init() 系列
来源：http://na.wgjwhj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xw.shxzukj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zv.lnxyls.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ej.lnxyls.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pc.521024.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://or.521024.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bv.jctech888.com.cn

================================================================================
来源：http://ok.haigaiapp.cn

M. 命令行 / 进程 / 环境
来源：http://ti.nicolike.cn

================================================================================
来源：http://zk.szxytkj.cn

[M01] 读取命令行参数
来源：http://zd.panjiajie.cn

Py:   sys.argv[1:]
来源：http://yb.szxytkj.cn

PHP:  $argv;  $argc;
来源：http://mj.jianghongdianzi.cn

JS:   process.argv.slice(2)
来源：http://et.gzmigu.cn

TS:   process.argv.slice(2)
来源：http://bo.newstarts.cn

Java: args 数组（main 方法参数）
来源：http://vu.muxihuayi.cn

Go:   os.Args[1:]
来源：http://zv.panjiajie.cn

Ruby: ARGV
来源：http://ve.chemitech.net.cn

C#:   args 数组（Main 方法参数）
来源：http://kw.chemitech.net.cn

[M02] 读取环境变量
来源：http://jl.newstarts.cn

Py:   os.environ.get("HOME")
来源：http://xe.huixiangedu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qg.lnxyls.cn

JS:   process.env.HOME
来源：http://gr.hnjuh.cn

TS:   process.env.HOME
来源：http://dx.9csxet.cn

Java: System.getenv("HOME")
来源：http://xd.shxzskj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tv.jianghongdianzi.cn

Ruby: ENV["HOME"]
来源：http://kx.bookmarksfly.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bf.chemitech.net.cn

[M03] 执行外部命令
来源：http://xr.hnjuh.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://us.bjjhwx.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jm.hnjuh.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gq.chemitech.net.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://dk.asd995.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nx.jctech888.com.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://of.chemitech.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://du.huixiangedu.cn

C#:   Process.Start("ls", "-l");
来源：http://oq.haigaiapp.cn

[M04] 获取当前工作目录
来源：http://mf.hnjuh.cn

Py:   os.getcwd()
来源：http://qw.9csxet.cn

PHP:  getcwd();
来源：http://zj.szsharing.cn

JS:   process.cwd()
来源：http://qk.jctech888.com.cn

TS:   process.cwd()
来源：http://gz.jctech888.com.cn

Java: Path.of("").toAbsolutePath()
来源：http://oe.shxzskj.cn

Go:   os.Getwd()
来源：http://qj.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://ct.gzmigu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hj.hahajie.cn

[M05] 设置退出码
来源：http://so.huixinmuqiang.cn

Py:   sys.exit(1)
来源：http://aq.asd995.cn

PHP:  exit(1);
来源：http://rp.shxzukj.cn

JS:   process.exit(1)
来源：http://zk.gzmigu.cn

TS:   process.exit(1)
来源：http://cs.gzmigu.cn

Java: System.exit(1)
来源：http://di.hnjuh.cn

Go:   os.Exit(1)
来源：http://wc.jianghongdianzi.cn

Ruby: exit 1
来源：http://wj.szxytkj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mi.bjjhwx.cn

[M06] 向标准错误输出
来源：http://qu.szxytkj.cn

Py:   print("err", file=sys.stderr)
来源：http://cy.hnjuh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://np.bookmarksfly.cn

JS:   console.error("err")
来源：http://bl.nszjky.cn

TS:   console.error("err")
来源：http://no.hahajie.cn

Java: System.err.println("err")
来源：http://oz.lnxyls.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ji.panjiajie.cn

Ruby: warn "err"
来源：http://yx.huanxung.cn

C#:   Console.Error.WriteLine("err")
来源：http://nw.hnjuh.cn

[M07] 判断是否为主入口
来源：http://hg.nicolike.cn

Py:   if __name__ == "__main__":
来源：http://rl.hahajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kv.huixiangedu.cn

JS:   require.main === module
来源：http://bp.huixiangedu.cn

TS:   require.main === module
来源：http://sb.chemitech.net.cn

Java: public static void main(String[] args)
来源：http://ic.nszjky.cn

Go:   func main()
来源：http://cw.lnxyls.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mq.nszjky.cn

C#:   static void Main(string[] args)
来源：http://kt.newstarts.cn

[M08] 获取系统与运行时信息
来源：http://mn.huixiangedu.cn

Py:   platform.system();  platform.python_version()
来源：http://xu.asd995.cn

PHP:  PHP_OS;  phpversion();
来源：http://we.yuexingan06.cn

JS:   process.platform;  process.version
来源：http://os.hahajie.cn

TS:   process.platform;  process.version
来源：http://rz.yuntaijiaju.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jw.bjjhwx.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ge.shtwfgs.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sz.jianghongdianzi.cn


<!-- 参考信息 -->