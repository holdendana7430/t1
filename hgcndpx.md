代发 wailian999

Go:   time.Now()
来源：http://cd.huixinmuqiang.cn

Ruby: Time.now
来源：http://zp.haigaiapp.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lk.nszjky.cn

[J02] 格式化输出
来源：http://og.shtwfgs.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mg.panjiajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xb.newstarts.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vh.colortex.cn

TS:   d.toISOString()
来源：http://kw.colortex.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://aj.gzmigu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://el.lnxyls.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://da.szxytkj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qo.gzmigu.cn

[J03] 字符串解析为日期
来源：http://io.muxihuayi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://po.9csxet.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sc.panjiajie.cn

JS:   new Date("2024-01-02")
来源：http://mn.asd995.cn

TS:   new Date("2024-01-02")
来源：http://qi.newstarts.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ee.bookmarksfly.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://up.szsharing.cn

Ruby: Date.parse("2024-01-02")
来源：http://lc.colortex.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ao.shtwfgs.cn

[J04] 时间戳与日期互转
来源：http://db.shxzukj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yv.huanxung.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hl.szxytkj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ff.haigaiapp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qb.shtwfgs.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qc.yuntaijiaju.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://az.9csxet.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://to.yuntaijiaju.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cb.hnjuh.cn

[J05] 时间加减（加 7 天）
来源：http://kq.szsharing.cn

Py:   now + timedelta(days=7)
来源：http://gq.9csxet.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yp.haigaiapp.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pq.521024.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wt.asd995.cn

Java: LocalDate.now().plusDays(7)
来源：http://qz.colortex.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qs.hahajie.cn

Ruby: Time.now + 7 * 86400
来源：http://dy.yuexingan06.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jt.shxzukj.cn

[J06] 计算两时间之差
来源：http://gb.haigaiapp.cn

Py:   (end - start).total_seconds()
来源：http://sz.huanxung.cn

PHP:  $end->diff($start)->days;
来源：http://fp.chemitech.net.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fa.haigaiapp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bb.9csxet.cn

Java: Duration.between(start, end).toSeconds()
来源：http://tr.yuexingan06.cn

Go:   end.Sub(start).Hours()
来源：http://bt.yuexingan06.cn

Ruby: end - start                 # 返回秒数
来源：http://wg.haigaiapp.cn

C#:   (end - start).TotalSeconds
来源：http://ox.szxytkj.cn

[J07] 比较两个日期
来源：http://mj.lnxyls.cn

Py:   d1 < d2;  d1 == d2
来源：http://by.hahajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lz.nszjky.cn

JS:   d1.getTime() < d2.getTime()
来源：http://nq.szxytkj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://cj.huixiangedu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://iu.9csxet.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lo.panjiajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vl.nszjky.cn

C#:   d1 < d2;  d1 == d2
来源：http://ie.nicolike.cn

[J08] 提取年月日与星期
来源：http://vt.lnxyls.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://el.nicolike.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vx.521024.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lp.hahajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nr.yuexingan06.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pw.nicolike.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pw.hahajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ye.szxytkj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://je.bookmarksfly.cn

[J09] 时区处理
来源：http://xc.bjjhwx.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ny.huanxung.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qx.haigaiapp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ss.9csxet.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://go.hahajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ms.wgjwhj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vg.colortex.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tr.colortex.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nl.szxytkj.cn

[J10] 取今天 / 本月第一天
来源：http://wq.chemitech.net.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://si.gzmigu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fj.nszjky.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rx.newstarts.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gv.bjjhwx.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://za.shxzukj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ks.shtwfgs.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yw.bjjhwx.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nv.jctech888.com.cn

================================================================================
来源：http://vm.yuexingan06.cn

K. JSON 与序列化
来源：http://ei.lnxyls.cn

================================================================================
来源：http://kh.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://zm.huixiangedu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tp.jctech888.com.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yu.yuntaijiaju.cn

JS:   JSON.stringify(obj)
来源：http://ht.nszjky.cn

TS:   JSON.stringify(obj)
来源：http://ue.shxzukj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ro.shxzukj.cn

Go:   json.Marshal(obj)
来源：http://ww.jctech888.com.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qu.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vb.chemitech.net.cn

[K02] JSON 字符串转对象
来源：http://eh.haigaiapp.cn

Py:   json.loads(s)
来源：http://xg.shtwfgs.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bf.9csxet.cn

JS:   JSON.parse(s)
来源：http://kb.nicolike.cn

TS:   JSON.parse(s)
来源：http://zi.szsharing.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uq.muxihuayi.cn

Go:   json.Unmarshal(data, &v)
来源：http://nc.hnjuh.cn

Ruby: JSON.parse(s)
来源：http://td.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nr.gzmigu.cn

