代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vl.hnjuh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jn.yuntaijiaju.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://on.yuntaijiaju.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ww.hnjuh.cn

[J03] 字符串解析为日期
来源：http://ae.hahajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gi.hnjuh.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fq.9csxet.cn

JS:   new Date("2024-01-02")
来源：http://bj.colortex.cn

TS:   new Date("2024-01-02")
来源：http://uj.wgjwhj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://po.nszjky.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ea.huanxung.cn

Ruby: Date.parse("2024-01-02")
来源：http://tf.huixiangedu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ku.nicolike.cn

[J04] 时间戳与日期互转
来源：http://fj.haigaiapp.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fv.szxytkj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ex.colortex.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sb.jctech888.com.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://mp.yuntaijiaju.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nr.nicolike.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wa.szsharing.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kl.colortex.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://oz.asd995.cn

[J05] 时间加减（加 7 天）
来源：http://gd.shxzukj.cn

Py:   now + timedelta(days=7)
来源：http://et.9csxet.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://oe.szxytkj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vl.asd995.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sx.huixinmuqiang.cn

Java: LocalDate.now().plusDays(7)
来源：http://er.9csxet.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bz.shxzskj.cn

Ruby: Time.now + 7 * 86400
来源：http://bn.chemitech.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bm.jctech888.com.cn

[J06] 计算两时间之差
来源：http://pe.muxihuayi.cn

Py:   (end - start).total_seconds()
来源：http://de.gzmigu.cn

PHP:  $end->diff($start)->days;
来源：http://un.yuntaijiaju.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qb.shxzukj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vc.nicolike.cn

Java: Duration.between(start, end).toSeconds()
来源：http://uq.nicolike.cn

Go:   end.Sub(start).Hours()
来源：http://zt.panjiajie.cn

Ruby: end - start                 # 返回秒数
来源：http://ug.shxzskj.cn

C#:   (end - start).TotalSeconds
来源：http://mw.jianghongdianzi.cn

[J07] 比较两个日期
来源：http://cv.bjjhwx.cn

Py:   d1 < d2;  d1 == d2
来源：http://of.shxzskj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pp.haigaiapp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://nk.bookmarksfly.cn

TS:   d1.getTime() < d2.getTime()
来源：http://af.huixinmuqiang.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uz.wgjwhj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rb.muxihuayi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://yv.huixinmuqiang.cn

C#:   d1 < d2;  d1 == d2
来源：http://sw.9csxet.cn

[J08] 提取年月日与星期
来源：http://sw.gzmigu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://at.huixinmuqiang.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ok.lnxyls.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://id.huixinmuqiang.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dq.jianghongdianzi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ai.521024.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gg.hahajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fv.nszjky.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pp.newstarts.cn

[J09] 时区处理
来源：http://ox.jctech888.com.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jj.asd995.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dz.bjjhwx.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pf.asd995.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ka.haigaiapp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nx.huixiangedu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://iq.newstarts.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://bp.gzmigu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lv.gzmigu.cn

[J10] 取今天 / 本月第一天
来源：http://og.hahajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rt.9csxet.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lq.newstarts.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fx.jctech888.com.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://no.shxzskj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cn.lnxyls.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pv.muxihuayi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qc.bjjhwx.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kp.hnjuh.cn

================================================================================
来源：http://bq.gzmigu.cn

K. JSON 与序列化
来源：http://oj.newstarts.cn

================================================================================
来源：http://pm.huixiangedu.cn

[K01] 对象转 JSON 字符串
来源：http://zx.wgjwhj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ch.panjiajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ax.nicolike.cn

JS:   JSON.stringify(obj)
来源：http://ds.colortex.cn

TS:   JSON.stringify(obj)
来源：http://hn.yuexingan06.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ga.muxihuayi.cn

Go:   json.Marshal(obj)
来源：http://tj.lnxyls.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ng.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dv.haigaiapp.cn

[K02] JSON 字符串转对象
来源：http://bh.lnxyls.cn

Py:   json.loads(s)
来源：http://yu.hahajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kb.huixinmuqiang.cn

JS:   JSON.parse(s)
来源：http://tt.shtwfgs.cn

TS:   JSON.parse(s)
来源：http://cj.shtwfgs.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zr.wgjwhj.cn

Go:   json.Unmarshal(data, &v)
来源：http://cp.muxihuayi.cn

Ruby: JSON.parse(s)
来源：http://ns.hnjuh.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vx.asd995.cn

[K03] JSON 美化输出（带缩进）
来源：http://mt.yuntaijiaju.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cf.huixiangedu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cn.hahajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ve.yuntaijiaju.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ge.jctech888.com.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zg.nicolike.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uq.huanxung.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bq.panjiajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ut.yuexingan06.cn

