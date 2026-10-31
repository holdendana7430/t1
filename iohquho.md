代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qn.jctech888.com.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tg.huixiangedu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nt.yuexingan06.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://oh.jctech888.com.cn

[J03] 字符串解析为日期
来源：http://vv.bjjhwx.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://am.colortex.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://su.haigaiapp.cn

JS:   new Date("2024-01-02")
来源：http://oy.haigaiapp.cn

TS:   new Date("2024-01-02")
来源：http://tl.huixiangedu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dm.szsharing.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jf.shtwfgs.cn

Ruby: Date.parse("2024-01-02")
来源：http://hk.huanxung.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rl.haigaiapp.cn

[J04] 时间戳与日期互转
来源：http://xo.yuntaijiaju.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://et.szsharing.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jq.9csxet.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cj.521024.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fb.nszjky.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xd.hnjuh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kx.nicolike.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xn.shxzukj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ys.shxzukj.cn

[J05] 时间加减（加 7 天）
来源：http://ba.asd995.cn

Py:   now + timedelta(days=7)
来源：http://mq.szxytkj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://gk.chemitech.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yf.wgjwhj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tr.9csxet.cn

Java: LocalDate.now().plusDays(7)
来源：http://xt.huixiangedu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sf.yuexingan06.cn

Ruby: Time.now + 7 * 86400
来源：http://ys.newstarts.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wn.bjjhwx.cn

[J06] 计算两时间之差
来源：http://xi.huanxung.cn

Py:   (end - start).total_seconds()
来源：http://qe.yuntaijiaju.cn

PHP:  $end->diff($start)->days;
来源：http://cq.yuntaijiaju.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bt.yuntaijiaju.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hm.chemitech.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://yy.521024.cn

Go:   end.Sub(start).Hours()
来源：http://fc.szsharing.cn

Ruby: end - start                 # 返回秒数
来源：http://oj.jctech888.com.cn

C#:   (end - start).TotalSeconds
来源：http://tx.hnjuh.cn

[J07] 比较两个日期
来源：http://gq.lnxyls.cn

Py:   d1 < d2;  d1 == d2
来源：http://ao.yuexingan06.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://os.huanxung.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rm.yuntaijiaju.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ap.szxytkj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nq.newstarts.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ka.panjiajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://tt.asd995.cn

C#:   d1 < d2;  d1 == d2
来源：http://pt.shxzskj.cn

[J08] 提取年月日与星期
来源：http://rh.shxzukj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zs.lnxyls.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://af.huanxung.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ra.shtwfgs.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://um.hahajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jn.yuntaijiaju.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ng.gzmigu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uu.bookmarksfly.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bw.9csxet.cn

[J09] 时区处理
来源：http://jj.jctech888.com.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://py.szxytkj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hv.yuexingan06.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pi.bjjhwx.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pg.asd995.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ct.yuexingan06.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wm.newstarts.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://az.shxzskj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yn.9csxet.cn

[J10] 取今天 / 本月第一天
来源：http://hb.bookmarksfly.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://uu.lnxyls.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pi.yuntaijiaju.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ni.bookmarksfly.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uy.lnxyls.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ap.lnxyls.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uy.jctech888.com.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ky.nszjky.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ml.newstarts.cn

================================================================================
来源：http://vw.nicolike.cn

K. JSON 与序列化
来源：http://wa.shxzukj.cn

================================================================================
来源：http://zy.szsharing.cn

[K01] 对象转 JSON 字符串
来源：http://ut.newstarts.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zv.nicolike.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kh.521024.cn

JS:   JSON.stringify(obj)
来源：http://xe.newstarts.cn

TS:   JSON.stringify(obj)
来源：http://xi.9csxet.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://om.9csxet.cn

Go:   json.Marshal(obj)
来源：http://ju.wgjwhj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ps.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://to.chemitech.net.cn

[K02] JSON 字符串转对象
来源：http://ku.9csxet.cn

Py:   json.loads(s)
来源：http://ki.newstarts.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://le.shtwfgs.cn

JS:   JSON.parse(s)
来源：http://mw.521024.cn

TS:   JSON.parse(s)
来源：http://fv.yuntaijiaju.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wr.bookmarksfly.cn

Go:   json.Unmarshal(data, &v)
来源：http://py.yuntaijiaju.cn

Ruby: JSON.parse(s)
来源：http://ky.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dn.lnxyls.cn

[K03] JSON 美化输出（带缩进）
来源：http://iq.yuntaijiaju.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ai.szxytkj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://be.shxzskj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ly.nszjky.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vx.huanxung.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hh.newstarts.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ul.shxzukj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ne.gzmigu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mi.chemitech.net.cn

[K04] 读取 JSON 文件
来源：http://sr.szxytkj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pg.jianghongdianzi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kt.asd995.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yj.huixinmuqiang.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yb.szsharing.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://at.szsharing.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jm.gzmigu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ki.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ty.huixiangedu.cn

