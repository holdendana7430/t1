代发 wailian999

[J03] 字符串解析为日期
来源：http://ha.haigaiapp.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wz.haigaiapp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wy.yuntaijiaju.cn

JS:   new Date("2024-01-02")
来源：http://kx.521024.cn

TS:   new Date("2024-01-02")
来源：http://ia.bookmarksfly.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ki.yuexingan06.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ob.szxytkj.cn

Ruby: Date.parse("2024-01-02")
来源：http://xt.haigaiapp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://po.colortex.cn

[J04] 时间戳与日期互转
来源：http://cl.huixinmuqiang.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ep.newstarts.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://iw.muxihuayi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ua.muxihuayi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zv.huixinmuqiang.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lj.shxzskj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nd.gzmigu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ol.yuntaijiaju.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vm.panjiajie.cn

[J05] 时间加减（加 7 天）
来源：http://gi.colortex.cn

Py:   now + timedelta(days=7)
来源：http://tf.nszjky.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://uj.colortex.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hj.yuntaijiaju.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kj.shxzukj.cn

Java: LocalDate.now().plusDays(7)
来源：http://wr.panjiajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lw.gzmigu.cn

Ruby: Time.now + 7 * 86400
来源：http://in.yuexingan06.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kf.huixiangedu.cn

[J06] 计算两时间之差
来源：http://kk.shxzukj.cn

Py:   (end - start).total_seconds()
来源：http://lz.colortex.cn

PHP:  $end->diff($start)->days;
来源：http://dp.newstarts.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tj.bjjhwx.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mr.szsharing.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jz.lnxyls.cn

Go:   end.Sub(start).Hours()
来源：http://xv.yuntaijiaju.cn

Ruby: end - start                 # 返回秒数
来源：http://xn.gzmigu.cn

C#:   (end - start).TotalSeconds
来源：http://kh.hnjuh.cn

[J07] 比较两个日期
来源：http://vp.huixiangedu.cn

Py:   d1 < d2;  d1 == d2
来源：http://tf.huixinmuqiang.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nh.521024.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kq.szxytkj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qa.521024.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ri.huanxung.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://iu.hahajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ct.colortex.cn

C#:   d1 < d2;  d1 == d2
来源：http://ll.hahajie.cn

[J08] 提取年月日与星期
来源：http://hz.521024.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ma.jctech888.com.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pb.haigaiapp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tg.yuntaijiaju.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tg.shtwfgs.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bq.521024.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wl.yuexingan06.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://aw.wgjwhj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yi.nicolike.cn

[J09] 时区处理
来源：http://ib.asd995.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://en.bookmarksfly.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://im.jianghongdianzi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://og.521024.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pd.shxzukj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jz.shxzskj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pt.jctech888.com.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ak.bookmarksfly.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kf.yuexingan06.cn

[J10] 取今天 / 本月第一天
来源：http://im.shtwfgs.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zh.panjiajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cf.hahajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://os.asd995.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yk.chemitech.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hh.newstarts.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ik.shtwfgs.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://th.huanxung.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ex.jctech888.com.cn

================================================================================
来源：http://aj.shtwfgs.cn

K. JSON 与序列化
来源：http://dn.huixinmuqiang.cn

================================================================================
来源：http://fh.yuexingan06.cn

[K01] 对象转 JSON 字符串
来源：http://zn.gzmigu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hi.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://iz.shtwfgs.cn

JS:   JSON.stringify(obj)
来源：http://xt.chemitech.net.cn

TS:   JSON.stringify(obj)
来源：http://hw.chemitech.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xy.jctech888.com.cn

Go:   json.Marshal(obj)
来源：http://eq.hahajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mu.gzmigu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pg.shtwfgs.cn

[K02] JSON 字符串转对象
来源：http://fr.szxytkj.cn

Py:   json.loads(s)
来源：http://bi.9csxet.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tq.huixinmuqiang.cn

JS:   JSON.parse(s)
来源：http://js.hnjuh.cn

TS:   JSON.parse(s)
来源：http://qt.bjjhwx.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xa.9csxet.cn

Go:   json.Unmarshal(data, &v)
来源：http://ht.muxihuayi.cn

Ruby: JSON.parse(s)
来源：http://ow.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kq.panjiajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://eb.panjiajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yf.yuexingan06.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sw.haigaiapp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bd.gzmigu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mq.yuexingan06.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bi.yuntaijiaju.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nd.yuntaijiaju.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ar.hahajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://iq.huixiangedu.cn

[K04] 读取 JSON 文件
来源：http://vv.bookmarksfly.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jj.muxihuayi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cj.bookmarksfly.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zi.hnjuh.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zp.gzmigu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://su.szsharing.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mm.9csxet.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ca.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lz.huanxung.cn

