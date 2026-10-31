代发 wailian999

[J03] 字符串解析为日期
来源：http://yi.yuexingan06.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vs.muxihuayi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vn.wgjwhj.cn

JS:   new Date("2024-01-02")
来源：http://ix.9csxet.cn

TS:   new Date("2024-01-02")
来源：http://up.jctech888.com.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vd.jianghongdianzi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://re.muxihuayi.cn

Ruby: Date.parse("2024-01-02")
来源：http://hd.gzmigu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cb.9csxet.cn

[J04] 时间戳与日期互转
来源：http://th.newstarts.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ln.shxzskj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yx.nicolike.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rd.haigaiapp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://rp.bjjhwx.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xd.haigaiapp.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fx.shtwfgs.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zp.huanxung.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wy.asd995.cn

[J05] 时间加减（加 7 天）
来源：http://su.haigaiapp.cn

Py:   now + timedelta(days=7)
来源：http://bu.yuntaijiaju.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qe.shxzukj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sc.jianghongdianzi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fg.huixiangedu.cn

Java: LocalDate.now().plusDays(7)
来源：http://yr.hahajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vi.shtwfgs.cn

Ruby: Time.now + 7 * 86400
来源：http://wz.huixiangedu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bd.haigaiapp.cn

[J06] 计算两时间之差
来源：http://id.huanxung.cn

Py:   (end - start).total_seconds()
来源：http://jp.9csxet.cn

PHP:  $end->diff($start)->days;
来源：http://le.colortex.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kx.bookmarksfly.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qu.nszjky.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ea.shxzskj.cn

Go:   end.Sub(start).Hours()
来源：http://dd.huixiangedu.cn

Ruby: end - start                 # 返回秒数
来源：http://ke.hnjuh.cn

C#:   (end - start).TotalSeconds
来源：http://lo.shxzukj.cn

[J07] 比较两个日期
来源：http://km.panjiajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://ss.hahajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ra.muxihuayi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kq.asd995.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jw.colortex.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ld.nicolike.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sr.panjiajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wk.nicolike.cn

C#:   d1 < d2;  d1 == d2
来源：http://ut.bookmarksfly.cn

[J08] 提取年月日与星期
来源：http://nk.shxzskj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zh.haigaiapp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rz.lnxyls.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bw.huixiangedu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ez.9csxet.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dm.shtwfgs.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rv.hahajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jf.huixinmuqiang.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vi.gzmigu.cn

[J09] 时区处理
来源：http://xj.lnxyls.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uk.haigaiapp.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ss.nszjky.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yb.colortex.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dc.asd995.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sl.hahajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yy.hnjuh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ug.muxihuayi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://od.bookmarksfly.cn

[J10] 取今天 / 本月第一天
来源：http://wz.yuntaijiaju.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hp.yuntaijiaju.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vd.yuexingan06.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tl.asd995.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://po.newstarts.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jm.szxytkj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ll.shxzukj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bh.szsharing.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gb.lnxyls.cn

================================================================================
来源：http://em.lnxyls.cn

K. JSON 与序列化
来源：http://vt.jianghongdianzi.cn

================================================================================
来源：http://zj.shxzskj.cn

[K01] 对象转 JSON 字符串
来源：http://xv.shxzukj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ql.521024.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gh.asd995.cn

JS:   JSON.stringify(obj)
来源：http://nz.haigaiapp.cn

TS:   JSON.stringify(obj)
来源：http://mc.shxzskj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sk.yuntaijiaju.cn

Go:   json.Marshal(obj)
来源：http://jv.shxzukj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xm.huanxung.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yj.9csxet.cn

[K02] JSON 字符串转对象
来源：http://xc.chemitech.net.cn

Py:   json.loads(s)
来源：http://fb.9csxet.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vq.asd995.cn

JS:   JSON.parse(s)
来源：http://pt.szsharing.cn

TS:   JSON.parse(s)
来源：http://ti.jctech888.com.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://as.huixinmuqiang.cn

Go:   json.Unmarshal(data, &v)
来源：http://hi.huixiangedu.cn

Ruby: JSON.parse(s)
来源：http://gd.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ix.nicolike.cn

[K03] JSON 美化输出（带缩进）
来源：http://yk.haigaiapp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sh.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://go.jctech888.com.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ti.jianghongdianzi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ip.asd995.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yc.gzmigu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://el.hahajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wr.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://np.bjjhwx.cn

[K04] 读取 JSON 文件
来源：http://jf.nszjky.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dd.yuexingan06.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://su.huanxung.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fr.szxytkj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pu.asd995.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fl.shxzskj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dv.gzmigu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vi.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://aj.yuntaijiaju.cn

[K05] 深拷贝对象
来源：http://mo.9csxet.cn

Py:   copy.deepcopy(obj)
来源：http://ua.huixinmuqiang.cn

