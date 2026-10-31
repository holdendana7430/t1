代发 wailian999

Go:   time.Now()
来源：http://pn.jctech888.com.cn

Ruby: Time.now
来源：http://kn.huixiangedu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gs.9csxet.cn

[J02] 格式化输出
来源：http://yd.nszjky.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ix.jctech888.com.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nn.chemitech.net.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tc.yuexingan06.cn

TS:   d.toISOString()
来源：http://bg.newstarts.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qv.shtwfgs.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lj.lnxyls.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vg.haigaiapp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ig.jianghongdianzi.cn

[J03] 字符串解析为日期
来源：http://nh.shxzskj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lu.huixiangedu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sk.521024.cn

JS:   new Date("2024-01-02")
来源：http://ef.shtwfgs.cn

TS:   new Date("2024-01-02")
来源：http://pi.nicolike.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jb.shxzukj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hw.szsharing.cn

Ruby: Date.parse("2024-01-02")
来源：http://yh.haigaiapp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://aa.nicolike.cn

[J04] 时间戳与日期互转
来源：http://hg.nszjky.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ph.jianghongdianzi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://im.lnxyls.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ex.521024.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dp.bookmarksfly.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cd.shxzukj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sm.521024.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ka.wgjwhj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://io.huanxung.cn

[J05] 时间加减（加 7 天）
来源：http://ub.panjiajie.cn

Py:   now + timedelta(days=7)
来源：http://ys.jctech888.com.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://hq.9csxet.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vq.newstarts.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ab.yuntaijiaju.cn

Java: LocalDate.now().plusDays(7)
来源：http://sv.haigaiapp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lz.jctech888.com.cn

Ruby: Time.now + 7 * 86400
来源：http://mf.9csxet.cn

C#:   DateTime.Now.AddDays(7)
来源：http://er.hahajie.cn

[J06] 计算两时间之差
来源：http://ty.szsharing.cn

Py:   (end - start).total_seconds()
来源：http://ks.szsharing.cn

PHP:  $end->diff($start)->days;
来源：http://mq.huixiangedu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rv.huixinmuqiang.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mf.asd995.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vg.jianghongdianzi.cn

Go:   end.Sub(start).Hours()
来源：http://vw.huanxung.cn

Ruby: end - start                 # 返回秒数
来源：http://av.szsharing.cn

C#:   (end - start).TotalSeconds
来源：http://om.chemitech.net.cn

[J07] 比较两个日期
来源：http://uo.newstarts.cn

Py:   d1 < d2;  d1 == d2
来源：http://fp.chemitech.net.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://li.gzmigu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hb.shtwfgs.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ly.wgjwhj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jb.colortex.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kw.gzmigu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jv.szxytkj.cn

C#:   d1 < d2;  d1 == d2
来源：http://ac.jctech888.com.cn

[J08] 提取年月日与星期
来源：http://hv.huixiangedu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qt.yuexingan06.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vg.szsharing.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mh.szxytkj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://en.asd995.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kl.hahajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yu.bjjhwx.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sx.shtwfgs.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://it.huanxung.cn

[J09] 时区处理
来源：http://ae.hnjuh.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://il.lnxyls.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ho.bjjhwx.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pk.jianghongdianzi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xo.lnxyls.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qt.jianghongdianzi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gu.shtwfgs.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qq.nicolike.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uh.hnjuh.cn

[J10] 取今天 / 本月第一天
来源：http://qq.shxzukj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ju.yuntaijiaju.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ud.hnjuh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://az.bookmarksfly.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iy.gzmigu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mv.haigaiapp.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dr.haigaiapp.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pw.haigaiapp.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wj.gzmigu.cn

================================================================================
来源：http://ax.muxihuayi.cn

K. JSON 与序列化
来源：http://ny.huixinmuqiang.cn

================================================================================
来源：http://dt.jctech888.com.cn

[K01] 对象转 JSON 字符串
来源：http://vm.szxytkj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lg.shxzskj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gp.bookmarksfly.cn

JS:   JSON.stringify(obj)
来源：http://jz.asd995.cn

TS:   JSON.stringify(obj)
来源：http://kp.nszjky.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://om.yuntaijiaju.cn

Go:   json.Marshal(obj)
来源：http://oe.panjiajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nt.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jd.jctech888.com.cn

[K02] JSON 字符串转对象
来源：http://jf.huixinmuqiang.cn

Py:   json.loads(s)
来源：http://ma.nszjky.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ep.yuexingan06.cn

JS:   JSON.parse(s)
来源：http://hm.bjjhwx.cn

TS:   JSON.parse(s)
来源：http://ka.jianghongdianzi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gb.jianghongdianzi.cn

Go:   json.Unmarshal(data, &v)
来源：http://mk.hahajie.cn