[K05] 深拷贝对象
来源：http://js.9csxet.cn

Py:   copy.deepcopy(obj)
来源：http://hy.jctech888.com.cn

PHP:  unserialize(serialize($obj));
来源：http://pc.shxzukj.cn

JS:   structuredClone(obj)
来源：http://no.shxzukj.cn

TS:   structuredClone(obj)
来源：http://zk.521024.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zy.muxihuayi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wp.shxzukj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mx.chemitech.net.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cm.shxzskj.cn

[K06] 解析 URL 查询串
来源：http://sp.haigaiapp.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://do.colortex.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ee.yuntaijiaju.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oo.9csxet.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ac.521024.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wd.hnjuh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cu.asd995.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mh.szxytkj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fb.newstarts.cn

[K07] 进制转换
来源：http://le.newstarts.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://oe.huixiangedu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://al.huixinmuqiang.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ls.colortex.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://st.shtwfgs.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yk.hnjuh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ev.nszjky.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dm.lnxyls.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yl.nszjky.cn

[K08] 二进制序列化（非 JSON）
来源：http://ai.haigaiapp.cn

Py:   pickle.dumps(obj)
来源：http://mg.szsharing.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://uc.szxytkj.cn

JS:   v8.serialize(obj)        // Node
来源：http://fr.bookmarksfly.cn

TS:   v8.serialize(obj)        // Node
来源：http://mt.gzmigu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rj.szxytkj.cn

Go:   encoding/gob
来源：http://yd.wgjwhj.cn

Ruby: Marshal.dump(obj)
来源：http://fv.521024.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ul.huixiangedu.cn

================================================================================
来源：http://sh.haigaiapp.cn

L. 网络请求
来源：http://wf.wgjwhj.cn

================================================================================
来源：http://nj.jianghongdianzi.cn

[L01] 发送 GET 请求
来源：http://ph.yuntaijiaju.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vu.nicolike.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gy.panjiajie.cn

JS:   await fetch(url)
来源：http://dk.newstarts.cn

TS:   await fetch(url)
来源：http://ci.jianghongdianzi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ev.wgjwhj.cn

Go:   resp, err := http.Get(url)
来源：http://py.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fn.newstarts.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xo.nszjky.cn

[L02] 发送 POST JSON
来源：http://oe.szxytkj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://us.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ek.521024.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wq.yuntaijiaju.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sj.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://je.521024.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fx.huixinmuqiang.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mb.wgjwhj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://es.nszjky.cn

[L03] 设置自定义请求头
来源：http://lb.shtwfgs.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://no.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zy.wgjwhj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pu.9csxet.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://en.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uv.nszjky.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wk.asd995.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gd.nszjky.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nr.huixinmuqiang.cn

[L04] 设置超时
来源：http://cu.gzmigu.cn

Py:   requests.get(url, timeout=5)
来源：http://zn.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pa.bjjhwx.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wp.nszjky.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ic.huanxung.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bp.huixiangedu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cp.lnxyls.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ey.panjiajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fj.huixiangedu.cn

[L05] 上传文件（multipart）
来源：http://mn.szsharing.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dq.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pp.szsharing.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qq.wgjwhj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jn.hnjuh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dx.yuntaijiaju.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rg.colortex.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ti.szsharing.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ya.chemitech.net.cn

[L06] 解析响应为 JSON
来源：http://el.yuexingan06.cn

Py:   resp.json()
来源：http://yv.bjjhwx.cn

PHP:  json_decode($body, true);
来源：http://oc.yuexingan06.cn

JS:   await resp.json()
来源：http://bl.huixinmuqiang.cn

TS:   await resp.json()
来源：http://yr.jianghongdianzi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fu.nszjky.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://le.muxihuayi.cn

Ruby: JSON.parse(resp.body)
来源：http://uy.9csxet.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ft.wgjwhj.cn

[L07] 处理 HTTP 状态码
来源：http://qg.bjjhwx.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uh.jianghongdianzi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://po.nicolike.cn

JS:   resp.ok;  resp.status
来源：http://za.shtwfgs.cn

TS:   resp.ok;  resp.status
来源：http://jg.9csxet.cn

Java: resp.statusCode()
来源：http://wi.huixinmuqiang.cn

Go:   resp.StatusCode
来源：http://jg.jctech888.com.cn

Ruby: resp.code.to_i
来源：http://he.shtwfgs.cn

C#:   (int)resp.StatusCode
来源：http://tu.lnxyls.cn

[L08] 并发请求多个地址
来源：http://ne.muxihuayi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://eg.bookmarksfly.cn

PHP:  curl_multi_init() 系列
来源：http://ty.szxytkj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bm.521024.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gj.9csxet.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bu.hnjuh.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kz.shtwfgs.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gg.colortex.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ye.9csxet.cn

