代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://la.asd995.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fa.hnjuh.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oq.szsharing.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cf.jianghongdianzi.cn

[J03] 字符串解析为日期
来源：http://pc.9csxet.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uw.shtwfgs.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dl.hnjuh.cn

JS:   new Date("2024-01-02")
来源：http://qo.szsharing.cn

TS:   new Date("2024-01-02")
来源：http://ym.9csxet.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ld.panjiajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qh.yuntaijiaju.cn

Ruby: Date.parse("2024-01-02")
来源：http://qc.9csxet.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yd.muxihuayi.cn

[J04] 时间戳与日期互转
来源：http://my.bookmarksfly.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://iy.bookmarksfly.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://oe.jctech888.com.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tq.szxytkj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dj.yuntaijiaju.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vn.bjjhwx.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xe.lnxyls.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vq.shtwfgs.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pm.shxzukj.cn

[J05] 时间加减（加 7 天）
来源：http://yg.9csxet.cn

Py:   now + timedelta(days=7)
来源：http://jg.szsharing.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://tq.bookmarksfly.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fj.hnjuh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://my.lnxyls.cn

Java: LocalDate.now().plusDays(7)
来源：http://bt.jctech888.com.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bf.nszjky.cn

Ruby: Time.now + 7 * 86400
来源：http://nj.jianghongdianzi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jx.szsharing.cn

[J06] 计算两时间之差
来源：http://jn.huixiangedu.cn

Py:   (end - start).total_seconds()
来源：http://ll.szsharing.cn

PHP:  $end->diff($start)->days;
来源：http://mx.bjjhwx.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jk.huanxung.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rl.hahajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lg.haigaiapp.cn

Go:   end.Sub(start).Hours()
来源：http://vm.bookmarksfly.cn

Ruby: end - start                 # 返回秒数
来源：http://de.521024.cn

C#:   (end - start).TotalSeconds
来源：http://ue.huixinmuqiang.cn

[J07] 比较两个日期
来源：http://up.shtwfgs.cn

Py:   d1 < d2;  d1 == d2
来源：http://mj.bjjhwx.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://df.jianghongdianzi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xl.9csxet.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vu.muxihuayi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xx.yuntaijiaju.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fd.nicolike.cn

Ruby: d1 < d2;  d1 == d2
来源：http://tg.colortex.cn

C#:   d1 < d2;  d1 == d2
来源：http://yj.jianghongdianzi.cn

[J08] 提取年月日与星期
来源：http://ut.yuexingan06.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fy.9csxet.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vc.gzmigu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jx.muxihuayi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qp.panjiajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kt.panjiajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lh.szsharing.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ke.asd995.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xt.huixinmuqiang.cn

[J09] 时区处理
来源：http://bw.yuntaijiaju.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ns.huanxung.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xo.hahajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tn.nszjky.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zs.lnxyls.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ma.chemitech.net.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ij.szsharing.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wb.szxytkj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lc.yuexingan06.cn

[J10] 取今天 / 本月第一天
来源：http://fu.nicolike.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://lr.shtwfgs.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fj.asd995.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://oo.colortex.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lf.bookmarksfly.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rp.panjiajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qr.haigaiapp.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wz.szsharing.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ep.yuntaijiaju.cn

================================================================================
来源：http://xh.szsharing.cn

K. JSON 与序列化
来源：http://ea.huanxung.cn

================================================================================
来源：http://gq.gzmigu.cn

[K01] 对象转 JSON 字符串
来源：http://nb.nszjky.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ob.chemitech.net.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tb.nszjky.cn

JS:   JSON.stringify(obj)
来源：http://ck.9csxet.cn

TS:   JSON.stringify(obj)
来源：http://dg.bookmarksfly.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://un.nicolike.cn

Go:   json.Marshal(obj)
来源：http://zm.shxzskj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://na.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://sg.9csxet.cn

[K02] JSON 字符串转对象
来源：http://fb.huixinmuqiang.cn

Py:   json.loads(s)
来源：http://ip.haigaiapp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yw.panjiajie.cn

JS:   JSON.parse(s)
来源：http://qn.asd995.cn

TS:   JSON.parse(s)
来源：http://ic.szxytkj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hd.huixinmuqiang.cn

Go:   json.Unmarshal(data, &v)
来源：http://mt.panjiajie.cn

Ruby: JSON.parse(s)
来源：http://jy.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ry.szxytkj.cn

[K03] JSON 美化输出（带缩进）
来源：http://dz.9csxet.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xd.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ez.jctech888.com.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nc.szsharing.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://uc.jianghongdianzi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wm.asd995.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://je.colortex.cn

Ruby: JSON.pretty_generate(obj)
来源：http://sb.huanxung.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ir.shxzskj.cn

