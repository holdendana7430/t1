代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pz.bjjhwx.cn

JS:   new Date();  Date.now()
来源：http://sw.colortex.cn

TS:   new Date();  Date.now()
来源：http://qc.bjjhwx.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://xa.shxzukj.cn

Go:   time.Now()
来源：http://vm.hahajie.cn

Ruby: Time.now
来源：http://yx.bookmarksfly.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ks.shxzskj.cn

[J02] 格式化输出
来源：http://de.asd995.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fo.nszjky.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cb.521024.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vg.newstarts.cn

TS:   d.toISOString()
来源：http://az.muxihuayi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://re.shxzukj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qa.chemitech.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cl.shxzskj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ao.bjjhwx.cn

[J03] 字符串解析为日期
来源：http://yx.panjiajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vc.haigaiapp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://se.newstarts.cn

JS:   new Date("2024-01-02")
来源：http://pk.szxytkj.cn

TS:   new Date("2024-01-02")
来源：http://ar.huixinmuqiang.cn

Java: LocalDate.parse("2024-01-02")
来源：http://eg.chemitech.net.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ve.jctech888.com.cn

Ruby: Date.parse("2024-01-02")
来源：http://py.newstarts.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://af.muxihuayi.cn

[J04] 时间戳与日期互转
来源：http://bm.shxzskj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vl.szsharing.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ft.nicolike.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://np.nszjky.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://od.huanxung.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uc.huanxung.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rl.gzmigu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ed.bookmarksfly.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ck.muxihuayi.cn

[J05] 时间加减（加 7 天）
来源：http://ot.panjiajie.cn

Py:   now + timedelta(days=7)
来源：http://mk.wgjwhj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://dm.shtwfgs.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ij.huixinmuqiang.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yf.huixinmuqiang.cn

Java: LocalDate.now().plusDays(7)
来源：http://gk.chemitech.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nf.yuntaijiaju.cn

Ruby: Time.now + 7 * 86400
来源：http://gp.gzmigu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ob.yuexingan06.cn

[J06] 计算两时间之差
来源：http://xz.szxytkj.cn

Py:   (end - start).total_seconds()
来源：http://tg.szxytkj.cn

PHP:  $end->diff($start)->days;
来源：http://kt.haigaiapp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ho.szxytkj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kt.9csxet.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qv.jctech888.com.cn

Go:   end.Sub(start).Hours()
来源：http://qp.huanxung.cn

Ruby: end - start                 # 返回秒数
来源：http://ep.panjiajie.cn

C#:   (end - start).TotalSeconds
来源：http://bq.muxihuayi.cn

[J07] 比较两个日期
来源：http://qv.chemitech.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://cc.jianghongdianzi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ck.newstarts.cn

JS:   d1.getTime() < d2.getTime()
来源：http://cq.szsharing.cn

TS:   d1.getTime() < d2.getTime()
来源：http://sh.shxzskj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hh.colortex.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ao.szsharing.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mt.muxihuayi.cn

C#:   d1 < d2;  d1 == d2
来源：http://xw.shtwfgs.cn

[J08] 提取年月日与星期
来源：http://ia.muxihuayi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vy.muxihuayi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ue.yuexingan06.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ce.asd995.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ew.huixinmuqiang.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rq.asd995.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kg.nicolike.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ah.lnxyls.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ho.asd995.cn

[J09] 时区处理
来源：http://jb.shtwfgs.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bx.haigaiapp.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yd.jianghongdianzi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ro.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ri.gzmigu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yb.gzmigu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xb.yuexingan06.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vn.shxzskj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vt.jctech888.com.cn

[J10] 取今天 / 本月第一天
来源：http://ny.bookmarksfly.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zk.huixinmuqiang.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qv.muxihuayi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://br.panjiajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uo.huanxung.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dd.yuntaijiaju.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xa.bookmarksfly.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pa.muxihuayi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qo.chemitech.net.cn

================================================================================
来源：http://pp.haigaiapp.cn

K. JSON 与序列化
来源：http://ft.wgjwhj.cn

================================================================================
来源：http://nb.shxzskj.cn

[K01] 对象转 JSON 字符串
来源：http://wn.hnjuh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dm.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yh.521024.cn

JS:   JSON.stringify(obj)
来源：http://ti.szxytkj.cn

TS:   JSON.stringify(obj)
来源：http://rw.nicolike.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bx.9csxet.cn

Go:   json.Marshal(obj)
来源：http://zf.hahajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hm.szsharing.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vu.haigaiapp.cn

[K02] JSON 字符串转对象
来源：http://ot.521024.cn

Py:   json.loads(s)
来源：http://rr.szxytkj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vc.shtwfgs.cn

JS:   JSON.parse(s)
来源：http://lj.yuntaijiaju.cn

