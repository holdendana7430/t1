代发 wailian999

[J03] 字符串解析为日期
来源：http://xc.lnxyls.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jn.jianghongdianzi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tr.jctech888.com.cn

JS:   new Date("2024-01-02")
来源：http://dr.panjiajie.cn

TS:   new Date("2024-01-02")
来源：http://bj.asd995.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ip.chemitech.net.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ia.shxzukj.cn

Ruby: Date.parse("2024-01-02")
来源：http://hb.nszjky.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dw.huixiangedu.cn

[J04] 时间戳与日期互转
来源：http://sl.yuexingan06.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gn.nicolike.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vc.bjjhwx.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://iv.shxzskj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tr.huanxung.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yp.yuntaijiaju.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qz.nszjky.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ki.wgjwhj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wx.lnxyls.cn

[J05] 时间加减（加 7 天）
来源：http://ag.panjiajie.cn

Py:   now + timedelta(days=7)
来源：http://ye.szxytkj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ht.newstarts.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tj.bookmarksfly.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ko.chemitech.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://rg.wgjwhj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sx.wgjwhj.cn

Ruby: Time.now + 7 * 86400
来源：http://ll.nszjky.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gr.muxihuayi.cn

[J06] 计算两时间之差
来源：http://ov.shxzskj.cn

Py:   (end - start).total_seconds()
来源：http://bv.wgjwhj.cn

PHP:  $end->diff($start)->days;
来源：http://va.jctech888.com.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://if.chemitech.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qr.gzmigu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ai.huixiangedu.cn

Go:   end.Sub(start).Hours()
来源：http://kc.szsharing.cn

Ruby: end - start                 # 返回秒数
来源：http://jx.hahajie.cn

C#:   (end - start).TotalSeconds
来源：http://ln.shtwfgs.cn

[J07] 比较两个日期
来源：http://uz.shxzukj.cn

Py:   d1 < d2;  d1 == d2
来源：http://yd.lnxyls.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pe.colortex.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vm.szsharing.cn

TS:   d1.getTime() < d2.getTime()
来源：http://kk.huixinmuqiang.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zs.szsharing.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xp.colortex.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lm.lnxyls.cn

C#:   d1 < d2;  d1 == d2
来源：http://mf.9csxet.cn

[J08] 提取年月日与星期
来源：http://fd.nszjky.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jg.szxytkj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ip.hahajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://op.wgjwhj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fp.szxytkj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://io.lnxyls.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zt.gzmigu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ie.nicolike.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vk.jianghongdianzi.cn

[J09] 时区处理
来源：http://sy.bjjhwx.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wu.hahajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gx.chemitech.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wk.lnxyls.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xk.haigaiapp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bm.nszjky.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hn.9csxet.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lm.szxytkj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ia.shxzukj.cn

[J10] 取今天 / 本月第一天
来源：http://vj.bookmarksfly.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ua.9csxet.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ly.bjjhwx.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dh.muxihuayi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mi.nszjky.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://th.asd995.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gh.wgjwhj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pa.521024.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sd.szxytkj.cn

================================================================================
来源：http://ir.huanxung.cn

K. JSON 与序列化
来源：http://la.bjjhwx.cn

================================================================================
来源：http://nb.yuntaijiaju.cn

[K01] 对象转 JSON 字符串
来源：http://pt.wgjwhj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vz.shtwfgs.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bf.yuexingan06.cn

JS:   JSON.stringify(obj)
来源：http://lu.gzmigu.cn

TS:   JSON.stringify(obj)
来源：http://ai.wgjwhj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ux.szsharing.cn

Go:   json.Marshal(obj)
来源：http://us.shtwfgs.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ab.hnjuh.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ki.jianghongdianzi.cn

[K02] JSON 字符串转对象
来源：http://ia.huixiangedu.cn

Py:   json.loads(s)
来源：http://wn.shtwfgs.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ey.521024.cn

JS:   JSON.parse(s)
来源：http://sq.szxytkj.cn

TS:   JSON.parse(s)
来源：http://aq.bjjhwx.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fv.shxzukj.cn

Go:   json.Unmarshal(data, &v)
来源：http://cc.huanxung.cn

Ruby: JSON.parse(s)
来源：http://fn.521024.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kg.hnjuh.cn

[K03] JSON 美化输出（带缩进）
来源：http://iv.hnjuh.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://un.bjjhwx.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bg.9csxet.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://we.jctech888.com.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://he.haigaiapp.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xk.521024.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qh.asd995.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rz.hahajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kc.huixiangedu.cn

[K04] 读取 JSON 文件
来源：http://nl.haigaiapp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rc.panjiajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vx.nszjky.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ou.9csxet.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aq.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://je.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xs.huanxung.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mo.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pj.shtwfgs.cn

