代发 wailian999

Go:   time.Now()
来源：http://bn.huixiangedu.cn

Ruby: Time.now
来源：http://mg.lnxyls.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mc.haigaiapp.cn

[J02] 格式化输出
来源：http://yt.gzmigu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tz.shxzukj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ms.colortex.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ld.hnjuh.cn

TS:   d.toISOString()
来源：http://by.shxzukj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yx.shtwfgs.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://py.newstarts.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ak.shxzukj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mx.521024.cn

[J03] 字符串解析为日期
来源：http://ia.jctech888.com.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://es.panjiajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://br.shxzskj.cn

JS:   new Date("2024-01-02")
来源：http://li.huixiangedu.cn

TS:   new Date("2024-01-02")
来源：http://fz.colortex.cn

Java: LocalDate.parse("2024-01-02")
来源：http://uy.colortex.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zi.asd995.cn

Ruby: Date.parse("2024-01-02")
来源：http://tm.nicolike.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ve.bjjhwx.cn

[J04] 时间戳与日期互转
来源：http://en.jctech888.com.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qy.yuexingan06.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hb.huanxung.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ql.szsharing.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bi.shxzskj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qm.jctech888.com.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zj.huixiangedu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ot.shxzskj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ph.chemitech.net.cn

[J05] 时间加减（加 7 天）
来源：http://vz.jianghongdianzi.cn

Py:   now + timedelta(days=7)
来源：http://zd.panjiajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qj.yuntaijiaju.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cb.yuexingan06.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rl.gzmigu.cn

Java: LocalDate.now().plusDays(7)
来源：http://gn.yuexingan06.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lq.gzmigu.cn

Ruby: Time.now + 7 * 86400
来源：http://wd.asd995.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hb.haigaiapp.cn

[J06] 计算两时间之差
来源：http://jv.chemitech.net.cn

Py:   (end - start).total_seconds()
来源：http://so.lnxyls.cn

PHP:  $end->diff($start)->days;
来源：http://bp.panjiajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sa.szxytkj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sg.wgjwhj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://go.huixinmuqiang.cn

Go:   end.Sub(start).Hours()
来源：http://hx.jctech888.com.cn

Ruby: end - start                 # 返回秒数
来源：http://km.yuexingan06.cn

C#:   (end - start).TotalSeconds
来源：http://ar.haigaiapp.cn

[J07] 比较两个日期
来源：http://hj.asd995.cn

Py:   d1 < d2;  d1 == d2
来源：http://hx.bjjhwx.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://si.szxytkj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gc.shxzskj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gf.muxihuayi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://at.chemitech.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cw.huixinmuqiang.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mb.szsharing.cn

C#:   d1 < d2;  d1 == d2
来源：http://qr.bjjhwx.cn

[J08] 提取年月日与星期
来源：http://mh.huixinmuqiang.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nt.hahajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oy.asd995.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vu.hnjuh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mk.haigaiapp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vs.haigaiapp.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zs.asd995.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lo.yuntaijiaju.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tt.shtwfgs.cn

[J09] 时区处理
来源：http://il.shxzskj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nh.521024.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lx.shxzskj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://um.hahajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://er.hnjuh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dh.yuntaijiaju.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://eu.szxytkj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://by.huixiangedu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://px.asd995.cn

[J10] 取今天 / 本月第一天
来源：http://px.haigaiapp.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gv.szxytkj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gg.huixinmuqiang.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ug.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://eg.yuntaijiaju.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bd.wgjwhj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sm.colortex.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uj.szxytkj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ut.chemitech.net.cn

================================================================================
来源：http://pr.yuntaijiaju.cn

K. JSON 与序列化
来源：http://qe.lnxyls.cn

================================================================================
来源：http://bc.newstarts.cn

[K01] 对象转 JSON 字符串
来源：http://lk.gzmigu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bg.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yt.bookmarksfly.cn

JS:   JSON.stringify(obj)
来源：http://te.lnxyls.cn

TS:   JSON.stringify(obj)
来源：http://ud.huixiangedu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jb.shtwfgs.cn

Go:   json.Marshal(obj)
来源：http://sd.hnjuh.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zf.nicolike.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://to.521024.cn

[K02] JSON 字符串转对象
来源：http://yu.szxytkj.cn

Py:   json.loads(s)
来源：http://fq.521024.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zp.bookmarksfly.cn

JS:   JSON.parse(s)
来源：http://am.muxihuayi.cn

TS:   JSON.parse(s)
来源：http://iy.hnjuh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fo.huixinmuqiang.cn

Go:   json.Unmarshal(data, &v)
来源：http://xk.shxzskj.cn