================================================================================
来源：http://rk.521024.cn

M. 命令行 / 进程 / 环境
来源：http://jc.huixinmuqiang.cn

================================================================================
来源：http://rm.hahajie.cn

[M01] 读取命令行参数
来源：http://ne.szsharing.cn

Py:   sys.argv[1:]
来源：http://ua.shxzskj.cn

PHP:  $argv;  $argc;
来源：http://xa.wgjwhj.cn

JS:   process.argv.slice(2)
来源：http://gf.huixinmuqiang.cn

TS:   process.argv.slice(2)
来源：http://gp.chemitech.net.cn

Java: args 数组（main 方法参数）
来源：http://rw.yuntaijiaju.cn

Go:   os.Args[1:]
来源：http://un.gzmigu.cn

Ruby: ARGV
来源：http://dl.wgjwhj.cn

C#:   args 数组（Main 方法参数）
来源：http://uq.hnjuh.cn

[M02] 读取环境变量
来源：http://hb.muxihuayi.cn

Py:   os.environ.get("HOME")
来源：http://hv.521024.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yb.asd995.cn

JS:   process.env.HOME
来源：http://lv.chemitech.net.cn

TS:   process.env.HOME
来源：http://eh.asd995.cn

Java: System.getenv("HOME")
来源：http://ry.jctech888.com.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gw.jctech888.com.cn

Ruby: ENV["HOME"]
来源：http://ah.9csxet.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lb.chemitech.net.cn

[M03] 执行外部命令
来源：http://df.wgjwhj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gw.szsharing.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ud.newstarts.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ru.hahajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://bz.huanxung.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://aj.huixinmuqiang.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://tl.521024.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qt.jianghongdianzi.cn

C#:   Process.Start("ls", "-l");
来源：http://rb.hnjuh.cn

[M04] 获取当前工作目录
来源：http://lg.521024.cn

Py:   os.getcwd()
来源：http://dn.huixinmuqiang.cn

PHP:  getcwd();
来源：http://mp.huanxung.cn

JS:   process.cwd()
来源：http://cp.muxihuayi.cn

TS:   process.cwd()
来源：http://og.panjiajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://xx.shtwfgs.cn

Go:   os.Getwd()
来源：http://xh.shxzskj.cn

Ruby: Dir.pwd
来源：http://rq.bookmarksfly.cn

C#:   Directory.GetCurrentDirectory()
来源：http://as.nicolike.cn

[M05] 设置退出码
来源：http://pr.lnxyls.cn

Py:   sys.exit(1)
来源：http://hj.bookmarksfly.cn

PHP:  exit(1);
来源：http://za.hnjuh.cn

JS:   process.exit(1)
来源：http://of.bookmarksfly.cn

TS:   process.exit(1)
来源：http://po.szxytkj.cn

Java: System.exit(1)
来源：http://zl.bjjhwx.cn

Go:   os.Exit(1)
来源：http://ay.yuexingan06.cn

Ruby: exit 1
来源：http://lu.muxihuayi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://za.shtwfgs.cn

[M06] 向标准错误输出
来源：http://ac.huanxung.cn

Py:   print("err", file=sys.stderr)
来源：http://sx.asd995.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kw.muxihuayi.cn

JS:   console.error("err")
来源：http://dq.newstarts.cn

TS:   console.error("err")
来源：http://xi.szsharing.cn

Java: System.err.println("err")
来源：http://ts.asd995.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rv.hnjuh.cn

Ruby: warn "err"
来源：http://ic.lnxyls.cn

C#:   Console.Error.WriteLine("err")
来源：http://ss.wgjwhj.cn

[M07] 判断是否为主入口
来源：http://ko.nszjky.cn

Py:   if __name__ == "__main__":
来源：http://le.muxihuayi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yv.jctech888.com.cn

JS:   require.main === module
来源：http://ka.gzmigu.cn

TS:   require.main === module
来源：http://il.yuntaijiaju.cn

Java: public static void main(String[] args)
来源：http://tn.hahajie.cn

Go:   func main()
来源：http://hv.nszjky.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lm.521024.cn

C#:   static void Main(string[] args)
来源：http://kw.shxzskj.cn

[M08] 获取系统与运行时信息
来源：http://fa.521024.cn

Py:   platform.system();  platform.python_version()
来源：http://xb.hahajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://gq.jianghongdianzi.cn

JS:   process.platform;  process.version
来源：http://qn.521024.cn

TS:   process.platform;  process.version
来源：http://if.huixiangedu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fi.bookmarksfly.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yl.newstarts.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gb.hnjuh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qz.huixiangedu.cn

================================================================================
来源：http://cs.hahajie.cn

N. 数据结构与算法
来源：http://km.wgjwhj.cn

================================================================================
来源：http://pw.huanxung.cn


<!-- 参考信息 -->