TS:   JSON.parse(s)
来源：http://eq.jctech888.com.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pt.9csxet.cn

Go:   json.Unmarshal(data, &v)
来源：http://lx.newstarts.cn

Ruby: JSON.parse(s)
来源：http://px.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dh.shxzukj.cn

[K03] JSON 美化输出（带缩进）
来源：http://hc.bookmarksfly.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fj.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://od.szsharing.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://af.yuexingan06.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://hp.colortex.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tr.hnjuh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cj.colortex.cn

Ruby: JSON.pretty_generate(obj)
来源：http://sl.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cv.hnjuh.cn

[K04] 读取 JSON 文件
来源：http://yr.asd995.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nv.colortex.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ju.wgjwhj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qk.nszjky.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dw.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gr.colortex.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pz.lnxyls.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://kj.asd995.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vv.szxytkj.cn

[K05] 深拷贝对象
来源：http://mj.panjiajie.cn

Py:   copy.deepcopy(obj)
来源：http://ix.shxzukj.cn

PHP:  unserialize(serialize($obj));
来源：http://tz.lnxyls.cn

JS:   structuredClone(obj)
来源：http://rt.yuexingan06.cn

TS:   structuredClone(obj)
来源：http://uh.hahajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kb.szsharing.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wp.jctech888.com.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ud.9csxet.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ju.muxihuayi.cn

[K06] 解析 URL 查询串
来源：http://pr.9csxet.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xz.panjiajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yt.yuexingan06.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wf.haigaiapp.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rm.jctech888.com.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cc.colortex.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vj.lnxyls.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uc.521024.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ie.muxihuayi.cn

[K07] 进制转换
来源：http://el.chemitech.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://at.yuexingan06.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cx.hahajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hh.huanxung.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ma.szsharing.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fx.szsharing.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nq.hnjuh.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://je.asd995.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://oo.huanxung.cn

[K08] 二进制序列化（非 JSON）
来源：http://mt.521024.cn

Py:   pickle.dumps(obj)
来源：http://bq.haigaiapp.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pv.chemitech.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://ke.haigaiapp.cn

TS:   v8.serialize(obj)        // Node
来源：http://bi.wgjwhj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hu.gzmigu.cn

Go:   encoding/gob
来源：http://sa.colortex.cn

Ruby: Marshal.dump(obj)
来源：http://ic.shtwfgs.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cb.newstarts.cn

================================================================================
来源：http://kc.nicolike.cn

L. 网络请求
来源：http://xa.haigaiapp.cn

================================================================================
来源：http://yt.yuexingan06.cn

[L01] 发送 GET 请求
来源：http://hq.muxihuayi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pg.nszjky.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ue.huixinmuqiang.cn

JS:   await fetch(url)
来源：http://yy.yuntaijiaju.cn

TS:   await fetch(url)
来源：http://is.bookmarksfly.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hk.gzmigu.cn

Go:   resp, err := http.Get(url)
来源：http://cb.lnxyls.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wc.newstarts.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ux.521024.cn

[L02] 发送 POST JSON
来源：http://eh.huixiangedu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ge.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vb.szxytkj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lb.521024.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://go.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sg.yuntaijiaju.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://se.huixinmuqiang.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tr.hnjuh.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rq.nicolike.cn

[L03] 设置自定义请求头
来源：http://ny.muxihuayi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kt.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xf.muxihuayi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ui.521024.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sk.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ub.szsharing.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yb.521024.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ya.jctech888.com.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nc.shxzskj.cn

[L04] 设置超时
来源：http://ca.yuexingan06.cn

Py:   requests.get(url, timeout=5)
来源：http://nn.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qg.asd995.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jx.huanxung.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ho.lnxyls.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yr.yuexingan06.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ra.lnxyls.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ng.yuexingan06.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qp.jianghongdianzi.cn

[L05] 上传文件（multipart）
来源：http://rw.lnxyls.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jz.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nu.hahajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ns.shtwfgs.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://it.huixiangedu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gu.jianghongdianzi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jw.bookmarksfly.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ne.yuntaijiaju.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fj.colortex.cn

[L06] 解析响应为 JSON
来源：http://mh.gzmigu.cn

Py:   resp.json()
来源：http://ar.gzmigu.cn

PHP:  json_decode($body, true);
来源：http://qw.shxzukj.cn

JS:   await resp.json()
来源：http://mi.chemitech.net.cn

TS:   await resp.json()
来源：http://ox.panjiajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ot.colortex.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ze.shxzskj.cn

Ruby: JSON.parse(resp.body)
来源：http://ga.muxihuayi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kj.huanxung.cn

[L07] 处理 HTTP 状态码
来源：http://zt.yuntaijiaju.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tz.bookmarksfly.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yv.bookmarksfly.cn