[K04] 读取 JSON 文件
来源：http://fa.shtwfgs.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dz.newstarts.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cc.shtwfgs.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://un.yuexingan06.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ex.szxytkj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yy.hahajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pj.shxzukj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://la.colortex.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uq.hnjuh.cn

[K05] 深拷贝对象
来源：http://cv.wgjwhj.cn

Py:   copy.deepcopy(obj)
来源：http://ex.9csxet.cn

PHP:  unserialize(serialize($obj));
来源：http://ro.szxytkj.cn

JS:   structuredClone(obj)
来源：http://oq.yuntaijiaju.cn

TS:   structuredClone(obj)
来源：http://aa.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ht.huanxung.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vw.nszjky.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bt.yuntaijiaju.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rb.jctech888.com.cn

[K06] 解析 URL 查询串
来源：http://lm.shxzskj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gg.shxzukj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mg.jctech888.com.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jv.lnxyls.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bk.yuexingan06.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yc.gzmigu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dp.yuntaijiaju.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rb.hnjuh.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ff.huixiangedu.cn

[K07] 进制转换
来源：http://mn.gzmigu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lw.huanxung.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xd.huanxung.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mx.shxzskj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sa.nicolike.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wg.newstarts.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://et.wgjwhj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qk.panjiajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ub.szsharing.cn

[K08] 二进制序列化（非 JSON）
来源：http://kd.nszjky.cn

Py:   pickle.dumps(obj)
来源：http://ls.hnjuh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ci.haigaiapp.cn

JS:   v8.serialize(obj)        // Node
来源：http://is.huixinmuqiang.cn

TS:   v8.serialize(obj)        // Node
来源：http://hm.nicolike.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zk.jianghongdianzi.cn

Go:   encoding/gob
来源：http://dv.huixiangedu.cn

Ruby: Marshal.dump(obj)
来源：http://ux.newstarts.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bb.yuexingan06.cn

================================================================================
来源：http://nb.haigaiapp.cn

L. 网络请求
来源：http://xo.nszjky.cn

================================================================================
来源：http://pa.nszjky.cn

[L01] 发送 GET 请求
来源：http://gq.muxihuayi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xg.yuexingan06.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://be.wgjwhj.cn

JS:   await fetch(url)
来源：http://xg.yuntaijiaju.cn

TS:   await fetch(url)
来源：http://sc.haigaiapp.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qq.bookmarksfly.cn

Go:   resp, err := http.Get(url)
来源：http://id.jctech888.com.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hw.chemitech.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://si.muxihuayi.cn

[L02] 发送 POST JSON
来源：http://us.yuntaijiaju.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zh.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kw.hahajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iw.yuntaijiaju.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lv.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xw.huanxung.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ih.jctech888.com.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mf.gzmigu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://le.huixinmuqiang.cn

[L03] 设置自定义请求头
来源：http://tl.szxytkj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yb.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fp.newstarts.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tx.colortex.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zi.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vj.gzmigu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://aq.chemitech.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://td.gzmigu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dx.wgjwhj.cn

[L04] 设置超时
来源：http://tp.yuexingan06.cn

Py:   requests.get(url, timeout=5)
来源：http://ky.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://on.shxzskj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ys.jctech888.com.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ar.shtwfgs.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cl.hnjuh.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fu.shxzukj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zb.szsharing.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ti.nszjky.cn

[L05] 上传文件（multipart）
来源：http://jl.szxytkj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vu.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lg.nszjky.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wd.yuntaijiaju.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bj.newstarts.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mq.hnjuh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ew.bjjhwx.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ce.szxytkj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jn.huanxung.cn

[L06] 解析响应为 JSON
来源：http://ly.shtwfgs.cn

Py:   resp.json()
来源：http://fa.hnjuh.cn

PHP:  json_decode($body, true);
来源：http://dp.hnjuh.cn

JS:   await resp.json()
来源：http://tr.szsharing.cn

TS:   await resp.json()
来源：http://sm.muxihuayi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rr.nicolike.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nm.bookmarksfly.cn

Ruby: JSON.parse(resp.body)
来源：http://mc.chemitech.net.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kz.nszjky.cn

[L07] 处理 HTTP 状态码
来源：http://jh.shtwfgs.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ar.newstarts.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://op.wgjwhj.cn

JS:   resp.ok;  resp.status
来源：http://va.9csxet.cn

TS:   resp.ok;  resp.status
来源：http://yf.shtwfgs.cn

Java: resp.statusCode()
来源：http://tw.hnjuh.cn

Go:   resp.StatusCode
来源：http://ls.nicolike.cn

Ruby: resp.code.to_i
来源：http://wx.huixiangedu.cn

C#:   (int)resp.StatusCode
来源：http://mu.panjiajie.cn

[L08] 并发请求多个地址
来源：http://ng.yuntaijiaju.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rd.yuexingan06.cn

