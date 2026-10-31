代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://uw.szxytkj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gs.shxzskj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ch.hahajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://us.huixiangedu.cn

[J03] 字符串解析为日期
来源：http://gn.shxzukj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://il.haigaiapp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://si.nicolike.cn

JS:   new Date("2024-01-02")
来源：http://mf.bookmarksfly.cn

TS:   new Date("2024-01-02")
来源：http://qu.newstarts.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gx.yuntaijiaju.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cf.panjiajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://jl.newstarts.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://oc.lnxyls.cn

[J04] 时间戳与日期互转
来源：http://qt.szsharing.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://un.shtwfgs.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tj.wgjwhj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ws.szxytkj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tl.nszjky.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tn.nszjky.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zj.521024.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pi.haigaiapp.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gv.huixiangedu.cn

[J05] 时间加减（加 7 天）
来源：http://qt.newstarts.cn

Py:   now + timedelta(days=7)
来源：http://li.colortex.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ur.huanxung.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pg.newstarts.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ne.asd995.cn

Java: LocalDate.now().plusDays(7)
来源：http://he.shtwfgs.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://id.haigaiapp.cn

Ruby: Time.now + 7 * 86400
来源：http://cb.huixinmuqiang.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ez.jctech888.com.cn

[J06] 计算两时间之差
来源：http://sq.wgjwhj.cn

Py:   (end - start).total_seconds()
来源：http://re.shxzskj.cn

PHP:  $end->diff($start)->days;
来源：http://af.nicolike.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vu.huixinmuqiang.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dg.shxzskj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lr.huixiangedu.cn

Go:   end.Sub(start).Hours()
来源：http://li.wgjwhj.cn

Ruby: end - start                 # 返回秒数
来源：http://uh.haigaiapp.cn

C#:   (end - start).TotalSeconds
来源：http://hi.szsharing.cn

[J07] 比较两个日期
来源：http://ny.colortex.cn

Py:   d1 < d2;  d1 == d2
来源：http://hy.hnjuh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cp.colortex.cn

JS:   d1.getTime() < d2.getTime()
来源：http://up.nszjky.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qn.shxzskj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jq.colortex.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ud.9csxet.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ap.lnxyls.cn

C#:   d1 < d2;  d1 == d2
来源：http://pk.wgjwhj.cn

[J08] 提取年月日与星期
来源：http://jn.hnjuh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jz.lnxyls.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qp.haigaiapp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jn.colortex.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kn.haigaiapp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://df.panjiajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kj.bookmarksfly.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pd.yuntaijiaju.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dx.newstarts.cn

[J09] 时区处理
来源：http://bx.bookmarksfly.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ar.bjjhwx.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gs.jianghongdianzi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fl.shxzukj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cg.wgjwhj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qu.shtwfgs.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fj.nicolike.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hx.szxytkj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fq.bjjhwx.cn

[J10] 取今天 / 本月第一天
来源：http://fs.shtwfgs.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vb.huixinmuqiang.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uk.nszjky.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vh.chemitech.net.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://aa.nszjky.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mi.9csxet.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dt.jianghongdianzi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mj.yuntaijiaju.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fz.9csxet.cn

================================================================================
来源：http://wl.521024.cn

K. JSON 与序列化
来源：http://um.nszjky.cn

================================================================================
来源：http://qn.hahajie.cn

[K01] 对象转 JSON 字符串
来源：http://dd.haigaiapp.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ux.yuexingan06.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bd.newstarts.cn

JS:   JSON.stringify(obj)
来源：http://df.huanxung.cn

TS:   JSON.stringify(obj)
来源：http://wj.shtwfgs.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kq.yuntaijiaju.cn

Go:   json.Marshal(obj)
来源：http://bk.huixinmuqiang.cn

Ruby: obj.to_json                                     // require "json"
来源：http://yu.szxytkj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bq.521024.cn

[K02] JSON 字符串转对象
来源：http://ja.9csxet.cn

Py:   json.loads(s)
来源：http://zk.szxytkj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cl.yuexingan06.cn

JS:   JSON.parse(s)
来源：http://mx.colortex.cn

TS:   JSON.parse(s)
来源：http://se.shxzskj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sn.bookmarksfly.cn

Go:   json.Unmarshal(data, &v)
来源：http://yp.bjjhwx.cn

Ruby: JSON.parse(s)
来源：http://ic.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://at.shxzukj.cn

[K03] JSON 美化输出（带缩进）
来源：http://dy.nszjky.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gg.bookmarksfly.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gh.chemitech.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ap.panjiajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vy.shxzskj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://er.panjiajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jy.nszjky.cn

Ruby: JSON.pretty_generate(obj)
来源：http://uf.hnjuh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dg.hahajie.cn

