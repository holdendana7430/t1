代发 wailian999

[J03] 字符串解析为日期
来源：http://ym.wgjwhj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sq.asd995.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://re.colortex.cn

JS:   new Date("2024-01-02")
来源：http://ak.shxzskj.cn

TS:   new Date("2024-01-02")
来源：http://jw.panjiajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hd.gzmigu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pg.bookmarksfly.cn

Ruby: Date.parse("2024-01-02")
来源：http://ew.szsharing.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dn.bookmarksfly.cn

[J04] 时间戳与日期互转
来源：http://xs.panjiajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lc.hnjuh.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gr.hahajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rj.9csxet.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qf.haigaiapp.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ct.hahajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ek.bjjhwx.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dx.szsharing.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lj.nicolike.cn

[J05] 时间加减（加 7 天）
来源：http://jp.hnjuh.cn

Py:   now + timedelta(days=7)
来源：http://nf.panjiajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://hs.szsharing.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hc.yuntaijiaju.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sf.huixiangedu.cn

Java: LocalDate.now().plusDays(7)
来源：http://pi.nszjky.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hd.shxzskj.cn

Ruby: Time.now + 7 * 86400
来源：http://bs.yuexingan06.cn

C#:   DateTime.Now.AddDays(7)
来源：http://nf.shtwfgs.cn

[J06] 计算两时间之差
来源：http://xs.szxytkj.cn

Py:   (end - start).total_seconds()
来源：http://rb.bookmarksfly.cn

PHP:  $end->diff($start)->days;
来源：http://iq.gzmigu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lv.shxzukj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://io.hnjuh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qj.yuntaijiaju.cn

Go:   end.Sub(start).Hours()
来源：http://gq.hnjuh.cn

Ruby: end - start                 # 返回秒数
来源：http://ls.huanxung.cn

C#:   (end - start).TotalSeconds
来源：http://fw.newstarts.cn

[J07] 比较两个日期
来源：http://xh.gzmigu.cn

Py:   d1 < d2;  d1 == d2
来源：http://pn.bookmarksfly.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qh.muxihuayi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ls.yuexingan06.cn

TS:   d1.getTime() < d2.getTime()
来源：http://sa.newstarts.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vm.yuntaijiaju.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jm.colortex.cn

Ruby: d1 < d2;  d1 == d2
来源：http://nh.shtwfgs.cn

C#:   d1 < d2;  d1 == d2
来源：http://fb.szxytkj.cn

[J08] 提取年月日与星期
来源：http://uj.nicolike.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tx.huixinmuqiang.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ez.bookmarksfly.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ar.huanxung.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wy.nicolike.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://in.gzmigu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yi.szsharing.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zo.yuntaijiaju.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ak.asd995.cn

[J09] 时区处理
来源：http://gc.shxzukj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pw.chemitech.net.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sb.shxzskj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ql.chemitech.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eo.hahajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://be.wgjwhj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gb.nszjky.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zl.newstarts.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fj.panjiajie.cn

[J10] 取今天 / 本月第一天
来源：http://ph.huixiangedu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ek.hahajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cp.nszjky.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ty.521024.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qi.shtwfgs.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gi.haigaiapp.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cf.jctech888.com.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://oy.muxihuayi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jx.szsharing.cn

================================================================================
来源：http://oe.nszjky.cn

K. JSON 与序列化
来源：http://rk.huixiangedu.cn

================================================================================
来源：http://bt.nszjky.cn

[K01] 对象转 JSON 字符串
来源：http://pz.yuntaijiaju.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hv.shxzukj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lu.9csxet.cn

JS:   JSON.stringify(obj)
来源：http://oh.shtwfgs.cn

TS:   JSON.stringify(obj)
来源：http://gv.nszjky.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xh.hnjuh.cn

Go:   json.Marshal(obj)
来源：http://qh.huixinmuqiang.cn

Ruby: obj.to_json                                     // require "json"
来源：http://do.colortex.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fi.nszjky.cn

[K02] JSON 字符串转对象
来源：http://cu.shxzskj.cn

Py:   json.loads(s)
来源：http://vj.szsharing.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lz.bookmarksfly.cn

JS:   JSON.parse(s)
来源：http://ln.panjiajie.cn

TS:   JSON.parse(s)
来源：http://lu.hahajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nq.huixiangedu.cn

Go:   json.Unmarshal(data, &v)
来源：http://vv.asd995.cn

Ruby: JSON.parse(s)
来源：http://yn.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rp.chemitech.net.cn

[K03] JSON 美化输出（带缩进）
来源：http://dh.gzmigu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ms.gzmigu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ke.wgjwhj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://at.jctech888.com.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wn.szxytkj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://om.bookmarksfly.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hi.shtwfgs.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pk.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kw.szsharing.cn