[K05] 深拷贝对象
来源：http://sv.hnjuh.cn

Py:   copy.deepcopy(obj)
来源：http://wg.yuexingan06.cn

PHP:  unserialize(serialize($obj));
来源：http://ae.szsharing.cn

JS:   structuredClone(obj)
来源：http://yh.yuexingan06.cn

TS:   structuredClone(obj)
来源：http://ps.nszjky.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fc.huixiangedu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tl.shxzskj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ms.hahajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dr.bjjhwx.cn

[K06] 解析 URL 查询串
来源：http://pg.gzmigu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sv.chemitech.net.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ff.panjiajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cy.szsharing.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mp.panjiajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vt.asd995.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ut.nszjky.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ii.muxihuayi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jt.bjjhwx.cn

[K07] 进制转换
来源：http://kq.shtwfgs.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ic.bookmarksfly.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://us.yuntaijiaju.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xs.muxihuayi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fx.huixinmuqiang.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rh.huixinmuqiang.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ln.nicolike.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qr.jianghongdianzi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uc.panjiajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://ny.chemitech.net.cn

Py:   pickle.dumps(obj)
来源：http://ji.hahajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://op.nicolike.cn

JS:   v8.serialize(obj)        // Node
来源：http://pe.hahajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://tu.huixinmuqiang.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wy.nszjky.cn

Go:   encoding/gob
来源：http://hr.huixiangedu.cn

Ruby: Marshal.dump(obj)
来源：http://jq.szxytkj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://em.jctech888.com.cn

================================================================================
来源：http://xj.shxzukj.cn

L. 网络请求
来源：http://mo.9csxet.cn

================================================================================
来源：http://ki.gzmigu.cn

[L01] 发送 GET 请求
来源：http://ic.haigaiapp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pn.hnjuh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dp.huanxung.cn

JS:   await fetch(url)
来源：http://qd.jianghongdianzi.cn

TS:   await fetch(url)
来源：http://zj.wgjwhj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mj.nszjky.cn

Go:   resp, err := http.Get(url)
来源：http://gh.newstarts.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://no.hnjuh.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://du.hahajie.cn

[L02] 发送 POST JSON
来源：http://zd.jianghongdianzi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ot.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ja.jctech888.com.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zn.shxzskj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yi.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sm.wgjwhj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qb.bookmarksfly.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gw.yuntaijiaju.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gm.hnjuh.cn

[L03] 设置自定义请求头
来源：http://xf.asd995.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wb.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mf.shtwfgs.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ze.hnjuh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fx.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://za.colortex.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wk.shxzskj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tm.yuntaijiaju.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ee.shxzskj.cn

[L04] 设置超时
来源：http://yh.panjiajie.cn

Py:   requests.get(url, timeout=5)
来源：http://xu.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fs.jctech888.com.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rh.bjjhwx.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vr.shxzukj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zz.panjiajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ei.colortex.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xw.9csxet.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nm.521024.cn

[L05] 上传文件（multipart）
来源：http://ug.huixiangedu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wg.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ah.colortex.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yi.jianghongdianzi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rp.jctech888.com.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zt.bookmarksfly.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jt.jctech888.com.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wn.bjjhwx.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lx.haigaiapp.cn

[L06] 解析响应为 JSON
来源：http://ix.gzmigu.cn

Py:   resp.json()
来源：http://wc.asd995.cn

PHP:  json_decode($body, true);
来源：http://vf.nszjky.cn

JS:   await resp.json()
来源：http://mu.asd995.cn

TS:   await resp.json()
来源：http://nu.yuntaijiaju.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cr.haigaiapp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nq.muxihuayi.cn

Ruby: JSON.parse(resp.body)
来源：http://zp.gzmigu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lt.huixinmuqiang.cn

[L07] 处理 HTTP 状态码
来源：http://dq.newstarts.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pt.9csxet.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wu.newstarts.cn

JS:   resp.ok;  resp.status
来源：http://tk.szxytkj.cn

TS:   resp.ok;  resp.status
来源：http://fe.gzmigu.cn

Java: resp.statusCode()
来源：http://oz.chemitech.net.cn

Go:   resp.StatusCode
来源：http://be.huanxung.cn

Ruby: resp.code.to_i
来源：http://ci.jianghongdianzi.cn

C#:   (int)resp.StatusCode
来源：http://ht.shxzskj.cn

[L08] 并发请求多个地址
来源：http://iw.521024.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gb.panjiajie.cn

PHP:  curl_multi_init() 系列
来源：http://lf.lnxyls.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zo.huixinmuqiang.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gy.huanxung.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gk.yuexingan06.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ku.huixinmuqiang.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fo.bjjhwx.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rc.jianghongdianzi.cn

================================================================================
来源：http://zh.shxzukj.cn

M. 命令行 / 进程 / 环境
来源：http://an.shxzukj.cn

