代发 wailian999

[J03] 字符串解析为日期
来源：http://rs.hnjuh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pw.panjiajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://no.521024.cn

JS:   new Date("2024-01-02")
来源：http://gd.521024.cn

TS:   new Date("2024-01-02")
来源：http://ym.wgjwhj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fl.szxytkj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ch.yuexingan06.cn

Ruby: Date.parse("2024-01-02")
来源：http://ze.shxzskj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fo.chemitech.net.cn

[J04] 时间戳与日期互转
来源：http://sl.shxzskj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bu.shxzukj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qr.yuntaijiaju.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yw.shxzskj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dp.huixiangedu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yf.newstarts.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ib.yuexingan06.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ao.hahajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hq.wgjwhj.cn

[J05] 时间加减（加 7 天）
来源：http://vj.9csxet.cn

Py:   now + timedelta(days=7)
来源：http://ce.yuexingan06.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sn.haigaiapp.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zo.jctech888.com.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ia.szxytkj.cn

Java: LocalDate.now().plusDays(7)
来源：http://ru.asd995.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xt.chemitech.net.cn

Ruby: Time.now + 7 * 86400
来源：http://yc.colortex.cn

C#:   DateTime.Now.AddDays(7)
来源：http://yo.huanxung.cn

[J06] 计算两时间之差
来源：http://av.hnjuh.cn

Py:   (end - start).total_seconds()
来源：http://gy.shxzukj.cn

PHP:  $end->diff($start)->days;
来源：http://fl.9csxet.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wn.huixiangedu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mr.yuntaijiaju.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fk.shxzskj.cn

Go:   end.Sub(start).Hours()
来源：http://sb.shtwfgs.cn

Ruby: end - start                 # 返回秒数
来源：http://wz.bjjhwx.cn

C#:   (end - start).TotalSeconds
来源：http://sr.colortex.cn

[J07] 比较两个日期
来源：http://ra.huixiangedu.cn

Py:   d1 < d2;  d1 == d2
来源：http://dj.haigaiapp.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ol.jianghongdianzi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://op.huixinmuqiang.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xg.asd995.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ke.shtwfgs.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mj.huixiangedu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qs.hahajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://sj.bjjhwx.cn

[J08] 提取年月日与星期
来源：http://vf.colortex.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ti.lnxyls.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sq.newstarts.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vi.521024.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cn.asd995.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vy.huixinmuqiang.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ng.newstarts.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ye.chemitech.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tj.muxihuayi.cn

[J09] 时区处理
来源：http://ko.nszjky.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sc.9csxet.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://va.nszjky.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wj.chemitech.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zd.gzmigu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ms.shxzukj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bd.yuntaijiaju.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://rv.asd995.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sw.lnxyls.cn

[J10] 取今天 / 本月第一天
来源：http://hb.521024.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kh.huixiangedu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wo.yuexingan06.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://al.muxihuayi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sd.jctech888.com.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fl.nicolike.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bb.jctech888.com.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gz.jianghongdianzi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gp.lnxyls.cn

================================================================================
来源：http://hi.521024.cn

K. JSON 与序列化
来源：http://kz.muxihuayi.cn

================================================================================
来源：http://nh.asd995.cn

[K01] 对象转 JSON 字符串
来源：http://dz.lnxyls.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://az.newstarts.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ci.hnjuh.cn

JS:   JSON.stringify(obj)
来源：http://am.huixiangedu.cn

TS:   JSON.stringify(obj)
来源：http://vw.jianghongdianzi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://oz.lnxyls.cn

Go:   json.Marshal(obj)
来源：http://iz.shtwfgs.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nn.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vl.lnxyls.cn

[K02] JSON 字符串转对象
来源：http://ox.szxytkj.cn

Py:   json.loads(s)
来源：http://pm.yuntaijiaju.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qd.szxytkj.cn

JS:   JSON.parse(s)
来源：http://pq.gzmigu.cn

TS:   JSON.parse(s)
来源：http://df.jctech888.com.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lt.shtwfgs.cn

Go:   json.Unmarshal(data, &v)
来源：http://iq.yuexingan06.cn

Ruby: JSON.parse(s)
来源：http://ap.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uo.521024.cn

[K03] JSON 美化输出（带缩进）
来源：http://na.bjjhwx.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qf.yuexingan06.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yr.colortex.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://yj.asd995.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zj.hnjuh.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zo.yuexingan06.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qi.colortex.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fu.asd995.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hh.hnjuh.cn

[K04] 读取 JSON 文件
来源：http://xs.lnxyls.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vn.wgjwhj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://oc.wgjwhj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qy.panjiajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ww.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ma.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ne.yuntaijiaju.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ku.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kk.huanxung.cn

[K05] 深拷贝对象
来源：http://qh.muxihuayi.cn