[K04] 读取 JSON 文件
来源：http://lj.shxzskj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ck.hahajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zt.szxytkj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ea.521024.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ap.szsharing.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://va.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lk.huixinmuqiang.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://tm.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qs.jianghongdianzi.cn

[K05] 深拷贝对象
来源：http://ge.newstarts.cn

Py:   copy.deepcopy(obj)
来源：http://nm.bjjhwx.cn

PHP:  unserialize(serialize($obj));
来源：http://pu.hahajie.cn

JS:   structuredClone(obj)
来源：http://xw.bjjhwx.cn

TS:   structuredClone(obj)
来源：http://ri.hnjuh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ir.hahajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gz.szsharing.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qu.shtwfgs.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ho.muxihuayi.cn

[K06] 解析 URL 查询串
来源：http://id.9csxet.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zb.jctech888.com.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cp.muxihuayi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ce.muxihuayi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tv.shtwfgs.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cp.gzmigu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hr.muxihuayi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yg.wgjwhj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wz.huanxung.cn

[K07] 进制转换
来源：http://gy.nicolike.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ji.jianghongdianzi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qx.bookmarksfly.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ue.9csxet.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qo.hahajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nv.9csxet.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zv.jianghongdianzi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bh.szsharing.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ln.shtwfgs.cn

[K08] 二进制序列化（非 JSON）
来源：http://dk.huanxung.cn

Py:   pickle.dumps(obj)
来源：http://yn.yuexingan06.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bl.panjiajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://hj.asd995.cn

TS:   v8.serialize(obj)        // Node
来源：http://ti.haigaiapp.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wd.jctech888.com.cn

Go:   encoding/gob
来源：http://ug.panjiajie.cn

Ruby: Marshal.dump(obj)
来源：http://xd.hahajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ct.asd995.cn

================================================================================
来源：http://xh.asd995.cn

L. 网络请求
来源：http://wu.nszjky.cn

================================================================================
来源：http://cs.huanxung.cn

[L01] 发送 GET 请求
来源：http://bx.shtwfgs.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xg.szsharing.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wv.lnxyls.cn

JS:   await fetch(url)
来源：http://mx.szxytkj.cn

TS:   await fetch(url)
来源：http://nc.chemitech.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yt.bjjhwx.cn

Go:   resp, err := http.Get(url)
来源：http://wh.shxzskj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ul.wgjwhj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rs.shxzskj.cn

[L02] 发送 POST JSON
来源：http://dj.lnxyls.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gj.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lu.colortex.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tt.shxzskj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fm.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xq.wgjwhj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lb.shxzukj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gi.yuexingan06.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://eb.jctech888.com.cn

[L03] 设置自定义请求头
来源：http://kn.colortex.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rm.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://iv.wgjwhj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://se.gzmigu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tk.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pq.panjiajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xd.yuntaijiaju.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jh.szsharing.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qf.shtwfgs.cn

[L04] 设置超时
来源：http://sj.szsharing.cn

Py:   requests.get(url, timeout=5)
来源：http://ws.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lv.shxzukj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iq.wgjwhj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ve.newstarts.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sj.panjiajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xw.jianghongdianzi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ch.shxzukj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lx.yuntaijiaju.cn

[L05] 上传文件（multipart）
来源：http://ed.newstarts.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tw.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vy.bjjhwx.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ae.panjiajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dt.huanxung.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cx.jctech888.com.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gz.huixinmuqiang.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pd.gzmigu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tx.haigaiapp.cn

[L06] 解析响应为 JSON
来源：http://ko.shtwfgs.cn

Py:   resp.json()
来源：http://ic.521024.cn

PHP:  json_decode($body, true);
来源：http://sh.colortex.cn

JS:   await resp.json()
来源：http://kq.9csxet.cn

TS:   await resp.json()
来源：http://fh.jianghongdianzi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lm.newstarts.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mn.jianghongdianzi.cn

Ruby: JSON.parse(resp.body)
来源：http://xf.huixiangedu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tp.muxihuayi.cn

[L07] 处理 HTTP 状态码
来源：http://tm.huixiangedu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wf.chemitech.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cs.nszjky.cn

JS:   resp.ok;  resp.status
来源：http://tq.bookmarksfly.cn

TS:   resp.ok;  resp.status
来源：http://iv.shtwfgs.cn

Java: resp.statusCode()
来源：http://bs.shxzukj.cn

Go:   resp.StatusCode
来源：http://xx.bjjhwx.cn

Ruby: resp.code.to_i
来源：http://bu.521024.cn

C#:   (int)resp.StatusCode
来源：http://ub.yuexingan06.cn

[L08] 并发请求多个地址
来源：http://ig.9csxet.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qu.szsharing.cn

PHP:  curl_multi_init() 系列
来源：http://qj.jctech888.com.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nl.colortex.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hl.521024.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pb.bookmarksfly.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ih.newstarts.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ac.colortex.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mi.lnxyls.cn

