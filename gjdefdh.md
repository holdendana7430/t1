代发 wailian999

Go:   time.Now()
来源：http://mm.wgjwhj.cn

Ruby: Time.now
来源：http://ff.nicolike.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pf.shtwfgs.cn

[J02] 格式化输出
来源：http://ex.bjjhwx.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ai.huixinmuqiang.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jb.gzmigu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uj.hahajie.cn

TS:   d.toISOString()
来源：http://di.bookmarksfly.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ko.newstarts.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lp.wgjwhj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hs.haigaiapp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cw.szxytkj.cn

[J03] 字符串解析为日期
来源：http://bp.bookmarksfly.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dd.9csxet.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nl.nicolike.cn

JS:   new Date("2024-01-02")
来源：http://bl.nszjky.cn

TS:   new Date("2024-01-02")
来源：http://qw.shxzskj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ao.lnxyls.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://il.9csxet.cn

Ruby: Date.parse("2024-01-02")
来源：http://ft.asd995.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hv.gzmigu.cn

[J04] 时间戳与日期互转
来源：http://dd.shtwfgs.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fh.haigaiapp.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://of.newstarts.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cr.haigaiapp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://sd.jctech888.com.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ad.yuntaijiaju.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tu.colortex.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zy.szxytkj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lo.bookmarksfly.cn

[J05] 时间加减（加 7 天）
来源：http://zf.nicolike.cn

Py:   now + timedelta(days=7)
来源：http://ve.shtwfgs.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://eq.colortex.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dq.newstarts.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ik.nicolike.cn

Java: LocalDate.now().plusDays(7)
来源：http://ib.nszjky.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gh.panjiajie.cn

Ruby: Time.now + 7 * 86400
来源：http://vx.gzmigu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://lb.chemitech.net.cn

[J06] 计算两时间之差
来源：http://zm.panjiajie.cn

Py:   (end - start).total_seconds()
来源：http://gs.huixiangedu.cn

PHP:  $end->diff($start)->days;
来源：http://em.panjiajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ae.bjjhwx.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lt.shxzukj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ux.hnjuh.cn

Go:   end.Sub(start).Hours()
来源：http://do.shxzukj.cn

Ruby: end - start                 # 返回秒数
来源：http://hw.9csxet.cn

C#:   (end - start).TotalSeconds
来源：http://jd.bjjhwx.cn

[J07] 比较两个日期
来源：http://cz.bjjhwx.cn

Py:   d1 < d2;  d1 == d2
来源：http://xm.yuntaijiaju.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ap.yuexingan06.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ub.gzmigu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://st.szxytkj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gi.muxihuayi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dq.newstarts.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fk.nicolike.cn

C#:   d1 < d2;  d1 == d2
来源：http://sr.huixinmuqiang.cn

[J08] 提取年月日与星期
来源：http://yq.lnxyls.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dq.yuexingan06.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gs.chemitech.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ks.9csxet.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hi.lnxyls.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://is.lnxyls.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qa.yuexingan06.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rf.newstarts.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zk.szxytkj.cn

[J09] 时区处理
来源：http://zm.panjiajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qq.nszjky.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gm.shxzskj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zb.colortex.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rc.colortex.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lc.szxytkj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bj.521024.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fp.szsharing.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ip.huanxung.cn

[J10] 取今天 / 本月第一天
来源：http://eu.newstarts.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vj.jianghongdianzi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://av.wgjwhj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yz.nszjky.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dq.hnjuh.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ek.shxzskj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dc.szxytkj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://og.hnjuh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qq.jctech888.com.cn

================================================================================
来源：http://cv.szxytkj.cn

K. JSON 与序列化
来源：http://pn.shxzukj.cn

================================================================================
来源：http://xy.9csxet.cn

[K01] 对象转 JSON 字符串
来源：http://kf.huixinmuqiang.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vt.muxihuayi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yh.szxytkj.cn

JS:   JSON.stringify(obj)
来源：http://pc.colortex.cn

TS:   JSON.stringify(obj)
来源：http://gz.hnjuh.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wm.yuexingan06.cn

Go:   json.Marshal(obj)
来源：http://lc.huixiangedu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mw.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://as.lnxyls.cn

[K02] JSON 字符串转对象
来源：http://yr.9csxet.cn

Py:   json.loads(s)
来源：http://fw.bjjhwx.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gs.szxytkj.cn

JS:   JSON.parse(s)
来源：http://dx.huanxung.cn

TS:   JSON.parse(s)
来源：http://cm.9csxet.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://br.shxzskj.cn

Go:   json.Unmarshal(data, &v)
来源：http://uh.nszjky.cn

Ruby: JSON.parse(s)
来源：http://ss.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vj.yuntaijiaju.cn