Py:   copy.deepcopy(obj)
来源：http://at.panjiajie.cn

PHP:  unserialize(serialize($obj));
来源：http://vt.wgjwhj.cn

JS:   structuredClone(obj)
来源：http://dq.yuntaijiaju.cn

TS:   structuredClone(obj)
来源：http://eu.colortex.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gq.haigaiapp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xx.wgjwhj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vt.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mo.gzmigu.cn

[K06] 解析 URL 查询串
来源：http://xj.panjiajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vj.9csxet.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kt.chemitech.net.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mb.shxzukj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sm.shxzskj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://iz.bookmarksfly.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://eq.bookmarksfly.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://er.shxzskj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gv.szsharing.cn

[K07] 进制转换
来源：http://nq.bookmarksfly.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ac.9csxet.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vp.gzmigu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ki.bjjhwx.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://iw.shxzskj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rm.jianghongdianzi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ah.haigaiapp.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ne.shxzskj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xa.shxzukj.cn

[K08] 二进制序列化（非 JSON）
来源：http://vk.gzmigu.cn

Py:   pickle.dumps(obj)
来源：http://zu.szxytkj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://az.newstarts.cn

JS:   v8.serialize(obj)        // Node
来源：http://vj.gzmigu.cn

TS:   v8.serialize(obj)        // Node
来源：http://fv.panjiajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hd.yuexingan06.cn

Go:   encoding/gob
来源：http://qv.newstarts.cn

Ruby: Marshal.dump(obj)
来源：http://zv.szsharing.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jw.shxzskj.cn

================================================================================
来源：http://kl.9csxet.cn

L. 网络请求
来源：http://eb.wgjwhj.cn

================================================================================
来源：http://vi.9csxet.cn

[L01] 发送 GET 请求
来源：http://pj.haigaiapp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kj.panjiajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rg.huanxung.cn

JS:   await fetch(url)
来源：http://bi.huixiangedu.cn

TS:   await fetch(url)
来源：http://rd.huixiangedu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cl.9csxet.cn

Go:   resp, err := http.Get(url)
来源：http://pd.yuntaijiaju.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://yq.huixiangedu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yw.jctech888.com.cn

[L02] 发送 POST JSON
来源：http://ny.chemitech.net.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hn.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://td.jianghongdianzi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://no.panjiajie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qh.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jw.nicolike.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kn.shxzukj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://il.hahajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ts.chemitech.net.cn

[L03] 设置自定义请求头
来源：http://mb.szsharing.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sp.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dx.jianghongdianzi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ns.chemitech.net.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://st.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ch.jctech888.com.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://so.gzmigu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fz.asd995.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ny.hahajie.cn

[L04] 设置超时
来源：http://vw.szxytkj.cn

Py:   requests.get(url, timeout=5)
来源：http://nj.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ay.shxzskj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pt.shxzukj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ol.yuntaijiaju.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fl.newstarts.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vi.nicolike.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mt.9csxet.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ll.gzmigu.cn

[L05] 上传文件（multipart）
来源：http://wj.muxihuayi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wt.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zg.wgjwhj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rd.huanxung.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ae.shxzukj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ii.nszjky.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wi.wgjwhj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ai.bookmarksfly.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qv.shxzukj.cn

[L06] 解析响应为 JSON
来源：http://bf.huixiangedu.cn

Py:   resp.json()
来源：http://ca.shtwfgs.cn

PHP:  json_decode($body, true);
来源：http://tn.yuexingan06.cn

JS:   await resp.json()
来源：http://wh.nicolike.cn

TS:   await resp.json()
来源：http://ox.colortex.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fq.shxzskj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tx.jianghongdianzi.cn

Ruby: JSON.parse(resp.body)
来源：http://lz.wgjwhj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://iz.panjiajie.cn

[L07] 处理 HTTP 状态码
来源：http://wi.chemitech.net.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qc.panjiajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zq.colortex.cn

JS:   resp.ok;  resp.status
来源：http://jr.szxytkj.cn

TS:   resp.ok;  resp.status
来源：http://vi.wgjwhj.cn

Java: resp.statusCode()
来源：http://ia.bookmarksfly.cn

Go:   resp.StatusCode
来源：http://zd.szsharing.cn

Ruby: resp.code.to_i
来源：http://fs.shxzskj.cn

C#:   (int)resp.StatusCode
来源：http://pq.szxytkj.cn

[L08] 并发请求多个地址
来源：http://un.nszjky.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ab.shxzskj.cn

PHP:  curl_multi_init() 系列
来源：http://tf.9csxet.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://re.wgjwhj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bm.521024.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mo.haigaiapp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bu.bookmarksfly.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yu.hnjuh.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://js.huanxung.cn