[K04] 读取 JSON 文件
来源：http://dc.newstarts.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vx.nicolike.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xs.huanxung.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ue.shxzukj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dv.hahajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ce.szsharing.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dl.colortex.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ob.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gs.yuntaijiaju.cn

[K05] 深拷贝对象
来源：http://rs.yuexingan06.cn

Py:   copy.deepcopy(obj)
来源：http://bd.szxytkj.cn

PHP:  unserialize(serialize($obj));
来源：http://fk.colortex.cn

JS:   structuredClone(obj)
来源：http://xv.muxihuayi.cn

TS:   structuredClone(obj)
来源：http://fj.huixinmuqiang.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zo.nszjky.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kk.lnxyls.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tl.muxihuayi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://kg.9csxet.cn

[K06] 解析 URL 查询串
来源：http://rh.521024.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dx.haigaiapp.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ip.huixiangedu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lv.521024.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hj.shtwfgs.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sx.panjiajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rt.hahajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pk.jianghongdianzi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dc.nszjky.cn

[K07] 进制转换
来源：http://mf.jianghongdianzi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qk.lnxyls.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nz.hahajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mj.jianghongdianzi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sk.newstarts.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zw.bookmarksfly.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ho.nszjky.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://he.shxzskj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://me.szsharing.cn

[K08] 二进制序列化（非 JSON）
来源：http://dq.yuexingan06.cn

Py:   pickle.dumps(obj)
来源：http://xe.shxzskj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ua.yuntaijiaju.cn

JS:   v8.serialize(obj)        // Node
来源：http://xy.newstarts.cn

TS:   v8.serialize(obj)        // Node
来源：http://lp.jianghongdianzi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mq.jianghongdianzi.cn

Go:   encoding/gob
来源：http://pe.huixiangedu.cn

Ruby: Marshal.dump(obj)
来源：http://rl.nszjky.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mh.bookmarksfly.cn

================================================================================
来源：http://wz.newstarts.cn

L. 网络请求
来源：http://ln.shtwfgs.cn

================================================================================
来源：http://lu.hahajie.cn

[L01] 发送 GET 请求
来源：http://yv.yuntaijiaju.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://os.yuntaijiaju.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vv.shtwfgs.cn

JS:   await fetch(url)
来源：http://fl.shxzukj.cn

TS:   await fetch(url)
来源：http://wi.yuexingan06.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://al.hnjuh.cn

Go:   resp, err := http.Get(url)
来源：http://ra.wgjwhj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://az.bjjhwx.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cy.gzmigu.cn

[L02] 发送 POST JSON
来源：http://bl.nicolike.cn

Py:   requests.post(url, json={"a": 1})
来源：http://on.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://td.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vd.shtwfgs.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gf.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://os.yuexingan06.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wv.lnxyls.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lz.haigaiapp.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://er.shxzukj.cn

[L03] 设置自定义请求头
来源：http://cy.wgjwhj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ok.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fj.shtwfgs.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gk.jianghongdianzi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ix.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://it.shxzskj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fz.huixiangedu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://so.colortex.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://om.wgjwhj.cn

[L04] 设置超时
来源：http://kp.szxytkj.cn

Py:   requests.get(url, timeout=5)
来源：http://ui.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gn.haigaiapp.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vj.hnjuh.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ot.yuexingan06.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://an.yuntaijiaju.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wj.haigaiapp.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vw.asd995.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jw.hnjuh.cn

[L05] 上传文件（multipart）
来源：http://ou.shtwfgs.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tp.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sv.szsharing.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ij.hahajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hm.yuntaijiaju.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xu.shxzukj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yo.shxzukj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pb.bjjhwx.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tw.521024.cn

[L06] 解析响应为 JSON
来源：http://mk.huanxung.cn

Py:   resp.json()
来源：http://gf.colortex.cn

PHP:  json_decode($body, true);
来源：http://bk.bjjhwx.cn

JS:   await resp.json()
来源：http://eg.nicolike.cn

TS:   await resp.json()
来源：http://ni.hnjuh.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ti.yuexingan06.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hf.hnjuh.cn

Ruby: JSON.parse(resp.body)
来源：http://mn.bookmarksfly.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://av.szxytkj.cn

[L07] 处理 HTTP 状态码
来源：http://vg.huixinmuqiang.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uo.shtwfgs.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uw.gzmigu.cn

JS:   resp.ok;  resp.status
来源：http://pp.hahajie.cn

TS:   resp.ok;  resp.status
来源：http://lu.chemitech.net.cn

Java: resp.statusCode()
来源：http://pg.haigaiapp.cn

Go:   resp.StatusCode
来源：http://zq.yuntaijiaju.cn

Ruby: resp.code.to_i
来源：http://wc.colortex.cn

C#:   (int)resp.StatusCode
来源：http://re.9csxet.cn

[L08] 并发请求多个地址
来源：http://ps.huanxung.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wb.wgjwhj.cn