Ruby: JSON.parse(s)
来源：http://vi.521024.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gu.panjiajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://ne.wgjwhj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qx.hahajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pk.gzmigu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pw.bookmarksfly.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://dt.jianghongdianzi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qs.bjjhwx.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vi.jctech888.com.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vm.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fm.shxzukj.cn

[K04] 读取 JSON 文件
来源：http://ue.521024.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ec.521024.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sq.wgjwhj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ej.shxzskj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qh.wgjwhj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://um.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dj.szxytkj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ak.521024.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://of.bookmarksfly.cn

[K05] 深拷贝对象
来源：http://da.shxzskj.cn

Py:   copy.deepcopy(obj)
来源：http://oq.asd995.cn

PHP:  unserialize(serialize($obj));
来源：http://el.nicolike.cn

JS:   structuredClone(obj)
来源：http://at.shtwfgs.cn

TS:   structuredClone(obj)
来源：http://xi.newstarts.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ph.wgjwhj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hb.shxzskj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yc.newstarts.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lw.colortex.cn

[K06] 解析 URL 查询串
来源：http://ni.haigaiapp.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qw.bjjhwx.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tz.wgjwhj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qe.bjjhwx.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xl.szxytkj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bb.lnxyls.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gx.huixiangedu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://br.jctech888.com.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vq.chemitech.net.cn

[K07] 进制转换
来源：http://lu.yuexingan06.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uc.szsharing.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ev.wgjwhj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lc.wgjwhj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yu.lnxyls.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ll.nicolike.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mz.muxihuayi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gl.yuntaijiaju.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fz.nicolike.cn

[K08] 二进制序列化（非 JSON）
来源：http://nl.nicolike.cn

Py:   pickle.dumps(obj)
来源：http://nt.bookmarksfly.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gt.nicolike.cn

JS:   v8.serialize(obj)        // Node
来源：http://ji.9csxet.cn

TS:   v8.serialize(obj)        // Node
来源：http://fk.jctech888.com.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gq.bookmarksfly.cn

Go:   encoding/gob
来源：http://jh.bookmarksfly.cn

Ruby: Marshal.dump(obj)
来源：http://qu.szsharing.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cg.asd995.cn

================================================================================
来源：http://fx.shxzskj.cn

L. 网络请求
来源：http://wm.newstarts.cn

================================================================================
来源：http://qu.szsharing.cn

[L01] 发送 GET 请求
来源：http://zf.521024.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lk.muxihuayi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://su.wgjwhj.cn

JS:   await fetch(url)
来源：http://vj.9csxet.cn

TS:   await fetch(url)
来源：http://ie.szsharing.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://du.haigaiapp.cn

Go:   resp, err := http.Get(url)
来源：http://mz.hnjuh.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://cg.jctech888.com.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://il.gzmigu.cn

[L02] 发送 POST JSON
来源：http://jv.szsharing.cn

Py:   requests.post(url, json={"a": 1})
来源：http://da.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ap.shxzukj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://th.bookmarksfly.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zl.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ry.nicolike.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bh.muxihuayi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nr.huanxung.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dl.yuntaijiaju.cn

[L03] 设置自定义请求头
来源：http://yb.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zn.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lz.lnxyls.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hf.lnxyls.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bj.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://am.haigaiapp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://iv.huixinmuqiang.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qq.shxzskj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ss.hnjuh.cn

[L04] 设置超时
来源：http://mb.panjiajie.cn

Py:   requests.get(url, timeout=5)
来源：http://ik.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ua.gzmigu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tm.shxzskj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eb.yuexingan06.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://oi.nicolike.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yq.gzmigu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lo.szxytkj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ap.panjiajie.cn

[L05] 上传文件（multipart）
来源：http://ba.hahajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mf.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ix.colortex.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mf.yuexingan06.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nv.yuntaijiaju.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kb.panjiajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mg.muxihuayi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qe.hahajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dh.9csxet.cn

[L06] 解析响应为 JSON
来源：http://vn.nicolike.cn

Py:   resp.json()
来源：http://mb.asd995.cn

PHP:  json_decode($body, true);
来源：http://mu.haigaiapp.cn

JS:   await resp.json()
来源：http://qb.szxytkj.cn

TS:   await resp.json()
来源：http://wq.shxzukj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oc.jianghongdianzi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uu.shtwfgs.cn

Ruby: JSON.parse(resp.body)
来源：http://ps.yuexingan06.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qc.muxihuayi.cn

[L07] 处理 HTTP 状态码
来源：http://vp.jianghongdianzi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qa.yuntaijiaju.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://et.nszjky.cn

JS:   resp.ok;  resp.status
来源：http://zm.newstarts.cn

TS:   resp.ok;  resp.status
来源：http://ci.jctech888.com.cn

Java: resp.statusCode()
来源：http://zi.wgjwhj.cn

Go:   resp.StatusCode
来源：http://ez.jianghongdianzi.cn