PHP:  unserialize(serialize($obj));
来源：http://dv.szxytkj.cn

JS:   structuredClone(obj)
来源：http://yr.bookmarksfly.cn

TS:   structuredClone(obj)
来源：http://rm.szsharing.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mq.jctech888.com.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nd.lnxyls.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vf.jianghongdianzi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xz.haigaiapp.cn

[K06] 解析 URL 查询串
来源：http://os.jctech888.com.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://do.yuexingan06.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xg.yuntaijiaju.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gf.yuexingan06.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sr.jctech888.com.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sv.haigaiapp.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://su.bookmarksfly.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tt.colortex.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cl.nicolike.cn

[K07] 进制转换
来源：http://rx.huixiangedu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gp.colortex.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dc.nicolike.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ml.shxzskj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gj.nszjky.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cg.colortex.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zh.huixiangedu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zq.bjjhwx.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xs.chemitech.net.cn

[K08] 二进制序列化（非 JSON）
来源：http://ah.huixiangedu.cn

Py:   pickle.dumps(obj)
来源：http://lj.nicolike.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://uq.colortex.cn

JS:   v8.serialize(obj)        // Node
来源：http://sm.shxzukj.cn

TS:   v8.serialize(obj)        // Node
来源：http://nk.huixinmuqiang.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yr.bjjhwx.cn

Go:   encoding/gob
来源：http://cn.521024.cn

Ruby: Marshal.dump(obj)
来源：http://sd.lnxyls.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://eb.newstarts.cn

================================================================================
来源：http://gr.wgjwhj.cn

L. 网络请求
来源：http://np.haigaiapp.cn

================================================================================
来源：http://zs.asd995.cn

[L01] 发送 GET 请求
来源：http://xr.hahajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qu.yuntaijiaju.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gd.colortex.cn

JS:   await fetch(url)
来源：http://ia.9csxet.cn

TS:   await fetch(url)
来源：http://oy.bjjhwx.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://og.shtwfgs.cn

Go:   resp, err := http.Get(url)
来源：http://lq.shtwfgs.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://sl.9csxet.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bb.yuexingan06.cn

[L02] 发送 POST JSON
来源：http://hr.bjjhwx.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bh.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gh.colortex.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://on.colortex.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://na.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pz.nicolike.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ql.bjjhwx.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qc.yuntaijiaju.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://it.haigaiapp.cn

[L03] 设置自定义请求头
来源：http://ak.yuntaijiaju.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gn.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ti.huanxung.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://st.szxytkj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ik.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ve.colortex.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ei.bookmarksfly.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ve.huixinmuqiang.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wn.gzmigu.cn

[L04] 设置超时
来源：http://sa.yuexingan06.cn

Py:   requests.get(url, timeout=5)
来源：http://fu.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vi.9csxet.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ia.yuntaijiaju.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://om.yuexingan06.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gq.shtwfgs.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bc.yuntaijiaju.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://op.chemitech.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ee.haigaiapp.cn

[L05] 上传文件（multipart）
来源：http://pu.panjiajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tp.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mk.haigaiapp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uy.chemitech.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ws.9csxet.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gf.jctech888.com.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hc.newstarts.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wq.jianghongdianzi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xy.9csxet.cn

[L06] 解析响应为 JSON
来源：http://yl.lnxyls.cn

Py:   resp.json()
来源：http://sa.haigaiapp.cn

PHP:  json_decode($body, true);
来源：http://gu.hnjuh.cn

JS:   await resp.json()
来源：http://qv.yuexingan06.cn

TS:   await resp.json()
来源：http://oq.huixiangedu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zy.colortex.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kc.nicolike.cn

Ruby: JSON.parse(resp.body)
来源：http://kp.panjiajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qj.521024.cn

[L07] 处理 HTTP 状态码
来源：http://bf.panjiajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vq.colortex.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vu.hahajie.cn

JS:   resp.ok;  resp.status
来源：http://th.jctech888.com.cn

TS:   resp.ok;  resp.status
来源：http://ut.bookmarksfly.cn

Java: resp.statusCode()
来源：http://fe.yuexingan06.cn

Go:   resp.StatusCode
来源：http://ed.muxihuayi.cn

Ruby: resp.code.to_i
来源：http://im.colortex.cn

C#:   (int)resp.StatusCode
来源：http://zw.hnjuh.cn

[L08] 并发请求多个地址
来源：http://iy.shtwfgs.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kd.huixiangedu.cn

PHP:  curl_multi_init() 系列
来源：http://kt.huanxung.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rd.9csxet.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sj.newstarts.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://aj.shtwfgs.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ik.gzmigu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://da.szxytkj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vm.hnjuh.cn

================================================================================
来源：http://he.shtwfgs.cn

M. 命令行 / 进程 / 环境
来源：http://nz.huixinmuqiang.cn