================================================================================
来源：http://tj.muxihuayi.cn

M. 命令行 / 进程 / 环境
来源：http://cl.szsharing.cn

================================================================================
来源：http://md.szxytkj.cn

[M01] 读取命令行参数
来源：http://jo.szsharing.cn

Py:   sys.argv[1:]
来源：http://gk.521024.cn

PHP:  $argv;  $argc;
来源：http://at.hahajie.cn

JS:   process.argv.slice(2)
来源：http://kk.hnjuh.cn

TS:   process.argv.slice(2)
来源：http://ty.jianghongdianzi.cn

Java: args 数组（main 方法参数）
来源：http://di.nicolike.cn

Go:   os.Args[1:]
来源：http://lx.colortex.cn

Ruby: ARGV
来源：http://ud.panjiajie.cn

C#:   args 数组（Main 方法参数）
来源：http://pi.huixinmuqiang.cn

[M02] 读取环境变量
来源：http://of.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://sk.haigaiapp.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ck.shxzskj.cn

JS:   process.env.HOME
来源：http://rk.9csxet.cn

TS:   process.env.HOME
来源：http://fo.gzmigu.cn

Java: System.getenv("HOME")
来源：http://oz.haigaiapp.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pn.shtwfgs.cn

Ruby: ENV["HOME"]
来源：http://of.colortex.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yr.nszjky.cn

[M03] 执行外部命令
来源：http://hz.szxytkj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ag.wgjwhj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ot.hnjuh.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jn.shxzskj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://he.colortex.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mt.wgjwhj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hv.wgjwhj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vz.nicolike.cn

C#:   Process.Start("ls", "-l");
来源：http://ao.szxytkj.cn

[M04] 获取当前工作目录
来源：http://zy.jctech888.com.cn

Py:   os.getcwd()
来源：http://hd.panjiajie.cn

PHP:  getcwd();
来源：http://wp.muxihuayi.cn

JS:   process.cwd()
来源：http://zs.bjjhwx.cn

TS:   process.cwd()
来源：http://rm.shxzskj.cn

Java: Path.of("").toAbsolutePath()
来源：http://ea.shxzskj.cn

Go:   os.Getwd()
来源：http://nv.jctech888.com.cn

Ruby: Dir.pwd
来源：http://qx.szxytkj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sq.shxzskj.cn

[M05] 设置退出码
来源：http://ae.colortex.cn

Py:   sys.exit(1)
来源：http://rb.shxzukj.cn

PHP:  exit(1);
来源：http://pm.nicolike.cn

JS:   process.exit(1)
来源：http://fi.gzmigu.cn

TS:   process.exit(1)
来源：http://wx.haigaiapp.cn

Java: System.exit(1)
来源：http://cd.panjiajie.cn

Go:   os.Exit(1)
来源：http://st.asd995.cn

Ruby: exit 1
来源：http://ki.9csxet.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://eq.asd995.cn

[M06] 向标准错误输出
来源：http://va.haigaiapp.cn

Py:   print("err", file=sys.stderr)
来源：http://vu.szxytkj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ga.colortex.cn

JS:   console.error("err")
来源：http://kc.wgjwhj.cn

TS:   console.error("err")
来源：http://uq.muxihuayi.cn

Java: System.err.println("err")
来源：http://rr.huixinmuqiang.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yc.szxytkj.cn

Ruby: warn "err"
来源：http://pa.shxzskj.cn

C#:   Console.Error.WriteLine("err")
来源：http://ja.asd995.cn

[M07] 判断是否为主入口
来源：http://wm.huixiangedu.cn

Py:   if __name__ == "__main__":
来源：http://jw.huanxung.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gw.nicolike.cn

JS:   require.main === module
来源：http://kj.asd995.cn

TS:   require.main === module
来源：http://yk.huanxung.cn

Java: public static void main(String[] args)
来源：http://ho.huixinmuqiang.cn

Go:   func main()
来源：http://vq.lnxyls.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://me.lnxyls.cn

C#:   static void Main(string[] args)
来源：http://bl.huanxung.cn

[M08] 获取系统与运行时信息
来源：http://pz.chemitech.net.cn

Py:   platform.system();  platform.python_version()
来源：http://dl.chemitech.net.cn

PHP:  PHP_OS;  phpversion();
来源：http://db.huixiangedu.cn

JS:   process.platform;  process.version
来源：http://dy.lnxyls.cn

TS:   process.platform;  process.version
来源：http://hb.shtwfgs.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://od.gzmigu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://lz.asd995.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zv.asd995.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://do.newstarts.cn

================================================================================
来源：http://xu.lnxyls.cn

N. 数据结构与算法
来源：http://on.muxihuayi.cn

================================================================================
来源：http://lp.nicolike.cn


<!-- 参考信息 -->