Ruby: JSON.parse(s)
来源：http://tv.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bj.nszjky.cn

[K03] JSON 美化输出（带缩进）
来源：http://bq.jianghongdianzi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ci.yuexingan06.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ac.yuntaijiaju.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bi.bookmarksfly.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wg.shxzukj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oe.gzmigu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fc.szsharing.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qs.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://js.shtwfgs.cn

[K04] 读取 JSON 文件
来源：http://ja.muxihuayi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pr.521024.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lm.wgjwhj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://un.huixiangedu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lj.colortex.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pi.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kf.colortex.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://us.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://og.gzmigu.cn

[K05] 深拷贝对象
来源：http://xn.huanxung.cn

Py:   copy.deepcopy(obj)
来源：http://ln.huanxung.cn

PHP:  unserialize(serialize($obj));
来源：http://iv.yuexingan06.cn

JS:   structuredClone(obj)
来源：http://qv.colortex.cn

TS:   structuredClone(obj)
来源：http://xd.nszjky.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ih.nicolike.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kp.hnjuh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ls.bookmarksfly.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ha.nicolike.cn

[K06] 解析 URL 查询串
来源：http://ct.jctech888.com.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zl.nicolike.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://uf.shxzukj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mj.lnxyls.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tz.jianghongdianzi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rm.yuntaijiaju.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cy.szsharing.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gp.chemitech.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rg.nicolike.cn

[K07] 进制转换
来源：http://bl.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ia.521024.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zx.lnxyls.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qy.huanxung.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yo.nicolike.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jv.lnxyls.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ab.bookmarksfly.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uo.hahajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cb.newstarts.cn

[K08] 二进制序列化（非 JSON）
来源：http://dn.bjjhwx.cn

Py:   pickle.dumps(obj)
来源：http://im.nszjky.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yi.gzmigu.cn

JS:   v8.serialize(obj)        // Node
来源：http://ym.shxzskj.cn

TS:   v8.serialize(obj)        // Node
来源：http://ml.szxytkj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pj.wgjwhj.cn

Go:   encoding/gob
来源：http://cp.9csxet.cn

Ruby: Marshal.dump(obj)
来源：http://ss.nszjky.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://iz.9csxet.cn

================================================================================
来源：http://mk.haigaiapp.cn

L. 网络请求
来源：http://ig.szxytkj.cn

================================================================================
来源：http://kr.huixinmuqiang.cn

[L01] 发送 GET 请求
来源：http://vf.newstarts.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lb.jctech888.com.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vn.nicolike.cn

JS:   await fetch(url)
来源：http://qs.nszjky.cn

TS:   await fetch(url)
来源：http://sj.chemitech.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fb.huanxung.cn

Go:   resp, err := http.Get(url)
来源：http://hu.9csxet.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ga.huixiangedu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cb.jctech888.com.cn

[L02] 发送 POST JSON
来源：http://dn.shxzskj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mi.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sp.hnjuh.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ie.shxzukj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ma.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sw.gzmigu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ge.asd995.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hh.shxzukj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jg.jctech888.com.cn

[L03] 设置自定义请求头
来源：http://xn.jctech888.com.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xo.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lt.lnxyls.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nl.panjiajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oa.521024.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zg.shtwfgs.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hp.9csxet.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hu.521024.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jp.bookmarksfly.cn

[L04] 设置超时
来源：http://bb.shxzskj.cn

Py:   requests.get(url, timeout=5)
来源：http://wj.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://om.9csxet.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pe.asd995.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dg.bjjhwx.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zw.shtwfgs.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zn.colortex.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pj.colortex.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ls.bookmarksfly.cn

[L05] 上传文件（multipart）
来源：http://xz.wgjwhj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ii.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://om.newstarts.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://of.bookmarksfly.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zc.yuntaijiaju.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://px.asd995.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yd.huanxung.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xl.nszjky.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jq.shxzskj.cn

[L06] 解析响应为 JSON
来源：http://qz.huixinmuqiang.cn

Py:   resp.json()
来源：http://yb.muxihuayi.cn

PHP:  json_decode($body, true);
来源：http://cm.szxytkj.cn

JS:   await resp.json()
来源：http://wt.shtwfgs.cn

TS:   await resp.json()
来源：http://rr.gzmigu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ob.newstarts.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yc.shtwfgs.cn

Ruby: JSON.parse(resp.body)
来源：http://rc.shxzskj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://og.jctech888.com.cn

[L07] 处理 HTTP 状态码
来源：http://bi.wgjwhj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wk.9csxet.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uo.gzmigu.cn

JS:   resp.ok;  resp.status
来源：http://wm.nicolike.cn

TS:   resp.ok;  resp.status
来源：http://do.nicolike.cn

Java: resp.statusCode()
来源：http://hq.panjiajie.cn

