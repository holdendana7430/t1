代发 wailian999

[J03] 字符串解析为日期
来源：http://gh.nicolike.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ev.nicolike.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://iq.bjjhwx.cn

JS:   new Date("2024-01-02")
来源：http://fc.huanxung.cn

TS:   new Date("2024-01-02")
来源：http://au.bjjhwx.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ab.gzmigu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hj.chemitech.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://ll.yuntaijiaju.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://km.gzmigu.cn

[J04] 时间戳与日期互转
来源：http://fn.hnjuh.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gm.jianghongdianzi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://al.asd995.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ws.chemitech.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zs.huanxung.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qa.521024.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ma.nicolike.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cf.colortex.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yp.yuntaijiaju.cn

[J05] 时间加减（加 7 天）
来源：http://mr.nicolike.cn

Py:   now + timedelta(days=7)
来源：http://wv.nszjky.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ha.jianghongdianzi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ct.hnjuh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gi.lnxyls.cn

Java: LocalDate.now().plusDays(7)
来源：http://vy.szxytkj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gp.hnjuh.cn

Ruby: Time.now + 7 * 86400
来源：http://qw.shxzukj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gw.colortex.cn

[J06] 计算两时间之差
来源：http://an.nszjky.cn

Py:   (end - start).total_seconds()
来源：http://vs.hahajie.cn

PHP:  $end->diff($start)->days;
来源：http://qn.shxzukj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qj.bookmarksfly.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cf.newstarts.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ut.jianghongdianzi.cn

Go:   end.Sub(start).Hours()
来源：http://xa.bjjhwx.cn

Ruby: end - start                 # 返回秒数
来源：http://hc.nicolike.cn

C#:   (end - start).TotalSeconds
来源：http://lt.huanxung.cn

[J07] 比较两个日期
来源：http://cz.yuntaijiaju.cn

Py:   d1 < d2;  d1 == d2
来源：http://xg.shtwfgs.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qf.521024.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ao.szxytkj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yi.muxihuayi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ga.newstarts.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wo.huixinmuqiang.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wt.jctech888.com.cn

C#:   d1 < d2;  d1 == d2
来源：http://eb.bjjhwx.cn

[J08] 提取年月日与星期
来源：http://og.9csxet.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zh.wgjwhj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tc.nszjky.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fr.huanxung.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pv.colortex.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ke.9csxet.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bf.shxzukj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://re.newstarts.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mj.szsharing.cn

[J09] 时区处理
来源：http://uc.hahajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xq.szsharing.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wk.shtwfgs.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xh.muxihuayi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zn.szxytkj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ks.hahajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bo.gzmigu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://or.shxzukj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://os.huixinmuqiang.cn

[J10] 取今天 / 本月第一天
来源：http://fu.panjiajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ft.yuntaijiaju.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ds.huixinmuqiang.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fn.shxzskj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dn.szxytkj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wx.haigaiapp.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jp.shxzukj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ch.huanxung.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jr.9csxet.cn

================================================================================
来源：http://mq.colortex.cn

K. JSON 与序列化
来源：http://cl.newstarts.cn

================================================================================
来源：http://rf.hnjuh.cn

[K01] 对象转 JSON 字符串
来源：http://ak.panjiajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sk.bookmarksfly.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ve.colortex.cn

JS:   JSON.stringify(obj)
来源：http://wf.9csxet.cn

TS:   JSON.stringify(obj)
来源：http://me.gzmigu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://eg.huanxung.cn

Go:   json.Marshal(obj)
来源：http://zd.gzmigu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://us.szxytkj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ce.yuexingan06.cn

[K02] JSON 字符串转对象
来源：http://ip.shtwfgs.cn

Py:   json.loads(s)
来源：http://qm.asd995.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ut.wgjwhj.cn

JS:   JSON.parse(s)
来源：http://rq.huixinmuqiang.cn

TS:   JSON.parse(s)
来源：http://db.yuntaijiaju.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rs.muxihuayi.cn

Go:   json.Unmarshal(data, &v)
来源：http://pp.jianghongdianzi.cn

Ruby: JSON.parse(s)
来源：http://np.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ee.hnjuh.cn

[K03] JSON 美化输出（带缩进）
来源：http://qr.gzmigu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qw.521024.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ib.yuntaijiaju.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gm.yuntaijiaju.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://uq.shxzskj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dt.szxytkj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ag.jianghongdianzi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nz.shxzskj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nt.gzmigu.cn

[K04] 读取 JSON 文件
来源：http://gb.newstarts.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vf.bjjhwx.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://eu.yuntaijiaju.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://px.lnxyls.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mb.hnjuh.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fv.szxytkj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dt.hahajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hv.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ot.haigaiapp.cn

[K05] 深拷贝对象
来源：http://ht.jctech888.com.cn