[K04] 读取 JSON 文件
来源：http://vy.wgjwhj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bn.newstarts.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yn.muxihuayi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ec.shxzukj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qi.wgjwhj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tz.colortex.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rd.chemitech.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ci.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ea.hnjuh.cn

[K05] 深拷贝对象
来源：http://ca.yuntaijiaju.cn

Py:   copy.deepcopy(obj)
来源：http://zp.huixinmuqiang.cn

PHP:  unserialize(serialize($obj));
来源：http://kz.bjjhwx.cn

JS:   structuredClone(obj)
来源：http://jh.haigaiapp.cn

TS:   structuredClone(obj)
来源：http://aq.huixiangedu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://eg.colortex.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qp.panjiajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yb.yuexingan06.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wu.huixinmuqiang.cn

[K06] 解析 URL 查询串
来源：http://rv.shxzskj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hp.newstarts.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://py.asd995.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bi.shtwfgs.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nc.bjjhwx.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ea.hahajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ak.yuexingan06.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qn.shxzukj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ho.yuexingan06.cn

[K07] 进制转换
来源：http://ei.huixinmuqiang.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uo.colortex.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://me.bjjhwx.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hf.hnjuh.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tf.colortex.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yd.hnjuh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dp.szsharing.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://la.hnjuh.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tx.wgjwhj.cn

[K08] 二进制序列化（非 JSON）
来源：http://pq.hahajie.cn

Py:   pickle.dumps(obj)
来源：http://fn.chemitech.net.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mr.chemitech.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://wh.szxytkj.cn

TS:   v8.serialize(obj)        // Node
来源：http://kd.huixinmuqiang.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ye.521024.cn

Go:   encoding/gob
来源：http://ib.huixiangedu.cn

Ruby: Marshal.dump(obj)
来源：http://dj.chemitech.net.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dq.asd995.cn

================================================================================
来源：http://et.521024.cn

L. 网络请求
来源：http://cr.shxzukj.cn

================================================================================
来源：http://gt.huixiangedu.cn

[L01] 发送 GET 请求
来源：http://in.hnjuh.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ez.shxzukj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bf.haigaiapp.cn

JS:   await fetch(url)
来源：http://lw.nszjky.cn

TS:   await fetch(url)
来源：http://oe.lnxyls.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xi.newstarts.cn

Go:   resp, err := http.Get(url)
来源：http://dk.yuntaijiaju.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://de.huixinmuqiang.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bg.wgjwhj.cn

[L02] 发送 POST JSON
来源：http://ik.gzmigu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mf.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lz.wgjwhj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hd.panjiajie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ue.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hr.hnjuh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ce.haigaiapp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://du.shxzskj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dn.gzmigu.cn

[L03] 设置自定义请求头
来源：http://kk.bjjhwx.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tg.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vi.szxytkj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xu.panjiajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xk.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ul.huixiangedu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ni.haigaiapp.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sg.szxytkj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qv.hnjuh.cn

[L04] 设置超时
来源：http://eo.shxzskj.cn

Py:   requests.get(url, timeout=5)
来源：http://yi.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://za.chemitech.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tp.colortex.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sz.bookmarksfly.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bi.huixinmuqiang.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gj.9csxet.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ru.panjiajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gk.muxihuayi.cn

[L05] 上传文件（multipart）
来源：http://wz.lnxyls.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://iw.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nj.chemitech.net.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sy.bookmarksfly.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://it.hnjuh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bv.haigaiapp.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vx.colortex.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hc.shxzukj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sy.asd995.cn

[L06] 解析响应为 JSON
来源：http://yk.huanxung.cn

Py:   resp.json()
来源：http://aw.lnxyls.cn

PHP:  json_decode($body, true);
来源：http://ci.jctech888.com.cn

JS:   await resp.json()
来源：http://vo.nicolike.cn

TS:   await resp.json()
来源：http://nd.chemitech.net.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kl.gzmigu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ly.shxzskj.cn

Ruby: JSON.parse(resp.body)
来源：http://ob.hnjuh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gv.huanxung.cn

[L07] 处理 HTTP 状态码
来源：http://ue.nszjky.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ia.colortex.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lq.szsharing.cn

JS:   resp.ok;  resp.status
来源：http://ee.lnxyls.cn

TS:   resp.ok;  resp.status
来源：http://nl.nicolike.cn

Java: resp.statusCode()
来源：http://uy.jianghongdianzi.cn

Go:   resp.StatusCode
来源：http://xu.asd995.cn

Ruby: resp.code.to_i
来源：http://ez.gzmigu.cn

C#:   (int)resp.StatusCode
来源：http://pk.chemitech.net.cn

[L08] 并发请求多个地址
来源：http://og.chemitech.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tw.hahajie.cn