================================================================================
来源：http://ge.yuntaijiaju.cn

[M01] 读取命令行参数
来源：http://vf.muxihuayi.cn

Py:   sys.argv[1:]
来源：http://xm.chemitech.net.cn

PHP:  $argv;  $argc;
来源：http://bw.jctech888.com.cn

JS:   process.argv.slice(2)
来源：http://le.hnjuh.cn

TS:   process.argv.slice(2)
来源：http://am.asd995.cn

Java: args 数组（main 方法参数）
来源：http://bg.newstarts.cn

Go:   os.Args[1:]
来源：http://ca.jctech888.com.cn

Ruby: ARGV
来源：http://ia.jianghongdianzi.cn

C#:   args 数组（Main 方法参数）
来源：http://xv.newstarts.cn

[M02] 读取环境变量
来源：http://ww.shxzukj.cn

Py:   os.environ.get("HOME")
来源：http://fy.jctech888.com.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yw.panjiajie.cn

JS:   process.env.HOME
来源：http://xf.haigaiapp.cn

TS:   process.env.HOME
来源：http://hm.chemitech.net.cn

Java: System.getenv("HOME")
来源：http://zw.szxytkj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://um.yuntaijiaju.cn

Ruby: ENV["HOME"]
来源：http://qb.nszjky.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bw.lnxyls.cn

[M03] 执行外部命令
来源：http://ov.huixiangedu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lj.jctech888.com.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://oi.wgjwhj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ss.panjiajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ai.nicolike.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gj.9csxet.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vi.521024.cn

Ruby: system("ls -l");  `ls -l`
来源：http://sg.huixinmuqiang.cn

C#:   Process.Start("ls", "-l");
来源：http://uk.9csxet.cn

[M04] 获取当前工作目录
来源：http://id.bookmarksfly.cn

Py:   os.getcwd()
来源：http://cz.szxytkj.cn

PHP:  getcwd();
来源：http://ir.nszjky.cn

JS:   process.cwd()
来源：http://ek.hnjuh.cn

TS:   process.cwd()
来源：http://fb.huixiangedu.cn

Java: Path.of("").toAbsolutePath()
来源：http://tz.chemitech.net.cn

Go:   os.Getwd()
来源：http://ye.newstarts.cn

Ruby: Dir.pwd
来源：http://sq.chemitech.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://dd.shxzukj.cn

[M05] 设置退出码
来源：http://uw.shxzukj.cn

Py:   sys.exit(1)
来源：http://vo.newstarts.cn

PHP:  exit(1);
来源：http://el.szsharing.cn

JS:   process.exit(1)
来源：http://kh.bjjhwx.cn

TS:   process.exit(1)
来源：http://iv.shxzukj.cn

Java: System.exit(1)
来源：http://tw.huixiangedu.cn

Go:   os.Exit(1)
来源：http://ks.yuntaijiaju.cn

Ruby: exit 1
来源：http://lv.bjjhwx.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lv.szsharing.cn

[M06] 向标准错误输出
来源：http://iw.gzmigu.cn

Py:   print("err", file=sys.stderr)
来源：http://mq.hahajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hb.hahajie.cn

JS:   console.error("err")
来源：http://jd.szsharing.cn

TS:   console.error("err")
来源：http://hb.shxzukj.cn

Java: System.err.println("err")
来源：http://sp.hahajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://we.nszjky.cn

Ruby: warn "err"
来源：http://gr.yuntaijiaju.cn

C#:   Console.Error.WriteLine("err")
来源：http://pf.jctech888.com.cn

[M07] 判断是否为主入口
来源：http://wf.shtwfgs.cn

Py:   if __name__ == "__main__":
来源：http://ig.chemitech.net.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xc.newstarts.cn

JS:   require.main === module
来源：http://dy.wgjwhj.cn

TS:   require.main === module
来源：http://og.521024.cn

Java: public static void main(String[] args)
来源：http://in.hnjuh.cn

Go:   func main()
来源：http://au.bjjhwx.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kf.shtwfgs.cn

C#:   static void Main(string[] args)
来源：http://rv.wgjwhj.cn

[M08] 获取系统与运行时信息
来源：http://mz.wgjwhj.cn

Py:   platform.system();  platform.python_version()
来源：http://ji.muxihuayi.cn

PHP:  PHP_OS;  phpversion();
来源：http://ms.hahajie.cn

JS:   process.platform;  process.version
来源：http://wp.wgjwhj.cn

TS:   process.platform;  process.version
来源：http://nw.yuexingan06.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bs.yuntaijiaju.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://re.hahajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rt.hahajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ew.newstarts.cn

================================================================================
来源：http://df.shxzskj.cn

N. 数据结构与算法
来源：http://gc.yuexingan06.cn

================================================================================
来源：http://oy.shxzskj.cn


<!-- 参考信息 -->