Py:   copy.deepcopy(obj)
来源：http://ez.shtwfgs.cn

PHP:  unserialize(serialize($obj));
来源：http://lg.yuntaijiaju.cn

JS:   structuredClone(obj)
来源：http://xt.yuexingan06.cn

TS:   structuredClone(obj)
来源：http://wv.huixinmuqiang.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vd.gzmigu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yi.nicolike.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ha.szxytkj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lx.gzmigu.cn

[K06] 解析 URL 查询串
来源：http://eo.yuexingan06.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vj.nicolike.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wn.bjjhwx.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ud.haigaiapp.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cy.huixiangedu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yw.9csxet.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ox.huixiangedu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://px.hahajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yy.nszjky.cn

[K07] 进制转换
来源：http://hj.shxzskj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bg.gzmigu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wn.hnjuh.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hb.gzmigu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ym.jianghongdianzi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sf.bjjhwx.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xo.9csxet.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uh.chemitech.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wp.szxytkj.cn

[K08] 二进制序列化（非 JSON）
来源：http://rw.chemitech.net.cn

Py:   pickle.dumps(obj)
来源：http://lm.9csxet.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dr.bookmarksfly.cn

JS:   v8.serialize(obj)        // Node
来源：http://mh.wgjwhj.cn

TS:   v8.serialize(obj)        // Node
来源：http://zb.hnjuh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yy.yuntaijiaju.cn

Go:   encoding/gob
来源：http://zn.newstarts.cn

Ruby: Marshal.dump(obj)
来源：http://lc.nicolike.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ay.newstarts.cn

================================================================================
来源：http://sx.nszjky.cn

L. 网络请求
来源：http://pu.shxzskj.cn

================================================================================
来源：http://jk.bjjhwx.cn

[L01] 发送 GET 请求
来源：http://di.szsharing.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://if.bjjhwx.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ln.gzmigu.cn

JS:   await fetch(url)
来源：http://nl.yuntaijiaju.cn

TS:   await fetch(url)
来源：http://hi.wgjwhj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zr.szxytkj.cn

Go:   resp, err := http.Get(url)
来源：http://oe.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ak.9csxet.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qi.jctech888.com.cn

[L02] 发送 POST JSON
来源：http://zm.shxzukj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://po.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pq.shxzskj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nl.shxzskj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sk.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xq.lnxyls.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hr.bjjhwx.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ag.huanxung.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uk.chemitech.net.cn

[L03] 设置自定义请求头
来源：http://pp.szxytkj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ns.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ju.shxzskj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zm.colortex.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fo.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://is.huanxung.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yz.haigaiapp.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bs.521024.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kf.shtwfgs.cn

[L04] 设置超时
来源：http://ux.lnxyls.cn

Py:   requests.get(url, timeout=5)
来源：http://yv.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://si.huanxung.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jy.szsharing.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://re.chemitech.net.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ki.muxihuayi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zf.newstarts.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gm.huanxung.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jx.colortex.cn

[L05] 上传文件（multipart）
来源：http://iy.nicolike.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zr.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://im.shxzukj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ax.muxihuayi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://te.asd995.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bv.nszjky.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://un.haigaiapp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ri.bjjhwx.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xn.haigaiapp.cn

[L06] 解析响应为 JSON
来源：http://xr.haigaiapp.cn

Py:   resp.json()
来源：http://ih.huixiangedu.cn

PHP:  json_decode($body, true);
来源：http://lo.shxzukj.cn

JS:   await resp.json()
来源：http://as.nszjky.cn

TS:   await resp.json()
来源：http://bm.szxytkj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gm.jianghongdianzi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://eh.wgjwhj.cn

Ruby: JSON.parse(resp.body)
来源：http://jv.asd995.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kh.gzmigu.cn

[L07] 处理 HTTP 状态码
来源：http://iz.yuntaijiaju.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hj.asd995.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vq.yuexingan06.cn

JS:   resp.ok;  resp.status
来源：http://pi.521024.cn

TS:   resp.ok;  resp.status
来源：http://ld.lnxyls.cn

Java: resp.statusCode()
来源：http://sw.wgjwhj.cn

Go:   resp.StatusCode
来源：http://gg.panjiajie.cn

Ruby: resp.code.to_i
来源：http://as.bookmarksfly.cn

C#:   (int)resp.StatusCode
来源：http://hi.gzmigu.cn

[L08] 并发请求多个地址
来源：http://ti.521024.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://li.newstarts.cn

PHP:  curl_multi_init() 系列
来源：http://ru.shxzskj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hn.shxzukj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://on.szsharing.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jy.haigaiapp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://af.huanxung.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uf.haigaiapp.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://la.haigaiapp.cn

================================================================================
来源：http://ix.huixinmuqiang.cn