Ruby: resp.code.to_i
来源：http://lv.shtwfgs.cn

C#:   (int)resp.StatusCode
来源：http://jc.haigaiapp.cn

[L08] 并发请求多个地址
来源：http://db.huixiangedu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pt.asd995.cn

PHP:  curl_multi_init() 系列
来源：http://mq.haigaiapp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sk.wgjwhj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cv.521024.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ld.521024.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hh.shtwfgs.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ej.hahajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ze.shtwfgs.cn

================================================================================
来源：http://yc.lnxyls.cn

M. 命令行 / 进程 / 环境
来源：http://wq.shtwfgs.cn

================================================================================
来源：http://bi.nicolike.cn

[M01] 读取命令行参数
来源：http://bm.nszjky.cn

Py:   sys.argv[1:]
来源：http://nk.bjjhwx.cn

PHP:  $argv;  $argc;
来源：http://qj.hnjuh.cn

JS:   process.argv.slice(2)
来源：http://lz.shxzskj.cn

TS:   process.argv.slice(2)
来源：http://qc.newstarts.cn

Java: args 数组（main 方法参数）
来源：http://fn.521024.cn

Go:   os.Args[1:]
来源：http://bz.gzmigu.cn

Ruby: ARGV
来源：http://ri.asd995.cn

C#:   args 数组（Main 方法参数）
来源：http://bo.muxihuayi.cn

[M02] 读取环境变量
来源：http://pe.shtwfgs.cn

Py:   os.environ.get("HOME")
来源：http://qn.9csxet.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ue.panjiajie.cn

JS:   process.env.HOME
来源：http://du.nicolike.cn

TS:   process.env.HOME
来源：http://uo.gzmigu.cn

Java: System.getenv("HOME")
来源：http://ml.lnxyls.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rt.gzmigu.cn

Ruby: ENV["HOME"]
来源：http://oc.gzmigu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ch.haigaiapp.cn

[M03] 执行外部命令
来源：http://vz.gzmigu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xf.gzmigu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ra.szxytkj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vr.nszjky.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ik.gzmigu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gb.lnxyls.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://sf.lnxyls.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gc.yuexingan06.cn

C#:   Process.Start("ls", "-l");
来源：http://ll.jianghongdianzi.cn

[M04] 获取当前工作目录
来源：http://uv.9csxet.cn

Py:   os.getcwd()
来源：http://pu.huixinmuqiang.cn

PHP:  getcwd();
来源：http://cv.nicolike.cn

JS:   process.cwd()
来源：http://fp.huixinmuqiang.cn

TS:   process.cwd()
来源：http://ys.wgjwhj.cn

Java: Path.of("").toAbsolutePath()
来源：http://ip.bjjhwx.cn

Go:   os.Getwd()
来源：http://kn.gzmigu.cn

Ruby: Dir.pwd
来源：http://nu.yuexingan06.cn

C#:   Directory.GetCurrentDirectory()
来源：http://uf.huixinmuqiang.cn

[M05] 设置退出码
来源：http://zs.shtwfgs.cn

Py:   sys.exit(1)
来源：http://rs.panjiajie.cn

PHP:  exit(1);
来源：http://bz.yuntaijiaju.cn

JS:   process.exit(1)
来源：http://ag.nicolike.cn

TS:   process.exit(1)
来源：http://mj.yuntaijiaju.cn

Java: System.exit(1)
来源：http://ky.muxihuayi.cn

Go:   os.Exit(1)
来源：http://ps.asd995.cn

Ruby: exit 1
来源：http://gk.newstarts.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ff.muxihuayi.cn

[M06] 向标准错误输出
来源：http://je.bookmarksfly.cn

Py:   print("err", file=sys.stderr)
来源：http://br.wgjwhj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jj.chemitech.net.cn

JS:   console.error("err")
来源：http://rx.yuntaijiaju.cn

TS:   console.error("err")
来源：http://xe.huixinmuqiang.cn

Java: System.err.println("err")
来源：http://nt.lnxyls.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bi.bjjhwx.cn

Ruby: warn "err"
来源：http://gd.nszjky.cn

C#:   Console.Error.WriteLine("err")
来源：http://cj.gzmigu.cn

[M07] 判断是否为主入口
来源：http://mr.bjjhwx.cn

Py:   if __name__ == "__main__":
来源：http://sz.colortex.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cf.lnxyls.cn

JS:   require.main === module
来源：http://yp.colortex.cn

TS:   require.main === module
来源：http://zu.newstarts.cn

Java: public static void main(String[] args)
来源：http://ph.panjiajie.cn

Go:   func main()
来源：http://ex.wgjwhj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wl.yuexingan06.cn

C#:   static void Main(string[] args)
来源：http://ks.shxzskj.cn


<!-- 参考信息 -->