JS:   resp.ok;  resp.status
来源：http://ur.huixiangedu.cn

TS:   resp.ok;  resp.status
来源：http://jc.yuntaijiaju.cn

Java: resp.statusCode()
来源：http://to.newstarts.cn

Go:   resp.StatusCode
来源：http://ej.asd995.cn

Ruby: resp.code.to_i
来源：http://rn.lnxyls.cn

C#:   (int)resp.StatusCode
来源：http://fh.lnxyls.cn

[L08] 并发请求多个地址
来源：http://rx.hnjuh.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wn.huixiangedu.cn

PHP:  curl_multi_init() 系列
来源：http://sx.9csxet.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ju.yuntaijiaju.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ef.bookmarksfly.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://oc.newstarts.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kg.gzmigu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ov.shxzskj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ou.colortex.cn

================================================================================
来源：http://kw.hahajie.cn

M. 命令行 / 进程 / 环境
来源：http://fi.shxzukj.cn

================================================================================
来源：http://qv.szsharing.cn

[M01] 读取命令行参数
来源：http://uh.panjiajie.cn

Py:   sys.argv[1:]
来源：http://lb.shxzskj.cn

PHP:  $argv;  $argc;
来源：http://tv.szxytkj.cn

JS:   process.argv.slice(2)
来源：http://zp.bjjhwx.cn

TS:   process.argv.slice(2)
来源：http://td.hahajie.cn

Java: args 数组（main 方法参数）
来源：http://qx.newstarts.cn

Go:   os.Args[1:]
来源：http://iu.szxytkj.cn

Ruby: ARGV
来源：http://ev.yuntaijiaju.cn

C#:   args 数组（Main 方法参数）
来源：http://vo.jctech888.com.cn

[M02] 读取环境变量
来源：http://ew.huixiangedu.cn

Py:   os.environ.get("HOME")
来源：http://mp.nicolike.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://el.chemitech.net.cn

JS:   process.env.HOME
来源：http://zi.nszjky.cn

TS:   process.env.HOME
来源：http://or.asd995.cn

Java: System.getenv("HOME")
来源：http://hh.bjjhwx.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zd.haigaiapp.cn

Ruby: ENV["HOME"]
来源：http://cz.9csxet.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wu.szsharing.cn

[M03] 执行外部命令
来源：http://vg.szsharing.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dg.shtwfgs.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ci.9csxet.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xe.lnxyls.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ut.shtwfgs.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ca.huixinmuqiang.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mu.shxzukj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ni.jctech888.com.cn

C#:   Process.Start("ls", "-l");
来源：http://qd.muxihuayi.cn

[M04] 获取当前工作目录
来源：http://uw.nszjky.cn

Py:   os.getcwd()
来源：http://ez.lnxyls.cn

PHP:  getcwd();
来源：http://jb.521024.cn

JS:   process.cwd()
来源：http://xo.szxytkj.cn

TS:   process.cwd()
来源：http://tl.hnjuh.cn

Java: Path.of("").toAbsolutePath()
来源：http://qe.haigaiapp.cn

Go:   os.Getwd()
来源：http://lf.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://pp.jianghongdianzi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://pf.shxzukj.cn

[M05] 设置退出码
来源：http://pq.asd995.cn

Py:   sys.exit(1)
来源：http://um.szsharing.cn

PHP:  exit(1);
来源：http://bd.huixinmuqiang.cn

JS:   process.exit(1)
来源：http://up.hnjuh.cn

TS:   process.exit(1)
来源：http://wq.wgjwhj.cn

Java: System.exit(1)
来源：http://sy.szxytkj.cn

Go:   os.Exit(1)
来源：http://rv.shxzukj.cn

Ruby: exit 1
来源：http://kb.jianghongdianzi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zl.lnxyls.cn

[M06] 向标准错误输出
来源：http://bp.yuntaijiaju.cn

Py:   print("err", file=sys.stderr)
来源：http://ph.huixiangedu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ej.shxzskj.cn

JS:   console.error("err")
来源：http://xg.nicolike.cn

TS:   console.error("err")
来源：http://gs.521024.cn

Java: System.err.println("err")
来源：http://wn.nicolike.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xu.chemitech.net.cn

Ruby: warn "err"
来源：http://va.asd995.cn

C#:   Console.Error.WriteLine("err")
来源：http://yb.gzmigu.cn

[M07] 判断是否为主入口
来源：http://hf.bookmarksfly.cn

Py:   if __name__ == "__main__":
来源：http://vq.panjiajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bk.nicolike.cn

JS:   require.main === module
来源：http://kh.newstarts.cn

TS:   require.main === module
来源：http://rk.wgjwhj.cn


<!-- 参考信息 -->