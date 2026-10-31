代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xx.9csxet.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zs.huanxung.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ra.szsharing.cn

TS:   d.toISOString()
来源：http://vd.yuexingan06.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sx.nicolike.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vq.bookmarksfly.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gq.jianghongdianzi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pb.521024.cn

[J03] 字符串解析为日期
来源：http://ig.lnxyls.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bf.colortex.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mq.muxihuayi.cn

JS:   new Date("2024-01-02")
来源：http://oy.panjiajie.cn

TS:   new Date("2024-01-02")
来源：http://in.yuntaijiaju.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mh.shtwfgs.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fa.huixiangedu.cn

Ruby: Date.parse("2024-01-02")
来源：http://ln.haigaiapp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ds.haigaiapp.cn

[J04] 时间戳与日期互转
来源：http://at.yuexingan06.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wn.yuexingan06.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xz.newstarts.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ly.muxihuayi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bp.newstarts.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nv.bjjhwx.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gs.hnjuh.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kd.9csxet.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zq.haigaiapp.cn

[J05] 时间加减（加 7 天）
来源：http://lm.newstarts.cn

Py:   now + timedelta(days=7)
来源：http://dc.bjjhwx.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://fx.nicolike.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ko.panjiajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uq.szxytkj.cn

Java: LocalDate.now().plusDays(7)
来源：http://ap.yuntaijiaju.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://er.hahajie.cn

Ruby: Time.now + 7 * 86400
来源：http://vs.asd995.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bh.wgjwhj.cn

[J06] 计算两时间之差
来源：http://gb.9csxet.cn

Py:   (end - start).total_seconds()
来源：http://eh.9csxet.cn

PHP:  $end->diff($start)->days;
来源：http://hk.asd995.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ta.muxihuayi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hs.yuexingan06.cn

Java: Duration.between(start, end).toSeconds()
来源：http://tt.9csxet.cn

Go:   end.Sub(start).Hours()
来源：http://dd.shtwfgs.cn

Ruby: end - start                 # 返回秒数
来源：http://yz.szxytkj.cn

C#:   (end - start).TotalSeconds
来源：http://ni.colortex.cn

[J07] 比较两个日期
来源：http://io.muxihuayi.cn

Py:   d1 < d2;  d1 == d2
来源：http://mw.bjjhwx.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lh.asd995.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ua.bookmarksfly.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ur.hahajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qe.hahajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tq.nszjky.cn

Ruby: d1 < d2;  d1 == d2
来源：http://sy.huixinmuqiang.cn

C#:   d1 < d2;  d1 == d2
来源：http://zc.shtwfgs.cn

[J08] 提取年月日与星期
来源：http://cb.bjjhwx.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nu.hnjuh.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yl.asd995.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yi.hahajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zt.huanxung.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nt.asd995.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rs.asd995.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dv.nszjky.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://re.nszjky.cn

[J09] 时区处理
来源：http://zk.huixinmuqiang.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zg.yuntaijiaju.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ks.shxzukj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://az.szxytkj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xu.shxzskj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ni.shxzukj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nb.huixinmuqiang.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ky.wgjwhj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ff.huixinmuqiang.cn

[J10] 取今天 / 本月第一天
来源：http://me.szsharing.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ha.gzmigu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bd.bookmarksfly.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ve.newstarts.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xp.yuntaijiaju.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qp.colortex.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uy.nszjky.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xe.szsharing.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dk.bjjhwx.cn

================================================================================
来源：http://bo.huixiangedu.cn

K. JSON 与序列化
来源：http://hp.asd995.cn

================================================================================
来源：http://eu.521024.cn

[K01] 对象转 JSON 字符串
来源：http://eb.colortex.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kx.yuexingan06.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://am.hahajie.cn

JS:   JSON.stringify(obj)
来源：http://hq.szsharing.cn

TS:   JSON.stringify(obj)
来源：http://wh.huixinmuqiang.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bu.wgjwhj.cn

Go:   json.Marshal(obj)
来源：http://il.wgjwhj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ku.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qy.jctech888.com.cn

[K02] JSON 字符串转对象
来源：http://it.hnjuh.cn

Py:   json.loads(s)
来源：http://pg.shxzskj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kw.haigaiapp.cn

JS:   JSON.parse(s)
来源：http://ja.nicolike.cn

TS:   JSON.parse(s)
来源：http://av.shxzskj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wp.huixinmuqiang.cn

Go:   json.Unmarshal(data, &v)
来源：http://uq.asd995.cn

Ruby: JSON.parse(s)
来源：http://xl.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ct.huixiangedu.cn

[K03] JSON 美化输出（带缩进）
来源：http://lu.jianghongdianzi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bl.haigaiapp.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ey.521024.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dk.521024.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://pt.bjjhwx.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rz.lnxyls.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ta.huanxung.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hw.hnjuh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yo.jianghongdianzi.cn