[K05] 深拷贝对象
来源：http://yi.hahajie.cn

Py:   copy.deepcopy(obj)
来源：http://sp.panjiajie.cn

PHP:  unserialize(serialize($obj));
来源：http://rk.hahajie.cn

JS:   structuredClone(obj)
来源：http://xm.shtwfgs.cn

TS:   structuredClone(obj)
来源：http://pj.jctech888.com.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://aj.shtwfgs.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lz.bookmarksfly.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dq.chemitech.net.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dg.lnxyls.cn

[K06] 解析 URL 查询串
来源：http://yr.lnxyls.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gf.shxzskj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dp.hahajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://af.yuntaijiaju.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mu.bjjhwx.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://so.shxzskj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pg.huixinmuqiang.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bz.9csxet.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fb.shxzukj.cn

[K07] 进制转换
来源：http://eu.huixiangedu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://of.lnxyls.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rh.wgjwhj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mt.hnjuh.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xg.szsharing.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sa.yuexingan06.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nf.yuexingan06.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://up.hnjuh.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ip.shtwfgs.cn

[K08] 二进制序列化（非 JSON）
来源：http://om.huixinmuqiang.cn

Py:   pickle.dumps(obj)
来源：http://zv.asd995.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zw.shxzukj.cn

JS:   v8.serialize(obj)        // Node
来源：http://tn.yuntaijiaju.cn

TS:   v8.serialize(obj)        // Node
来源：http://xd.nszjky.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sf.9csxet.cn

Go:   encoding/gob
来源：http://um.yuexingan06.cn

Ruby: Marshal.dump(obj)
来源：http://xb.lnxyls.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yr.huixinmuqiang.cn

================================================================================
来源：http://su.bjjhwx.cn

L. 网络请求
来源：http://pg.nszjky.cn

================================================================================
来源：http://ye.colortex.cn

[L01] 发送 GET 请求
来源：http://mu.gzmigu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wy.lnxyls.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gx.521024.cn

JS:   await fetch(url)
来源：http://ij.haigaiapp.cn

TS:   await fetch(url)
来源：http://io.9csxet.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pc.bjjhwx.cn

Go:   resp, err := http.Get(url)
来源：http://gf.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://vq.jianghongdianzi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ah.huixiangedu.cn

[L02] 发送 POST JSON
来源：http://vl.wgjwhj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://sm.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qb.lnxyls.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xe.shtwfgs.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ma.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://en.shtwfgs.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wf.yuntaijiaju.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hr.521024.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gx.bjjhwx.cn

[L03] 设置自定义请求头
来源：http://qr.shxzukj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jg.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nw.hnjuh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sp.haigaiapp.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kb.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ge.chemitech.net.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mw.wgjwhj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pu.szxytkj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ep.wgjwhj.cn

[L04] 设置超时
来源：http://tk.muxihuayi.cn

Py:   requests.get(url, timeout=5)
来源：http://nv.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tj.jctech888.com.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://no.wgjwhj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ky.colortex.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://us.jianghongdianzi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ao.wgjwhj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gh.hahajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zp.nszjky.cn

[L05] 上传文件（multipart）
来源：http://mm.shxzskj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lv.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://oa.nszjky.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://po.huanxung.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yy.bookmarksfly.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bx.szsharing.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ye.lnxyls.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tn.gzmigu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zz.bookmarksfly.cn

[L06] 解析响应为 JSON
来源：http://yz.chemitech.net.cn

Py:   resp.json()
来源：http://oi.yuntaijiaju.cn

PHP:  json_decode($body, true);
来源：http://ho.bookmarksfly.cn

JS:   await resp.json()
来源：http://om.hahajie.cn

TS:   await resp.json()
来源：http://ov.muxihuayi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tv.asd995.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yp.colortex.cn

Ruby: JSON.parse(resp.body)
来源：http://bz.shxzskj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wl.yuntaijiaju.cn

[L07] 处理 HTTP 状态码
来源：http://wg.wgjwhj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uf.bookmarksfly.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xe.jianghongdianzi.cn

JS:   resp.ok;  resp.status
来源：http://ei.panjiajie.cn

TS:   resp.ok;  resp.status
来源：http://ja.huixiangedu.cn

Java: resp.statusCode()
来源：http://ca.nszjky.cn

Go:   resp.StatusCode
来源：http://la.panjiajie.cn

Ruby: resp.code.to_i
来源：http://ah.nszjky.cn

C#:   (int)resp.StatusCode
来源：http://ac.muxihuayi.cn

[L08] 并发请求多个地址
来源：http://yw.bjjhwx.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vl.wgjwhj.cn