================================================================================
来源：http://dy.newstarts.cn

M. 命令行 / 进程 / 环境
来源：http://od.gzmigu.cn

================================================================================
来源：http://et.shtwfgs.cn

[M01] 读取命令行参数
来源：http://tf.shxzskj.cn

Py:   sys.argv[1:]
来源：http://om.newstarts.cn

PHP:  $argv;  $argc;
来源：http://ws.wgjwhj.cn

JS:   process.argv.slice(2)
来源：http://nw.nicolike.cn

TS:   process.argv.slice(2)
来源：http://zz.bookmarksfly.cn

Java: args 数组（main 方法参数）
来源：http://rp.nicolike.cn

Go:   os.Args[1:]
来源：http://zh.nszjky.cn

Ruby: ARGV
来源：http://eh.gzmigu.cn

C#:   args 数组（Main 方法参数）
来源：http://ap.shxzskj.cn

[M02] 读取环境变量
来源：http://hj.huixinmuqiang.cn

Py:   os.environ.get("HOME")
来源：http://ok.huanxung.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vj.colortex.cn

JS:   process.env.HOME
来源：http://kp.yuexingan06.cn

TS:   process.env.HOME
来源：http://ov.szxytkj.cn

Java: System.getenv("HOME")
来源：http://sx.muxihuayi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lu.panjiajie.cn

Ruby: ENV["HOME"]
来源：http://qh.9csxet.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qd.shxzskj.cn

[M03] 执行外部命令
来源：http://vi.huanxung.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rk.jianghongdianzi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://oy.szsharing.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://px.shxzskj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ip.jianghongdianzi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zo.nszjky.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ui.shtwfgs.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fa.bjjhwx.cn

C#:   Process.Start("ls", "-l");
来源：http://zn.szsharing.cn

[M04] 获取当前工作目录
来源：http://xg.szsharing.cn

Py:   os.getcwd()
来源：http://lc.asd995.cn

PHP:  getcwd();
来源：http://td.9csxet.cn

JS:   process.cwd()
来源：http://rz.muxihuayi.cn

TS:   process.cwd()
来源：http://wl.panjiajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://qn.hnjuh.cn

Go:   os.Getwd()
来源：http://au.hahajie.cn

Ruby: Dir.pwd
来源：http://jv.lnxyls.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sz.asd995.cn

[M05] 设置退出码
来源：http://cz.panjiajie.cn

Py:   sys.exit(1)
来源：http://kz.shxzukj.cn

PHP:  exit(1);
来源：http://cr.huanxung.cn

JS:   process.exit(1)
来源：http://jm.szsharing.cn

TS:   process.exit(1)
来源：http://yg.panjiajie.cn

Java: System.exit(1)
来源：http://cx.521024.cn

Go:   os.Exit(1)
来源：http://si.yuntaijiaju.cn

Ruby: exit 1
来源：http://mc.yuexingan06.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://co.wgjwhj.cn

[M06] 向标准错误输出
来源：http://kl.jctech888.com.cn

Py:   print("err", file=sys.stderr)
来源：http://hk.huixinmuqiang.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ig.yuntaijiaju.cn

JS:   console.error("err")
来源：http://sx.szxytkj.cn

TS:   console.error("err")
来源：http://am.shtwfgs.cn

Java: System.err.println("err")
来源：http://ar.521024.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ou.521024.cn

Ruby: warn "err"
来源：http://ao.jianghongdianzi.cn

C#:   Console.Error.WriteLine("err")
来源：http://bz.jianghongdianzi.cn

[M07] 判断是否为主入口
来源：http://eo.asd995.cn

Py:   if __name__ == "__main__":
来源：http://vm.hahajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://up.bookmarksfly.cn

JS:   require.main === module
来源：http://ki.hahajie.cn

TS:   require.main === module
来源：http://nk.szxytkj.cn

Java: public static void main(String[] args)
来源：http://yn.nszjky.cn

Go:   func main()
来源：http://fb.szsharing.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://db.szxytkj.cn

C#:   static void Main(string[] args)
来源：http://or.muxihuayi.cn

[M08] 获取系统与运行时信息
来源：http://xz.521024.cn

Py:   platform.system();  platform.python_version()
来源：http://pl.yuexingan06.cn

PHP:  PHP_OS;  phpversion();
来源：http://ep.521024.cn

JS:   process.platform;  process.version
来源：http://jr.521024.cn

TS:   process.platform;  process.version
来源：http://hy.nszjky.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xj.wgjwhj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dq.shxzskj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sl.chemitech.net.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://mj.hahajie.cn

================================================================================
来源：http://cx.asd995.cn

N. 数据结构与算法
来源：http://zq.szxytkj.cn

================================================================================
来源：http://yr.panjiajie.cn


<!-- 参考信息 -->