[K04] 读取 JSON 文件
来源：http://xi.shxzukj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xy.nszjky.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wu.wgjwhj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pv.muxihuayi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://db.huixiangedu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pr.newstarts.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ni.hnjuh.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wx.asd995.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://av.asd995.cn

[K05] 深拷贝对象
来源：http://do.yuexingan06.cn

Py:   copy.deepcopy(obj)
来源：http://dn.jianghongdianzi.cn

PHP:  unserialize(serialize($obj));
来源：http://fe.chemitech.net.cn

JS:   structuredClone(obj)
来源：http://am.colortex.cn

TS:   structuredClone(obj)
来源：http://st.szsharing.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://cd.9csxet.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kj.szxytkj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nw.chemitech.net.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pk.panjiajie.cn

[K06] 解析 URL 查询串
来源：http://qj.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yj.szsharing.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pr.shxzukj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kz.huixiangedu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vc.9csxet.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nv.huanxung.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fs.asd995.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fi.shxzskj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jg.huanxung.cn

[K07] 进制转换
来源：http://qi.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ze.bookmarksfly.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ob.haigaiapp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vu.haigaiapp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dw.nszjky.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qi.muxihuayi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bx.bjjhwx.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uy.yuexingan06.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://il.bookmarksfly.cn

[K08] 二进制序列化（非 JSON）
来源：http://ur.jianghongdianzi.cn

Py:   pickle.dumps(obj)
来源：http://rn.521024.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cr.haigaiapp.cn

JS:   v8.serialize(obj)        // Node
来源：http://xx.jctech888.com.cn

TS:   v8.serialize(obj)        // Node
来源：http://xf.521024.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ya.bookmarksfly.cn

Go:   encoding/gob
来源：http://wx.panjiajie.cn

Ruby: Marshal.dump(obj)
来源：http://ee.yuntaijiaju.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://je.lnxyls.cn

================================================================================
来源：http://ea.nicolike.cn

L. 网络请求
来源：http://hc.nszjky.cn

================================================================================
来源：http://xt.huanxung.cn

[L01] 发送 GET 请求
来源：http://up.haigaiapp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cq.521024.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cl.gzmigu.cn

JS:   await fetch(url)
来源：http://lj.newstarts.cn

TS:   await fetch(url)
来源：http://xq.hnjuh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ex.nicolike.cn

Go:   resp, err := http.Get(url)
来源：http://zm.newstarts.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://df.huanxung.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bq.shxzskj.cn

[L02] 发送 POST JSON
来源：http://mn.huanxung.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xx.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qp.hnjuh.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://if.huixinmuqiang.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ue.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vn.nszjky.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nc.wgjwhj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bn.9csxet.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://er.shxzukj.cn

[L03] 设置自定义请求头
来源：http://vw.huanxung.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sq.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hj.nicolike.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nu.gzmigu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ql.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ab.jianghongdianzi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nb.shxzskj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xr.huixinmuqiang.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vx.huanxung.cn

[L04] 设置超时
来源：http://ap.chemitech.net.cn

Py:   requests.get(url, timeout=5)
来源：http://si.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gx.shtwfgs.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hv.haigaiapp.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dd.lnxyls.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kr.9csxet.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pd.asd995.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jl.shxzukj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hh.hnjuh.cn

[L05] 上传文件（multipart）
来源：http://sv.hahajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mt.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fk.yuexingan06.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cg.huixiangedu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://du.bjjhwx.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ze.chemitech.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://so.lnxyls.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uv.jctech888.com.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hg.jctech888.com.cn

[L06] 解析响应为 JSON
来源：http://jf.yuexingan06.cn

Py:   resp.json()
来源：http://pe.gzmigu.cn

PHP:  json_decode($body, true);
来源：http://ir.huanxung.cn

JS:   await resp.json()
来源：http://mp.jianghongdianzi.cn

TS:   await resp.json()
来源：http://it.lnxyls.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bq.hahajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ak.jianghongdianzi.cn

Ruby: JSON.parse(resp.body)
来源：http://sw.newstarts.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://na.yuntaijiaju.cn

[L07] 处理 HTTP 状态码
来源：http://kh.nicolike.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lb.panjiajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cz.chemitech.net.cn

JS:   resp.ok;  resp.status
来源：http://pq.yuexingan06.cn

TS:   resp.ok;  resp.status
来源：http://pb.newstarts.cn

Java: resp.statusCode()
来源：http://zr.huixinmuqiang.cn

Go:   resp.StatusCode
来源：http://vm.wgjwhj.cn

Ruby: resp.code.to_i
来源：http://rf.yuntaijiaju.cn

C#:   (int)resp.StatusCode
来源：http://vl.nicolike.cn

[L08] 并发请求多个地址
来源：http://sj.nicolike.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xb.nszjky.cn