PHP:  curl_multi_init() 系列
来源：http://kk.szxytkj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ci.asd995.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fo.chemitech.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://md.shxzukj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kh.muxihuayi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qy.shxzukj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://st.gzmigu.cn

================================================================================
来源：http://ys.chemitech.net.cn

M. 命令行 / 进程 / 环境
来源：http://ar.yuexingan06.cn

================================================================================
来源：http://uy.wgjwhj.cn

[M01] 读取命令行参数
来源：http://ch.szxytkj.cn

Py:   sys.argv[1:]
来源：http://cl.chemitech.net.cn

PHP:  $argv;  $argc;
来源：http://nz.huixinmuqiang.cn

JS:   process.argv.slice(2)
来源：http://gt.521024.cn

TS:   process.argv.slice(2)
来源：http://gy.muxihuayi.cn

Java: args 数组（main 方法参数）
来源：http://zw.szxytkj.cn

Go:   os.Args[1:]
来源：http://pz.huixiangedu.cn

Ruby: ARGV
来源：http://vi.521024.cn

C#:   args 数组（Main 方法参数）
来源：http://uq.yuexingan06.cn

[M02] 读取环境变量
来源：http://yc.nszjky.cn

Py:   os.environ.get("HOME")
来源：http://xn.szsharing.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xq.muxihuayi.cn

JS:   process.env.HOME
来源：http://sr.szsharing.cn

TS:   process.env.HOME
来源：http://qo.shxzskj.cn

Java: System.getenv("HOME")
来源：http://sm.chemitech.net.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://el.asd995.cn

Ruby: ENV["HOME"]
来源：http://kb.huixinmuqiang.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ur.shtwfgs.cn

[M03] 执行外部命令
来源：http://nj.hnjuh.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jm.newstarts.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lk.jctech888.com.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gk.jianghongdianzi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://du.haigaiapp.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ux.yuexingan06.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zi.huanxung.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ws.huixinmuqiang.cn

C#:   Process.Start("ls", "-l");
来源：http://ui.hnjuh.cn

[M04] 获取当前工作目录
来源：http://ew.shxzskj.cn

Py:   os.getcwd()
来源：http://al.jianghongdianzi.cn

PHP:  getcwd();
来源：http://qw.chemitech.net.cn

JS:   process.cwd()
来源：http://ct.asd995.cn

TS:   process.cwd()
来源：http://rh.hnjuh.cn

Java: Path.of("").toAbsolutePath()
来源：http://bk.bjjhwx.cn

Go:   os.Getwd()
来源：http://vk.hahajie.cn

Ruby: Dir.pwd
来源：http://ah.newstarts.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ht.newstarts.cn

[M05] 设置退出码
来源：http://re.hahajie.cn

Py:   sys.exit(1)
来源：http://eo.yuntaijiaju.cn

PHP:  exit(1);
来源：http://az.muxihuayi.cn

JS:   process.exit(1)
来源：http://zb.panjiajie.cn

TS:   process.exit(1)
来源：http://ha.colortex.cn

Java: System.exit(1)
来源：http://zo.szsharing.cn

Go:   os.Exit(1)
来源：http://jt.haigaiapp.cn

Ruby: exit 1
来源：http://yg.colortex.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fd.hahajie.cn

[M06] 向标准错误输出
来源：http://ka.nicolike.cn

Py:   print("err", file=sys.stderr)
来源：http://me.bookmarksfly.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cy.shxzskj.cn

JS:   console.error("err")
来源：http://hs.colortex.cn

TS:   console.error("err")
来源：http://ku.bjjhwx.cn

Java: System.err.println("err")
来源：http://vg.shtwfgs.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qb.yuntaijiaju.cn

Ruby: warn "err"
来源：http://dl.colortex.cn

C#:   Console.Error.WriteLine("err")
来源：http://pb.haigaiapp.cn

[M07] 判断是否为主入口
来源：http://hb.jctech888.com.cn

Py:   if __name__ == "__main__":
来源：http://sh.521024.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bk.nicolike.cn

JS:   require.main === module
来源：http://ak.shtwfgs.cn

TS:   require.main === module
来源：http://dr.nicolike.cn

Java: public static void main(String[] args)
来源：http://am.colortex.cn

Go:   func main()
来源：http://lq.haigaiapp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ew.nicolike.cn

C#:   static void Main(string[] args)
来源：http://gb.9csxet.cn

[M08] 获取系统与运行时信息
来源：http://ri.wgjwhj.cn

Py:   platform.system();  platform.python_version()
来源：http://hk.panjiajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://qj.gzmigu.cn

JS:   process.platform;  process.version
来源：http://bd.huanxung.cn

TS:   process.platform;  process.version
来源：http://mp.asd995.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wj.gzmigu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yr.521024.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mb.hahajie.cn


<!-- 参考信息 -->