Go:   resp.StatusCode
来源：http://il.521024.cn

Ruby: resp.code.to_i
来源：http://gr.hnjuh.cn

C#:   (int)resp.StatusCode
来源：http://xl.chemitech.net.cn

[L08] 并发请求多个地址
来源：http://hv.yuexingan06.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ni.nszjky.cn

PHP:  curl_multi_init() 系列
来源：http://vc.9csxet.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jy.asd995.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ug.huixinmuqiang.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lr.yuexingan06.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xu.szsharing.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://va.yuntaijiaju.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ia.szxytkj.cn

================================================================================
来源：http://sk.newstarts.cn

M. 命令行 / 进程 / 环境
来源：http://ah.szxytkj.cn

================================================================================
来源：http://gk.bookmarksfly.cn

[M01] 读取命令行参数
来源：http://nl.bookmarksfly.cn

Py:   sys.argv[1:]
来源：http://lr.bjjhwx.cn

PHP:  $argv;  $argc;
来源：http://sx.asd995.cn

JS:   process.argv.slice(2)
来源：http://cj.yuntaijiaju.cn

TS:   process.argv.slice(2)
来源：http://oa.nszjky.cn

Java: args 数组（main 方法参数）
来源：http://hi.shxzskj.cn

Go:   os.Args[1:]
来源：http://xc.bjjhwx.cn

Ruby: ARGV
来源：http://lz.shxzskj.cn

C#:   args 数组（Main 方法参数）
来源：http://lv.yuntaijiaju.cn

[M02] 读取环境变量
来源：http://lm.shxzskj.cn

Py:   os.environ.get("HOME")
来源：http://bc.huanxung.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lz.lnxyls.cn

JS:   process.env.HOME
来源：http://jz.huixinmuqiang.cn

TS:   process.env.HOME
来源：http://kf.yuntaijiaju.cn

Java: System.getenv("HOME")
来源：http://qa.chemitech.net.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://th.huixiangedu.cn

Ruby: ENV["HOME"]
来源：http://lm.huanxung.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ou.bjjhwx.cn

[M03] 执行外部命令
来源：http://ec.haigaiapp.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ci.hahajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ac.colortex.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://rd.huixiangedu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zn.shtwfgs.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rw.9csxet.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ba.muxihuayi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ng.bjjhwx.cn

C#:   Process.Start("ls", "-l");
来源：http://ju.hnjuh.cn

[M04] 获取当前工作目录
来源：http://sm.chemitech.net.cn

Py:   os.getcwd()
来源：http://sh.shtwfgs.cn

PHP:  getcwd();
来源：http://bw.yuexingan06.cn

JS:   process.cwd()
来源：http://sh.huixinmuqiang.cn

TS:   process.cwd()
来源：http://cv.9csxet.cn

Java: Path.of("").toAbsolutePath()
来源：http://ar.shtwfgs.cn

Go:   os.Getwd()
来源：http://hg.lnxyls.cn

Ruby: Dir.pwd
来源：http://py.shtwfgs.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mi.huixinmuqiang.cn

[M05] 设置退出码
来源：http://fg.colortex.cn

Py:   sys.exit(1)
来源：http://vk.newstarts.cn

PHP:  exit(1);
来源：http://rv.haigaiapp.cn

JS:   process.exit(1)
来源：http://tc.shtwfgs.cn

TS:   process.exit(1)
来源：http://xx.lnxyls.cn

Java: System.exit(1)
来源：http://ew.nszjky.cn

Go:   os.Exit(1)
来源：http://dj.huixinmuqiang.cn

Ruby: exit 1
来源：http://ag.nszjky.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nj.panjiajie.cn

[M06] 向标准错误输出
来源：http://ij.asd995.cn

Py:   print("err", file=sys.stderr)
来源：http://ob.nicolike.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vz.haigaiapp.cn

JS:   console.error("err")
来源：http://ic.shtwfgs.cn

TS:   console.error("err")
来源：http://hx.newstarts.cn

Java: System.err.println("err")
来源：http://fd.szxytkj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nd.colortex.cn

Ruby: warn "err"
来源：http://od.szxytkj.cn

C#:   Console.Error.WriteLine("err")
来源：http://vy.szsharing.cn

[M07] 判断是否为主入口
来源：http://nc.hnjuh.cn

Py:   if __name__ == "__main__":
来源：http://tr.hnjuh.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://te.muxihuayi.cn

JS:   require.main === module
来源：http://ja.szxytkj.cn

TS:   require.main === module
来源：http://te.shxzukj.cn

Java: public static void main(String[] args)
来源：http://ma.newstarts.cn

Go:   func main()
来源：http://oj.newstarts.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xj.nszjky.cn

C#:   static void Main(string[] args)
来源：http://rf.bookmarksfly.cn


<!-- 参考信息 -->