================================================================================
来源：http://an.gzmigu.cn

[M01] 读取命令行参数
来源：http://uf.colortex.cn

Py:   sys.argv[1:]
来源：http://bn.jctech888.com.cn

PHP:  $argv;  $argc;
来源：http://cw.huixinmuqiang.cn

JS:   process.argv.slice(2)
来源：http://nf.newstarts.cn

TS:   process.argv.slice(2)
来源：http://dl.haigaiapp.cn

Java: args 数组（main 方法参数）
来源：http://fz.9csxet.cn

Go:   os.Args[1:]
来源：http://qx.szxytkj.cn

Ruby: ARGV
来源：http://kh.hahajie.cn

C#:   args 数组（Main 方法参数）
来源：http://js.asd995.cn

[M02] 读取环境变量
来源：http://rn.szsharing.cn

Py:   os.environ.get("HOME")
来源：http://rs.shtwfgs.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://te.szxytkj.cn

JS:   process.env.HOME
来源：http://wr.jianghongdianzi.cn

TS:   process.env.HOME
来源：http://il.muxihuayi.cn

Java: System.getenv("HOME")
来源：http://mq.szxytkj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hb.muxihuayi.cn

Ruby: ENV["HOME"]
来源：http://ls.jctech888.com.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dd.szsharing.cn

[M03] 执行外部命令
来源：http://ha.muxihuayi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ao.gzmigu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://br.jianghongdianzi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vo.szxytkj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://aj.hahajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ox.hnjuh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wx.shxzskj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://za.gzmigu.cn

C#:   Process.Start("ls", "-l");
来源：http://ag.colortex.cn

[M04] 获取当前工作目录
来源：http://ye.shxzukj.cn

Py:   os.getcwd()
来源：http://qs.jctech888.com.cn

PHP:  getcwd();
来源：http://dn.panjiajie.cn

JS:   process.cwd()
来源：http://xo.szsharing.cn

TS:   process.cwd()
来源：http://gg.shxzukj.cn

Java: Path.of("").toAbsolutePath()
来源：http://cg.szxytkj.cn

Go:   os.Getwd()
来源：http://ln.wgjwhj.cn

Ruby: Dir.pwd
来源：http://rh.lnxyls.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jc.bookmarksfly.cn

[M05] 设置退出码
来源：http://vn.bjjhwx.cn

Py:   sys.exit(1)
来源：http://lz.asd995.cn

PHP:  exit(1);
来源：http://dy.bookmarksfly.cn

JS:   process.exit(1)
来源：http://ja.521024.cn

TS:   process.exit(1)
来源：http://wl.wgjwhj.cn

Java: System.exit(1)
来源：http://de.wgjwhj.cn

Go:   os.Exit(1)
来源：http://qg.hnjuh.cn

Ruby: exit 1
来源：http://fo.haigaiapp.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nj.jctech888.com.cn

[M06] 向标准错误输出
来源：http://jk.nicolike.cn

Py:   print("err", file=sys.stderr)
来源：http://bp.nicolike.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://em.szsharing.cn

JS:   console.error("err")
来源：http://oc.huixinmuqiang.cn

TS:   console.error("err")
来源：http://si.yuntaijiaju.cn

Java: System.err.println("err")
来源：http://zk.chemitech.net.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mg.wgjwhj.cn

Ruby: warn "err"
来源：http://yg.colortex.cn

C#:   Console.Error.WriteLine("err")
来源：http://gg.9csxet.cn

[M07] 判断是否为主入口
来源：http://yf.newstarts.cn

Py:   if __name__ == "__main__":
来源：http://hs.newstarts.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nf.muxihuayi.cn

JS:   require.main === module
来源：http://hn.yuntaijiaju.cn

TS:   require.main === module
来源：http://zy.gzmigu.cn

Java: public static void main(String[] args)
来源：http://yy.nszjky.cn

Go:   func main()
来源：http://if.bookmarksfly.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cg.shxzskj.cn

C#:   static void Main(string[] args)
来源：http://bz.nicolike.cn

[M08] 获取系统与运行时信息
来源：http://st.yuexingan06.cn

Py:   platform.system();  platform.python_version()
来源：http://qu.jctech888.com.cn

PHP:  PHP_OS;  phpversion();
来源：http://sf.9csxet.cn

JS:   process.platform;  process.version
来源：http://xu.hnjuh.cn

TS:   process.platform;  process.version
来源：http://li.gzmigu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://un.asd995.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://pn.huixiangedu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lg.jianghongdianzi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ie.yuexingan06.cn

================================================================================
来源：http://cj.nszjky.cn

N. 数据结构与算法
来源：http://yk.huixiangedu.cn

================================================================================
来源：http://ry.lnxyls.cn


<!-- 参考信息 -->