M. 命令行 / 进程 / 环境
来源：http://mu.shtwfgs.cn

================================================================================
来源：http://lh.hnjuh.cn

[M01] 读取命令行参数
来源：http://bk.colortex.cn

Py:   sys.argv[1:]
来源：http://af.gzmigu.cn

PHP:  $argv;  $argc;
来源：http://jl.huixiangedu.cn

JS:   process.argv.slice(2)
来源：http://ar.hahajie.cn

TS:   process.argv.slice(2)
来源：http://ed.haigaiapp.cn

Java: args 数组（main 方法参数）
来源：http://kn.panjiajie.cn

Go:   os.Args[1:]
来源：http://za.colortex.cn

Ruby: ARGV
来源：http://sd.shxzukj.cn

C#:   args 数组（Main 方法参数）
来源：http://qw.gzmigu.cn

[M02] 读取环境变量
来源：http://ze.haigaiapp.cn

Py:   os.environ.get("HOME")
来源：http://is.wgjwhj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://on.bookmarksfly.cn

JS:   process.env.HOME
来源：http://yq.shtwfgs.cn

TS:   process.env.HOME
来源：http://md.chemitech.net.cn

Java: System.getenv("HOME")
来源：http://mj.huixiangedu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://li.nicolike.cn

Ruby: ENV["HOME"]
来源：http://uf.panjiajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fj.shxzukj.cn

[M03] 执行外部命令
来源：http://ds.yuexingan06.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lv.colortex.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://oo.jctech888.com.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zz.jctech888.com.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xc.hnjuh.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fy.gzmigu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://id.yuexingan06.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kd.hahajie.cn

C#:   Process.Start("ls", "-l");
来源：http://ky.shxzskj.cn

[M04] 获取当前工作目录
来源：http://wm.yuntaijiaju.cn

Py:   os.getcwd()
来源：http://zl.panjiajie.cn

PHP:  getcwd();
来源：http://yl.gzmigu.cn

JS:   process.cwd()
来源：http://ch.huanxung.cn

TS:   process.cwd()
来源：http://jv.hnjuh.cn

Java: Path.of("").toAbsolutePath()
来源：http://gr.bjjhwx.cn

Go:   os.Getwd()
来源：http://cw.hahajie.cn

Ruby: Dir.pwd
来源：http://sc.nicolike.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sz.521024.cn

[M05] 设置退出码
来源：http://fi.colortex.cn

Py:   sys.exit(1)
来源：http://ed.hnjuh.cn

PHP:  exit(1);
来源：http://bl.huanxung.cn

JS:   process.exit(1)
来源：http://uy.gzmigu.cn

TS:   process.exit(1)
来源：http://bm.shxzukj.cn

Java: System.exit(1)
来源：http://mz.gzmigu.cn

Go:   os.Exit(1)
来源：http://iq.hahajie.cn

Ruby: exit 1
来源：http://yi.huixinmuqiang.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ib.521024.cn

[M06] 向标准错误输出
来源：http://bq.hahajie.cn

Py:   print("err", file=sys.stderr)
来源：http://ta.yuntaijiaju.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xm.bjjhwx.cn

JS:   console.error("err")
来源：http://jj.yuexingan06.cn

TS:   console.error("err")
来源：http://eo.bookmarksfly.cn

Java: System.err.println("err")
来源：http://pr.jianghongdianzi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mi.szxytkj.cn

Ruby: warn "err"
来源：http://hv.9csxet.cn

C#:   Console.Error.WriteLine("err")
来源：http://qu.nszjky.cn

[M07] 判断是否为主入口
来源：http://la.521024.cn

Py:   if __name__ == "__main__":
来源：http://pw.muxihuayi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://iu.muxihuayi.cn

JS:   require.main === module
来源：http://em.huixiangedu.cn

TS:   require.main === module
来源：http://co.521024.cn

Java: public static void main(String[] args)
来源：http://hg.huixinmuqiang.cn

Go:   func main()
来源：http://lp.nszjky.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ai.asd995.cn

C#:   static void Main(string[] args)
来源：http://do.asd995.cn

[M08] 获取系统与运行时信息
来源：http://qv.bjjhwx.cn

Py:   platform.system();  platform.python_version()
来源：http://cm.nicolike.cn

PHP:  PHP_OS;  phpversion();
来源：http://mt.shtwfgs.cn

JS:   process.platform;  process.version
来源：http://xn.szsharing.cn

TS:   process.platform;  process.version
来源：http://tq.shxzskj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tr.shxzskj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://px.chemitech.net.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hk.nszjky.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zu.panjiajie.cn

================================================================================
来源：http://mg.panjiajie.cn

N. 数据结构与算法
来源：http://qe.muxihuayi.cn

================================================================================
来源：http://wb.521024.cn


<!-- 参考信息 -->