PHP:  curl_multi_init() 系列
来源：http://pz.colortex.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zs.jctech888.com.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bu.yuexingan06.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gs.huixinmuqiang.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qb.yuexingan06.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zz.shxzskj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ha.haigaiapp.cn

================================================================================
来源：http://ys.panjiajie.cn

M. 命令行 / 进程 / 环境
来源：http://or.shtwfgs.cn

================================================================================
来源：http://ef.panjiajie.cn

[M01] 读取命令行参数
来源：http://gv.nicolike.cn

Py:   sys.argv[1:]
来源：http://br.shtwfgs.cn

PHP:  $argv;  $argc;
来源：http://ne.gzmigu.cn

JS:   process.argv.slice(2)
来源：http://ur.hnjuh.cn

TS:   process.argv.slice(2)
来源：http://dv.huixiangedu.cn

Java: args 数组（main 方法参数）
来源：http://my.szxytkj.cn

Go:   os.Args[1:]
来源：http://rm.yuexingan06.cn

Ruby: ARGV
来源：http://tu.9csxet.cn

C#:   args 数组（Main 方法参数）
来源：http://oy.jianghongdianzi.cn

[M02] 读取环境变量
来源：http://nv.szxytkj.cn

Py:   os.environ.get("HOME")
来源：http://ax.9csxet.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://re.bookmarksfly.cn

JS:   process.env.HOME
来源：http://sx.shxzskj.cn

TS:   process.env.HOME
来源：http://cj.panjiajie.cn

Java: System.getenv("HOME")
来源：http://zc.yuntaijiaju.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ho.haigaiapp.cn

Ruby: ENV["HOME"]
来源：http://ux.gzmigu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nf.wgjwhj.cn

[M03] 执行外部命令
来源：http://kl.wgjwhj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cd.yuexingan06.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://od.huanxung.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ik.chemitech.net.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rp.huixinmuqiang.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gs.szsharing.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://cw.bjjhwx.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bc.panjiajie.cn

C#:   Process.Start("ls", "-l");
来源：http://lo.9csxet.cn

[M04] 获取当前工作目录
来源：http://od.shxzukj.cn

Py:   os.getcwd()
来源：http://vt.hnjuh.cn

PHP:  getcwd();
来源：http://be.521024.cn

JS:   process.cwd()
来源：http://mz.haigaiapp.cn

TS:   process.cwd()
来源：http://fe.asd995.cn

Java: Path.of("").toAbsolutePath()
来源：http://im.nicolike.cn

Go:   os.Getwd()
来源：http://kf.521024.cn

Ruby: Dir.pwd
来源：http://fk.nicolike.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gl.chemitech.net.cn

[M05] 设置退出码
来源：http://rb.haigaiapp.cn

Py:   sys.exit(1)
来源：http://ot.9csxet.cn

PHP:  exit(1);
来源：http://ss.wgjwhj.cn

JS:   process.exit(1)
来源：http://od.lnxyls.cn

TS:   process.exit(1)
来源：http://tg.hahajie.cn

Java: System.exit(1)
来源：http://zn.9csxet.cn

Go:   os.Exit(1)
来源：http://mh.jctech888.com.cn

Ruby: exit 1
来源：http://bl.muxihuayi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vu.521024.cn

[M06] 向标准错误输出
来源：http://rq.wgjwhj.cn

Py:   print("err", file=sys.stderr)
来源：http://cm.asd995.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ix.muxihuayi.cn

JS:   console.error("err")
来源：http://lb.nszjky.cn

TS:   console.error("err")
来源：http://vx.szsharing.cn

Java: System.err.println("err")
来源：http://mu.wgjwhj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://oz.huixinmuqiang.cn

Ruby: warn "err"
来源：http://fr.nszjky.cn

C#:   Console.Error.WriteLine("err")
来源：http://cq.huixinmuqiang.cn

[M07] 判断是否为主入口
来源：http://wc.szxytkj.cn

Py:   if __name__ == "__main__":
来源：http://ii.muxihuayi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lu.yuntaijiaju.cn

JS:   require.main === module
来源：http://vv.bookmarksfly.cn

TS:   require.main === module
来源：http://et.521024.cn

Java: public static void main(String[] args)
来源：http://ao.szxytkj.cn

Go:   func main()
来源：http://th.chemitech.net.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ip.hnjuh.cn

C#:   static void Main(string[] args)
来源：http://hb.hnjuh.cn

[M08] 获取系统与运行时信息
来源：http://ac.jianghongdianzi.cn

Py:   platform.system();  platform.python_version()
来源：http://nt.shxzskj.cn

PHP:  PHP_OS;  phpversion();
来源：http://pq.huixiangedu.cn

JS:   process.platform;  process.version
来源：http://wr.lnxyls.cn

TS:   process.platform;  process.version
来源：http://wm.newstarts.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ss.chemitech.net.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://kj.chemitech.net.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ax.shxzukj.cn


<!-- 参考信息 -->