[K03] JSON 美化输出（带缩进）
来源：http://zj.shxzskj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nj.shxzskj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dm.nszjky.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vx.szsharing.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qb.shtwfgs.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ao.colortex.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pe.gzmigu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dh.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ui.muxihuayi.cn

[K04] 读取 JSON 文件
来源：http://on.yuntaijiaju.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jn.yuexingan06.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zy.hahajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://le.wgjwhj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kf.huixinmuqiang.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://db.521024.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://es.muxihuayi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ky.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qv.huixiangedu.cn

[K05] 深拷贝对象
来源：http://sf.panjiajie.cn

Py:   copy.deepcopy(obj)
来源：http://nk.huixiangedu.cn

PHP:  unserialize(serialize($obj));
来源：http://fq.szsharing.cn

JS:   structuredClone(obj)
来源：http://zv.yuexingan06.cn

TS:   structuredClone(obj)
来源：http://rt.jianghongdianzi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://lq.bjjhwx.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gu.haigaiapp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rs.huixiangedu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://nj.shxzukj.cn

[K06] 解析 URL 查询串
来源：http://os.shtwfgs.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ap.nicolike.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mg.bjjhwx.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jx.huanxung.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ce.521024.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ou.521024.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://uy.chemitech.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uk.gzmigu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zk.colortex.cn

[K07] 进制转换
来源：http://ez.hnjuh.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kk.shxzukj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lh.nszjky.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fi.yuexingan06.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ln.muxihuayi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qp.huanxung.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://aj.huanxung.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://an.huanxung.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://oz.bjjhwx.cn

[K08] 二进制序列化（非 JSON）
来源：http://kn.huixiangedu.cn

Py:   pickle.dumps(obj)
来源：http://sf.muxihuayi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://rn.lnxyls.cn

JS:   v8.serialize(obj)        // Node
来源：http://dz.newstarts.cn

TS:   v8.serialize(obj)        // Node
来源：http://uw.9csxet.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gn.jctech888.com.cn

Go:   encoding/gob
来源：http://qb.huixinmuqiang.cn

Ruby: Marshal.dump(obj)
来源：http://ob.jianghongdianzi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ws.szsharing.cn

================================================================================
来源：http://hy.lnxyls.cn

L. 网络请求
来源：http://jt.yuexingan06.cn

================================================================================
来源：http://kq.9csxet.cn

[L01] 发送 GET 请求
来源：http://ny.panjiajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rq.yuexingan06.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://la.shxzskj.cn

JS:   await fetch(url)
来源：http://ku.521024.cn

TS:   await fetch(url)
来源：http://an.shtwfgs.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pe.shxzskj.cn

Go:   resp, err := http.Get(url)
来源：http://dn.bjjhwx.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://td.shxzskj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kr.wgjwhj.cn

[L02] 发送 POST JSON
来源：http://es.huixinmuqiang.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qh.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ey.newstarts.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pa.haigaiapp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vq.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ha.muxihuayi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ky.bjjhwx.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nt.colortex.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gr.shxzukj.cn

[L03] 设置自定义请求头
来源：http://rs.huixiangedu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ov.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nd.panjiajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ho.yuntaijiaju.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://el.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zn.jctech888.com.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ov.yuexingan06.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bl.panjiajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jh.szxytkj.cn

[L04] 设置超时
来源：http://uy.huixinmuqiang.cn

Py:   requests.get(url, timeout=5)
来源：http://mj.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lw.jianghongdianzi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ox.hnjuh.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eq.hahajie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ce.yuntaijiaju.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qc.muxihuayi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gk.haigaiapp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wp.yuexingan06.cn

[L05] 上传文件（multipart）
来源：http://bt.yuexingan06.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tz.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tl.nszjky.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qy.gzmigu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ev.nicolike.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://iu.bjjhwx.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qv.gzmigu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gh.haigaiapp.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uc.shxzukj.cn

[L06] 解析响应为 JSON
来源：http://gf.yuexingan06.cn

Py:   resp.json()
来源：http://mc.huixinmuqiang.cn

PHP:  json_decode($body, true);
来源：http://se.huixiangedu.cn

JS:   await resp.json()
来源：http://ah.shtwfgs.cn

TS:   await resp.json()
来源：http://df.huixinmuqiang.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dc.colortex.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fk.yuntaijiaju.cn

Ruby: JSON.parse(resp.body)
来源：http://hq.wgjwhj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tt.hnjuh.cn

[L07] 处理 HTTP 状态码
来源：http://tz.bookmarksfly.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ig.panjiajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://iq.nicolike.cn

JS:   resp.ok;  resp.status
来源：http://cu.szxytkj.cn

TS:   resp.ok;  resp.status
来源：http://jb.panjiajie.cn

Java: resp.statusCode()
来源：http://bb.szxytkj.cn

Go:   resp.StatusCode
来源：http://tu.muxihuayi.cn