[K03] JSON 美化输出（带缩进）
来源：http://us.yuexingan06.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jj.chemitech.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yg.huanxung.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dy.hahajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ks.huanxung.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pl.nicolike.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oi.bjjhwx.cn

Ruby: JSON.pretty_generate(obj)
来源：http://yu.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://si.asd995.cn

[K04] 读取 JSON 文件
来源：http://if.asd995.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rd.9csxet.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dp.yuexingan06.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://um.lnxyls.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yt.muxihuayi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zk.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kh.huixiangedu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fo.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ih.asd995.cn

[K05] 深拷贝对象
来源：http://cl.jctech888.com.cn

Py:   copy.deepcopy(obj)
来源：http://aj.colortex.cn

PHP:  unserialize(serialize($obj));
来源：http://ha.colortex.cn

JS:   structuredClone(obj)
来源：http://lw.shxzukj.cn

TS:   structuredClone(obj)
来源：http://ts.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://id.shxzukj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jj.haigaiapp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pi.lnxyls.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wq.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://bx.szxytkj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cl.newstarts.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://my.asd995.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://is.panjiajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fy.shxzukj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tg.huanxung.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://tc.yuexingan06.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hm.muxihuayi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mm.muxihuayi.cn

[K07] 进制转换
来源：http://qc.shtwfgs.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fj.yuexingan06.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tb.huixiangedu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cp.yuexingan06.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mx.521024.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sh.asd995.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qd.shtwfgs.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xf.asd995.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vo.hahajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://sa.szxytkj.cn

Py:   pickle.dumps(obj)
来源：http://nj.nszjky.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://qb.bjjhwx.cn

JS:   v8.serialize(obj)        // Node
来源：http://at.yuntaijiaju.cn

TS:   v8.serialize(obj)        // Node
来源：http://tr.huanxung.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gy.nicolike.cn

Go:   encoding/gob
来源：http://sw.jctech888.com.cn

Ruby: Marshal.dump(obj)
来源：http://xh.asd995.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://eb.nszjky.cn

================================================================================
来源：http://vd.huanxung.cn

L. 网络请求
来源：http://qs.yuntaijiaju.cn

================================================================================
来源：http://zv.hahajie.cn

[L01] 发送 GET 请求
来源：http://wm.hahajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wa.hnjuh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://eh.chemitech.net.cn

JS:   await fetch(url)
来源：http://xy.jctech888.com.cn

TS:   await fetch(url)
来源：http://sj.haigaiapp.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tp.bjjhwx.cn

Go:   resp, err := http.Get(url)
来源：http://uz.9csxet.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://it.bookmarksfly.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bb.shxzskj.cn

[L02] 发送 POST JSON
来源：http://yb.9csxet.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fk.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nr.521024.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jc.yuexingan06.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xk.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qm.gzmigu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qy.jctech888.com.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xa.jianghongdianzi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pw.bjjhwx.cn

[L03] 设置自定义请求头
来源：http://rl.nszjky.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zq.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nc.colortex.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yo.panjiajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ef.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gf.bookmarksfly.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bj.gzmigu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bp.bookmarksfly.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dg.shxzukj.cn

[L04] 设置超时
来源：http://jj.asd995.cn

Py:   requests.get(url, timeout=5)
来源：http://jj.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hu.hahajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qj.chemitech.net.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sf.gzmigu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kl.huanxung.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gn.szxytkj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jy.nicolike.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://in.szsharing.cn

[L05] 上传文件（multipart）
来源：http://xk.shxzskj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lo.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ts.jctech888.com.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bo.bookmarksfly.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ut.chemitech.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zo.bookmarksfly.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://if.huixinmuqiang.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bq.shxzskj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sy.521024.cn

[L06] 解析响应为 JSON
来源：http://ze.521024.cn

Py:   resp.json()
来源：http://rd.haigaiapp.cn

PHP:  json_decode($body, true);
来源：http://ha.asd995.cn

JS:   await resp.json()
来源：http://dh.panjiajie.cn

TS:   await resp.json()
来源：http://dx.shtwfgs.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hk.colortex.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://sb.huanxung.cn

Ruby: JSON.parse(resp.body)
来源：http://zb.shtwfgs.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dx.nicolike.cn

[L07] 处理 HTTP 状态码
来源：http://kv.yuexingan06.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://iu.jianghongdianzi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gn.jianghongdianzi.cn

JS:   resp.ok;  resp.status
来源：http://jl.jctech888.com.cn

TS:   resp.ok;  resp.status
来源：http://zl.huixiangedu.cn

Java: resp.statusCode()
来源：http://db.newstarts.cn

Go:   resp.StatusCode
来源：http://zr.shtwfgs.cn