PHP:  curl_multi_init() 系列
来源：http://sv.bookmarksfly.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kz.shxzukj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ud.szxytkj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qa.panjiajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://en.szxytkj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vw.shtwfgs.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gv.panjiajie.cn

================================================================================
来源：http://fn.bjjhwx.cn

M. 命令行 / 进程 / 环境
来源：http://xd.szxytkj.cn

================================================================================
来源：http://az.nicolike.cn

[M01] 读取命令行参数
来源：http://dk.shtwfgs.cn

Py:   sys.argv[1:]
来源：http://tt.panjiajie.cn

PHP:  $argv;  $argc;
来源：http://pv.yuexingan06.cn

JS:   process.argv.slice(2)
来源：http://or.haigaiapp.cn

TS:   process.argv.slice(2)
来源：http://vo.bookmarksfly.cn

Java: args 数组（main 方法参数）
来源：http://tz.gzmigu.cn

Go:   os.Args[1:]
来源：http://uq.huixiangedu.cn

Ruby: ARGV
来源：http://ro.bookmarksfly.cn

C#:   args 数组（Main 方法参数）
来源：http://tx.gzmigu.cn

[M02] 读取环境变量
来源：http://ke.jianghongdianzi.cn

Py:   os.environ.get("HOME")
来源：http://ak.nszjky.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qz.colortex.cn

JS:   process.env.HOME
来源：http://px.shtwfgs.cn

TS:   process.env.HOME
来源：http://vv.9csxet.cn

Java: System.getenv("HOME")
来源：http://tt.haigaiapp.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ht.panjiajie.cn

Ruby: ENV["HOME"]
来源：http://fi.jianghongdianzi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ey.jianghongdianzi.cn

[M03] 执行外部命令
来源：http://gb.asd995.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mn.yuntaijiaju.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://iz.colortex.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vp.hnjuh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://uk.shxzskj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ol.shxzskj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://be.newstarts.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gd.521024.cn

C#:   Process.Start("ls", "-l");
来源：http://eh.szxytkj.cn

[M04] 获取当前工作目录
来源：http://vq.huixiangedu.cn

Py:   os.getcwd()
来源：http://dl.colortex.cn

PHP:  getcwd();
来源：http://ld.gzmigu.cn

JS:   process.cwd()
来源：http://xd.panjiajie.cn

TS:   process.cwd()
来源：http://gh.yuexingan06.cn

Java: Path.of("").toAbsolutePath()
来源：http://yh.szxytkj.cn

Go:   os.Getwd()
来源：http://ie.shtwfgs.cn

Ruby: Dir.pwd
来源：http://hy.muxihuayi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jy.huanxung.cn

[M05] 设置退出码
来源：http://wt.wgjwhj.cn

Py:   sys.exit(1)
来源：http://to.521024.cn

PHP:  exit(1);
来源：http://um.colortex.cn

JS:   process.exit(1)
来源：http://xg.asd995.cn

TS:   process.exit(1)
来源：http://bn.shtwfgs.cn

Java: System.exit(1)
来源：http://tz.hahajie.cn

Go:   os.Exit(1)
来源：http://sq.jianghongdianzi.cn

Ruby: exit 1
来源：http://wk.asd995.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qp.hahajie.cn

[M06] 向标准错误输出
来源：http://wx.szsharing.cn

Py:   print("err", file=sys.stderr)
来源：http://ay.nszjky.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rl.chemitech.net.cn

JS:   console.error("err")
来源：http://rn.bookmarksfly.cn

TS:   console.error("err")
来源：http://yy.bookmarksfly.cn

Java: System.err.println("err")
来源：http://cl.chemitech.net.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gm.shxzukj.cn

Ruby: warn "err"
来源：http://fy.lnxyls.cn

C#:   Console.Error.WriteLine("err")
来源：http://ru.shxzukj.cn

[M07] 判断是否为主入口
来源：http://yt.newstarts.cn

Py:   if __name__ == "__main__":
来源：http://kq.nicolike.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xg.yuntaijiaju.cn

JS:   require.main === module
来源：http://aj.jctech888.com.cn

TS:   require.main === module
来源：http://pn.yuntaijiaju.cn

Java: public static void main(String[] args)
来源：http://rn.jctech888.com.cn

Go:   func main()
来源：http://xt.panjiajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ok.shxzukj.cn

C#:   static void Main(string[] args)
来源：http://os.asd995.cn

[M08] 获取系统与运行时信息
来源：http://ub.shxzukj.cn

Py:   platform.system();  platform.python_version()
来源：http://nr.newstarts.cn

PHP:  PHP_OS;  phpversion();
来源：http://ky.hnjuh.cn

JS:   process.platform;  process.version
来源：http://wq.chemitech.net.cn

TS:   process.platform;  process.version
来源：http://le.hahajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lg.hnjuh.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xq.shxzskj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pf.panjiajie.cn


<!-- 参考信息 -->