Ruby: resp.code.to_i
来源：http://wt.colortex.cn

C#:   (int)resp.StatusCode
来源：http://tz.jctech888.com.cn

[L08] 并发请求多个地址
来源：http://uz.panjiajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mm.yuntaijiaju.cn

PHP:  curl_multi_init() 系列
来源：http://lm.panjiajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://do.szxytkj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nszjky.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xe.haigaiapp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hu.bjjhwx.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bx.shxzukj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ir.haigaiapp.cn

================================================================================
来源：http://kn.lnxyls.cn

M. 命令行 / 进程 / 环境
来源：http://nn.gzmigu.cn

================================================================================
来源：http://nl.shxzskj.cn

[M01] 读取命令行参数
来源：http://yv.9csxet.cn

Py:   sys.argv[1:]
来源：http://mj.hnjuh.cn

PHP:  $argv;  $argc;
来源：http://dr.lnxyls.cn

JS:   process.argv.slice(2)
来源：http://wu.lnxyls.cn

TS:   process.argv.slice(2)
来源：http://fe.chemitech.net.cn

Java: args 数组（main 方法参数）
来源：http://px.yuntaijiaju.cn

Go:   os.Args[1:]
来源：http://gr.bookmarksfly.cn

Ruby: ARGV
来源：http://sl.9csxet.cn

C#:   args 数组（Main 方法参数）
来源：http://dl.huixinmuqiang.cn

[M02] 读取环境变量
来源：http://op.yuntaijiaju.cn

Py:   os.environ.get("HOME")
来源：http://ya.asd995.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hu.yuntaijiaju.cn

JS:   process.env.HOME
来源：http://ui.szsharing.cn

TS:   process.env.HOME
来源：http://af.hahajie.cn

Java: System.getenv("HOME")
来源：http://at.shxzskj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dl.yuexingan06.cn

Ruby: ENV["HOME"]
来源：http://mf.hahajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xq.shtwfgs.cn

[M03] 执行外部命令
来源：http://hr.shxzukj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://az.nszjky.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jr.hahajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nn.shxzukj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://eg.yuexingan06.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ho.hahajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://js.yuntaijiaju.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xx.jctech888.com.cn

C#:   Process.Start("ls", "-l");
来源：http://nq.hahajie.cn

[M04] 获取当前工作目录
来源：http://nm.nszjky.cn

Py:   os.getcwd()
来源：http://lj.shxzukj.cn

PHP:  getcwd();
来源：http://ku.asd995.cn

JS:   process.cwd()
来源：http://ec.hahajie.cn

TS:   process.cwd()
来源：http://ws.yuntaijiaju.cn

Java: Path.of("").toAbsolutePath()
来源：http://tm.9csxet.cn

Go:   os.Getwd()
来源：http://fy.bookmarksfly.cn

Ruby: Dir.pwd
来源：http://hg.jctech888.com.cn

C#:   Directory.GetCurrentDirectory()
来源：http://kq.9csxet.cn

[M05] 设置退出码
来源：http://px.jctech888.com.cn

Py:   sys.exit(1)
来源：http://xz.jianghongdianzi.cn

PHP:  exit(1);
来源：http://sw.gzmigu.cn

JS:   process.exit(1)
来源：http://hk.yuntaijiaju.cn

TS:   process.exit(1)
来源：http://tu.newstarts.cn

Java: System.exit(1)
来源：http://aq.chemitech.net.cn

Go:   os.Exit(1)
来源：http://ch.muxihuayi.cn

Ruby: exit 1
来源：http://vr.nszjky.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ba.gzmigu.cn

[M06] 向标准错误输出
来源：http://um.lnxyls.cn

Py:   print("err", file=sys.stderr)
来源：http://fn.haigaiapp.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xi.wgjwhj.cn

JS:   console.error("err")
来源：http://if.shxzukj.cn

TS:   console.error("err")
来源：http://fr.colortex.cn

Java: System.err.println("err")
来源：http://rm.shxzukj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ra.hahajie.cn

Ruby: warn "err"
来源：http://qn.huixinmuqiang.cn

C#:   Console.Error.WriteLine("err")
来源：http://pp.huixiangedu.cn

[M07] 判断是否为主入口
来源：http://ha.bookmarksfly.cn

Py:   if __name__ == "__main__":
来源：http://ve.bookmarksfly.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dt.nszjky.cn

JS:   require.main === module
来源：http://cq.jctech888.com.cn

TS:   require.main === module
来源：http://jp.9csxet.cn

Java: public static void main(String[] args)
来源：http://yl.huixinmuqiang.cn

Go:   func main()
来源：http://sp.nszjky.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://la.jctech888.com.cn

C#:   static void Main(string[] args)
来源：http://tr.shtwfgs.cn


<!-- 参考信息 -->