PHP:  curl_multi_init() 系列
来源：http://xn.newstarts.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ve.haigaiapp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oj.huixiangedu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qh.bjjhwx.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xm.yuexingan06.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yk.bjjhwx.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fl.lnxyls.cn

================================================================================
来源：http://lt.yuntaijiaju.cn

M. 命令行 / 进程 / 环境
来源：http://lu.lnxyls.cn

================================================================================
来源：http://li.szxytkj.cn

[M01] 读取命令行参数
来源：http://hv.jianghongdianzi.cn

Py:   sys.argv[1:]
来源：http://cu.panjiajie.cn

PHP:  $argv;  $argc;
来源：http://kf.chemitech.net.cn

JS:   process.argv.slice(2)
来源：http://bn.haigaiapp.cn

TS:   process.argv.slice(2)
来源：http://fl.szxytkj.cn

Java: args 数组（main 方法参数）
来源：http://wy.colortex.cn

Go:   os.Args[1:]
来源：http://fm.hahajie.cn

Ruby: ARGV
来源：http://pc.szxytkj.cn

C#:   args 数组（Main 方法参数）
来源：http://sf.521024.cn

[M02] 读取环境变量
来源：http://or.szsharing.cn

Py:   os.environ.get("HOME")
来源：http://fw.521024.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://af.9csxet.cn

JS:   process.env.HOME
来源：http://na.newstarts.cn

TS:   process.env.HOME
来源：http://uk.nszjky.cn

Java: System.getenv("HOME")
来源：http://bf.haigaiapp.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ml.chemitech.net.cn

Ruby: ENV["HOME"]
来源：http://cf.shxzukj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://aa.colortex.cn

[M03] 执行外部命令
来源：http://js.hahajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yw.hahajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yy.9csxet.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://lp.nszjky.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ex.huixiangedu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://by.huixiangedu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mr.9csxet.cn

Ruby: system("ls -l");  `ls -l`
来源：http://sq.huanxung.cn

C#:   Process.Start("ls", "-l");
来源：http://db.shtwfgs.cn

[M04] 获取当前工作目录
来源：http://lr.muxihuayi.cn

Py:   os.getcwd()
来源：http://wa.jctech888.com.cn

PHP:  getcwd();
来源：http://th.huixiangedu.cn

JS:   process.cwd()
来源：http://zw.bjjhwx.cn

TS:   process.cwd()
来源：http://iy.shxzskj.cn

Java: Path.of("").toAbsolutePath()
来源：http://hf.chemitech.net.cn

Go:   os.Getwd()
来源：http://pl.muxihuayi.cn

Ruby: Dir.pwd
来源：http://nq.huixinmuqiang.cn

C#:   Directory.GetCurrentDirectory()
来源：http://at.huixiangedu.cn

[M05] 设置退出码
来源：http://dx.huixinmuqiang.cn

Py:   sys.exit(1)
来源：http://co.hahajie.cn

PHP:  exit(1);
来源：http://if.chemitech.net.cn

JS:   process.exit(1)
来源：http://vv.huanxung.cn

TS:   process.exit(1)
来源：http://kf.newstarts.cn

Java: System.exit(1)
来源：http://hn.yuntaijiaju.cn

Go:   os.Exit(1)
来源：http://bv.521024.cn

Ruby: exit 1
来源：http://hr.huanxung.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yr.lnxyls.cn

[M06] 向标准错误输出
来源：http://oe.jianghongdianzi.cn

Py:   print("err", file=sys.stderr)
来源：http://rf.hahajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tr.haigaiapp.cn

JS:   console.error("err")
来源：http://qa.hahajie.cn

TS:   console.error("err")
来源：http://gy.shtwfgs.cn

Java: System.err.println("err")
来源：http://xs.wgjwhj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pj.shxzskj.cn

Ruby: warn "err"
来源：http://ts.huanxung.cn

C#:   Console.Error.WriteLine("err")
来源：http://zk.wgjwhj.cn

[M07] 判断是否为主入口
来源：http://hp.huanxung.cn

Py:   if __name__ == "__main__":
来源：http://pm.newstarts.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qc.muxihuayi.cn

JS:   require.main === module
来源：http://mw.hahajie.cn

TS:   require.main === module
来源：http://eo.huixiangedu.cn

Java: public static void main(String[] args)
来源：http://dm.huixiangedu.cn

Go:   func main()
来源：http://ja.jctech888.com.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ln.yuexingan06.cn

C#:   static void Main(string[] args)
来源：http://sa.yuexingan06.cn

[M08] 获取系统与运行时信息
来源：http://jn.asd995.cn

Py:   platform.system();  platform.python_version()
来源：http://qd.nszjky.cn

PHP:  PHP_OS;  phpversion();
来源：http://mr.szxytkj.cn

JS:   process.platform;  process.version
来源：http://qh.panjiajie.cn


<!-- 参考信息 -->