Ruby: resp.code.to_i
来源：http://wr.shxzukj.cn

C#:   (int)resp.StatusCode
来源：http://sj.huixinmuqiang.cn

[L08] 并发请求多个地址
来源：http://fr.shxzukj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ut.nicolike.cn

PHP:  curl_multi_init() 系列
来源：http://jc.haigaiapp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fp.jianghongdianzi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hx.bjjhwx.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ok.shxzskj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://za.colortex.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pd.bookmarksfly.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lb.panjiajie.cn

================================================================================
来源：http://ei.newstarts.cn

M. 命令行 / 进程 / 环境
来源：http://mj.shxzskj.cn

================================================================================
来源：http://kx.9csxet.cn

[M01] 读取命令行参数
来源：http://hi.huixiangedu.cn

Py:   sys.argv[1:]
来源：http://eq.hahajie.cn

PHP:  $argv;  $argc;
来源：http://ac.jctech888.com.cn

JS:   process.argv.slice(2)
来源：http://pc.9csxet.cn

TS:   process.argv.slice(2)
来源：http://ei.yuexingan06.cn

Java: args 数组（main 方法参数）
来源：http://su.shxzskj.cn

Go:   os.Args[1:]
来源：http://sb.bjjhwx.cn

Ruby: ARGV
来源：http://zf.521024.cn

C#:   args 数组（Main 方法参数）
来源：http://cl.521024.cn

[M02] 读取环境变量
来源：http://gt.nszjky.cn

Py:   os.environ.get("HOME")
来源：http://rb.chemitech.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://as.hnjuh.cn

JS:   process.env.HOME
来源：http://ft.colortex.cn

TS:   process.env.HOME
来源：http://qt.asd995.cn

Java: System.getenv("HOME")
来源：http://on.wgjwhj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lf.shxzskj.cn

Ruby: ENV["HOME"]
来源：http://nw.bookmarksfly.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sq.huixinmuqiang.cn

[M03] 执行外部命令
来源：http://py.asd995.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ii.jianghongdianzi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gl.bookmarksfly.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hq.nicolike.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yr.muxihuayi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gc.bookmarksfly.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://su.hnjuh.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vr.shtwfgs.cn

C#:   Process.Start("ls", "-l");
来源：http://ju.jctech888.com.cn

[M04] 获取当前工作目录
来源：http://tm.gzmigu.cn

Py:   os.getcwd()
来源：http://xe.haigaiapp.cn

PHP:  getcwd();
来源：http://nt.jctech888.com.cn

JS:   process.cwd()
来源：http://kw.jianghongdianzi.cn

TS:   process.cwd()
来源：http://jz.panjiajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://ao.hnjuh.cn

Go:   os.Getwd()
来源：http://hy.nicolike.cn

Ruby: Dir.pwd
来源：http://ec.shtwfgs.cn

C#:   Directory.GetCurrentDirectory()
来源：http://fh.jianghongdianzi.cn

[M05] 设置退出码
来源：http://er.9csxet.cn

Py:   sys.exit(1)
来源：http://we.yuexingan06.cn

PHP:  exit(1);
来源：http://az.nicolike.cn

JS:   process.exit(1)
来源：http://re.huixinmuqiang.cn

TS:   process.exit(1)
来源：http://em.nszjky.cn

Java: System.exit(1)
来源：http://ft.9csxet.cn

Go:   os.Exit(1)
来源：http://tp.szsharing.cn

Ruby: exit 1
来源：http://lb.colortex.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://px.hahajie.cn

[M06] 向标准错误输出
来源：http://zj.shxzukj.cn

Py:   print("err", file=sys.stderr)
来源：http://dy.shxzskj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ma.yuexingan06.cn

JS:   console.error("err")
来源：http://ef.jctech888.com.cn

TS:   console.error("err")
来源：http://dz.newstarts.cn

Java: System.err.println("err")
来源：http://tx.huixinmuqiang.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yi.chemitech.net.cn

Ruby: warn "err"
来源：http://tz.jianghongdianzi.cn

C#:   Console.Error.WriteLine("err")
来源：http://mv.bookmarksfly.cn

[M07] 判断是否为主入口
来源：http://hg.bookmarksfly.cn

Py:   if __name__ == "__main__":
来源：http://zq.newstarts.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mp.chemitech.net.cn

JS:   require.main === module
来源：http://xs.shxzukj.cn

TS:   require.main === module
来源：http://oc.shxzskj.cn

Java: public static void main(String[] args)
来源：http://go.newstarts.cn

Go:   func main()
来源：http://fe.asd995.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://eu.haigaiapp.cn

C#:   static void Main(string[] args)
来源：http://dl.bjjhwx.cn


<!-- 参考信息 -->