PHP:  curl_multi_init() 系列
来源：http://iz.panjiajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gzmigu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sp.yuexingan06.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yh.jianghongdianzi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rs.jianghongdianzi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://og.jctech888.com.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bd.shxzukj.cn

================================================================================
来源：http://vf.muxihuayi.cn

M. 命令行 / 进程 / 环境
来源：http://ji.asd995.cn

================================================================================
来源：http://zt.yuexingan06.cn

[M01] 读取命令行参数
来源：http://sc.lnxyls.cn

Py:   sys.argv[1:]
来源：http://gy.hahajie.cn

PHP:  $argv;  $argc;
来源：http://xh.szxytkj.cn

JS:   process.argv.slice(2)
来源：http://nf.shtwfgs.cn

TS:   process.argv.slice(2)
来源：http://qk.bookmarksfly.cn

Java: args 数组（main 方法参数）
来源：http://op.muxihuayi.cn

Go:   os.Args[1:]
来源：http://cs.newstarts.cn

Ruby: ARGV
来源：http://fv.hnjuh.cn

C#:   args 数组（Main 方法参数）
来源：http://um.muxihuayi.cn

[M02] 读取环境变量
来源：http://ay.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://ai.huanxung.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ji.newstarts.cn

JS:   process.env.HOME
来源：http://us.yuntaijiaju.cn

TS:   process.env.HOME
来源：http://wt.colortex.cn

Java: System.getenv("HOME")
来源：http://xy.szxytkj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sp.nszjky.cn

Ruby: ENV["HOME"]
来源：http://nd.gzmigu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oq.yuexingan06.cn

[M03] 执行外部命令
来源：http://ub.szsharing.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yi.shxzskj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ja.wgjwhj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gw.hahajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://to.nszjky.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nm.shxzukj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://cu.wgjwhj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ka.shtwfgs.cn

C#:   Process.Start("ls", "-l");
来源：http://hh.colortex.cn

[M04] 获取当前工作目录
来源：http://za.nszjky.cn

Py:   os.getcwd()
来源：http://tx.szxytkj.cn

PHP:  getcwd();
来源：http://xs.asd995.cn

JS:   process.cwd()
来源：http://sk.panjiajie.cn

TS:   process.cwd()
来源：http://xc.hahajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://sa.bookmarksfly.cn

Go:   os.Getwd()
来源：http://xs.hahajie.cn

Ruby: Dir.pwd
来源：http://ek.wgjwhj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://er.panjiajie.cn

[M05] 设置退出码
来源：http://ak.521024.cn

Py:   sys.exit(1)
来源：http://bp.bjjhwx.cn

PHP:  exit(1);
来源：http://sp.colortex.cn

JS:   process.exit(1)
来源：http://gb.muxihuayi.cn

TS:   process.exit(1)
来源：http://br.asd995.cn

Java: System.exit(1)
来源：http://yt.shtwfgs.cn

Go:   os.Exit(1)
来源：http://lk.colortex.cn

Ruby: exit 1
来源：http://nq.huanxung.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cv.bookmarksfly.cn

[M06] 向标准错误输出
来源：http://ge.shxzukj.cn

Py:   print("err", file=sys.stderr)
来源：http://bg.yuexingan06.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://uq.521024.cn

JS:   console.error("err")
来源：http://kg.panjiajie.cn

TS:   console.error("err")
来源：http://vs.hnjuh.cn

Java: System.err.println("err")
来源：http://lm.huanxung.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://eo.colortex.cn

Ruby: warn "err"
来源：http://ea.szsharing.cn

C#:   Console.Error.WriteLine("err")
来源：http://jp.yuntaijiaju.cn

[M07] 判断是否为主入口
来源：http://iv.haigaiapp.cn

Py:   if __name__ == "__main__":
来源：http://kl.huixiangedu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rd.nszjky.cn

JS:   require.main === module
来源：http://dz.asd995.cn

TS:   require.main === module
来源：http://en.bookmarksfly.cn

Java: public static void main(String[] args)
来源：http://vd.lnxyls.cn

Go:   func main()
来源：http://aa.nszjky.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ek.colortex.cn

C#:   static void Main(string[] args)
来源：http://bt.newstarts.cn

[M08] 获取系统与运行时信息
来源：http://zy.yuntaijiaju.cn

Py:   platform.system();  platform.python_version()
来源：http://tf.muxihuayi.cn

PHP:  PHP_OS;  phpversion();
来源：http://yx.521024.cn

JS:   process.platform;  process.version
来源：http://ra.yuexingan06.cn

TS:   process.platform;  process.version
来源：http://np.colortex.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zp.shxzskj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zw.huanxung.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mr.gzmigu.cn


<!-- 参考信息 -->