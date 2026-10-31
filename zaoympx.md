代发 wailian999

Go:   time.Now()
来源：http://mu.szxytkj.cn

Ruby: Time.now
来源：http://cj.hahajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ja.lnxyls.cn

[J02] 格式化输出
来源：http://ea.jianghongdianzi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eu.521024.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hj.huixiangedu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vx.shxzskj.cn

TS:   d.toISOString()
来源：http://fr.shtwfgs.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hh.nicolike.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gy.chemitech.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://la.szsharing.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ag.huanxung.cn

[J03] 字符串解析为日期
来源：http://ir.yuntaijiaju.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hq.9csxet.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pt.jctech888.com.cn

JS:   new Date("2024-01-02")
来源：http://bz.panjiajie.cn

TS:   new Date("2024-01-02")
来源：http://gi.jianghongdianzi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vv.chemitech.net.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lr.szsharing.cn

Ruby: Date.parse("2024-01-02")
来源：http://ux.jctech888.com.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hd.newstarts.cn

[J04] 时间戳与日期互转
来源：http://cm.szsharing.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yq.hnjuh.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://an.panjiajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://af.yuexingan06.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xq.hahajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sk.nszjky.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tc.asd995.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bj.huixinmuqiang.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lt.haigaiapp.cn

[J05] 时间加减（加 7 天）
来源：http://vj.muxihuayi.cn

Py:   now + timedelta(days=7)
来源：http://px.hahajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://na.huixiangedu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://um.shtwfgs.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ml.hnjuh.cn

Java: LocalDate.now().plusDays(7)
来源：http://hw.bjjhwx.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ft.hahajie.cn

Ruby: Time.now + 7 * 86400
来源：http://gg.szxytkj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pa.szxytkj.cn

[J06] 计算两时间之差
来源：http://yl.jctech888.com.cn

Py:   (end - start).total_seconds()
来源：http://ox.nicolike.cn

PHP:  $end->diff($start)->days;
来源：http://kl.9csxet.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uk.yuexingan06.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ln.szxytkj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zl.shxzukj.cn

Go:   end.Sub(start).Hours()
来源：http://yo.jianghongdianzi.cn

Ruby: end - start                 # 返回秒数
来源：http://og.muxihuayi.cn

C#:   (end - start).TotalSeconds
来源：http://et.521024.cn

[J07] 比较两个日期
来源：http://sp.bjjhwx.cn

Py:   d1 < d2;  d1 == d2
来源：http://zx.bjjhwx.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nc.haigaiapp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://uq.yuexingan06.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zk.nszjky.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dq.haigaiapp.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ia.colortex.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jq.521024.cn

C#:   d1 < d2;  d1 == d2
来源：http://mk.shtwfgs.cn

[J08] 提取年月日与星期
来源：http://bj.shtwfgs.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ni.shtwfgs.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tb.hnjuh.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fg.shxzukj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jn.yuntaijiaju.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zi.wgjwhj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lz.muxihuayi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pm.521024.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pp.gzmigu.cn

[J09] 时区处理
来源：http://xl.gzmigu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hg.haigaiapp.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ln.shxzskj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ec.hnjuh.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yg.jctech888.com.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://br.bjjhwx.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mx.huixiangedu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ur.521024.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bu.yuexingan06.cn

[J10] 取今天 / 本月第一天
来源：http://vg.521024.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ke.bookmarksfly.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://er.521024.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ol.asd995.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gj.muxihuayi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wm.chemitech.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pc.asd995.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vf.huanxung.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ml.lnxyls.cn

================================================================================
来源：http://le.huanxung.cn

K. JSON 与序列化
来源：http://ec.hahajie.cn

================================================================================
来源：http://uv.shtwfgs.cn

[K01] 对象转 JSON 字符串
来源：http://hi.colortex.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pv.jctech888.com.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bk.bookmarksfly.cn

JS:   JSON.stringify(obj)
来源：http://ch.nicolike.cn

TS:   JSON.stringify(obj)
来源：http://st.bookmarksfly.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://iw.wgjwhj.cn

Go:   json.Marshal(obj)
来源：http://vz.shxzukj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ae.szsharing.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yk.hahajie.cn

[K02] JSON 字符串转对象
来源：http://ge.panjiajie.cn

Py:   json.loads(s)
来源：http://us.huixiangedu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vf.szsharing.cn

JS:   JSON.parse(s)
来源：http://lc.szxytkj.cn

TS:   JSON.parse(s)
来源：http://bx.jctech888.com.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wn.hahajie.cn

Go:   json.Unmarshal(data, &v)
来源：http://so.shxzskj.cn

Ruby: JSON.parse(s)
来源：http://ub.asd995.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ch.szxytkj.cn

[K03] JSON 美化输出（带缩进）
来源：http://de.hahajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sr.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wm.haigaiapp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xt.jianghongdianzi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://df.shxzukj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xt.haigaiapp.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://eu.bookmarksfly.cn

Ruby: JSON.pretty_generate(obj)
来源：http://yi.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wc.szxytkj.cn

[K04] 读取 JSON 文件
来源：http://kl.huanxung.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kw.shtwfgs.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dg.haigaiapp.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fm.lnxyls.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tw.bookmarksfly.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mh.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ff.chemitech.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://li.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://so.szsharing.cn

[K05] 深拷贝对象
来源：http://bi.nicolike.cn

Py:   copy.deepcopy(obj)
来源：http://az.huixiangedu.cn

PHP:  unserialize(serialize($obj));
来源：http://rd.haigaiapp.cn

JS:   structuredClone(obj)
来源：http://pc.huixinmuqiang.cn

TS:   structuredClone(obj)
来源：http://sv.chemitech.net.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://md.hahajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gb.gzmigu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://et.newstarts.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yz.newstarts.cn

[K06] 解析 URL 查询串
来源：http://nb.lnxyls.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sj.lnxyls.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://he.lnxyls.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mk.hnjuh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mm.jctech888.com.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bo.hahajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qk.hnjuh.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vm.shxzskj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hg.521024.cn

[K07] 进制转换
来源：http://zl.shxzukj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rm.huanxung.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fn.nszjky.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nk.yuexingan06.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nf.huixinmuqiang.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mb.colortex.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pg.szxytkj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ar.muxihuayi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uc.hnjuh.cn

[K08] 二进制序列化（非 JSON）
来源：http://zc.huanxung.cn

Py:   pickle.dumps(obj)
来源：http://jb.gzmigu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ui.bookmarksfly.cn

JS:   v8.serialize(obj)        // Node
来源：http://go.haigaiapp.cn

TS:   v8.serialize(obj)        // Node
来源：http://bx.bookmarksfly.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://em.jianghongdianzi.cn

Go:   encoding/gob
来源：http://sf.huixinmuqiang.cn

Ruby: Marshal.dump(obj)
来源：http://ea.hahajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xg.asd995.cn

================================================================================
来源：http://jx.hahajie.cn

L. 网络请求
来源：http://iv.hnjuh.cn

================================================================================
来源：http://ta.bookmarksfly.cn

[L01] 发送 GET 请求
来源：http://mu.jianghongdianzi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://op.huixiangedu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cg.shxzukj.cn

JS:   await fetch(url)
来源：http://jy.jctech888.com.cn

TS:   await fetch(url)
来源：http://ea.nszjky.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tf.szxytkj.cn

Go:   resp, err := http.Get(url)
来源：http://hj.lnxyls.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://my.huixinmuqiang.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nv.hnjuh.cn

[L02] 发送 POST JSON
来源：http://nk.chemitech.net.cn

Py:   requests.post(url, json={"a": 1})
来源：http://sn.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zj.huanxung.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lk.colortex.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://le.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bv.shxzukj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nm.shxzskj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fb.asd995.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gr.chemitech.net.cn

[L03] 设置自定义请求头
来源：http://wa.haigaiapp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vw.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gn.lnxyls.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://us.yuexingan06.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lh.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gd.lnxyls.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vr.huixiangedu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xo.bookmarksfly.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://im.yuntaijiaju.cn

[L04] 设置超时
来源：http://rt.nszjky.cn

Py:   requests.get(url, timeout=5)
来源：http://bl.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ib.shxzukj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fj.nicolike.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ao.hnjuh.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vq.jianghongdianzi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hc.521024.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vh.nicolike.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lq.asd995.cn

[L05] 上传文件（multipart）
来源：http://og.bjjhwx.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ip.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xt.yuexingan06.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://br.wgjwhj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ti.huixiangedu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://av.yuntaijiaju.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fg.jctech888.com.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bx.yuntaijiaju.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xj.yuexingan06.cn

[L06] 解析响应为 JSON
来源：http://cp.yuntaijiaju.cn

Py:   resp.json()
来源：http://zc.szxytkj.cn

PHP:  json_decode($body, true);
来源：http://ro.nszjky.cn

JS:   await resp.json()
来源：http://cl.huixiangedu.cn

TS:   await resp.json()
来源：http://ba.panjiajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nw.wgjwhj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://no.newstarts.cn

Ruby: JSON.parse(resp.body)
来源：http://ld.9csxet.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jd.nicolike.cn

[L07] 处理 HTTP 状态码
来源：http://oo.asd995.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lh.panjiajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ov.hnjuh.cn

JS:   resp.ok;  resp.status
来源：http://ry.hnjuh.cn

TS:   resp.ok;  resp.status
来源：http://rs.wgjwhj.cn

Java: resp.statusCode()
来源：http://mv.bookmarksfly.cn

Go:   resp.StatusCode
来源：http://xu.haigaiapp.cn

Ruby: resp.code.to_i
来源：http://rp.yuexingan06.cn

C#:   (int)resp.StatusCode
来源：http://ry.nicolike.cn

[L08] 并发请求多个地址
来源：http://ih.colortex.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cr.yuntaijiaju.cn

PHP:  curl_multi_init() 系列
来源：http://sl.panjiajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gl.szsharing.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://um.shxzukj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rq.muxihuayi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xu.huixiangedu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://px.muxihuayi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sq.newstarts.cn

================================================================================
来源：http://wc.haigaiapp.cn

M. 命令行 / 进程 / 环境
来源：http://vk.521024.cn

================================================================================
来源：http://vv.szsharing.cn

[M01] 读取命令行参数
来源：http://in.yuexingan06.cn

Py:   sys.argv[1:]
来源：http://oq.chemitech.net.cn

PHP:  $argv;  $argc;
来源：http://hj.jctech888.com.cn

JS:   process.argv.slice(2)
来源：http://av.nicolike.cn

TS:   process.argv.slice(2)
来源：http://ra.szsharing.cn

Java: args 数组（main 方法参数）
来源：http://wv.huanxung.cn

Go:   os.Args[1:]
来源：http://vc.panjiajie.cn

Ruby: ARGV
来源：http://aq.shxzukj.cn

C#:   args 数组（Main 方法参数）
来源：http://mi.szsharing.cn

[M02] 读取环境变量
来源：http://rl.newstarts.cn

Py:   os.environ.get("HOME")
来源：http://ex.colortex.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tw.hnjuh.cn

JS:   process.env.HOME
来源：http://md.yuntaijiaju.cn

TS:   process.env.HOME
来源：http://nc.jianghongdianzi.cn

Java: System.getenv("HOME")
来源：http://zo.lnxyls.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jj.chemitech.net.cn

Ruby: ENV["HOME"]
来源：http://ii.panjiajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tw.nicolike.cn

[M03] 执行外部命令
来源：http://df.shtwfgs.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hw.shxzukj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xm.muxihuayi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gi.9csxet.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://bi.jianghongdianzi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mq.lnxyls.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fi.newstarts.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rr.gzmigu.cn

C#:   Process.Start("ls", "-l");
来源：http://yo.newstarts.cn

[M04] 获取当前工作目录
来源：http://be.521024.cn

Py:   os.getcwd()
来源：http://zr.shxzukj.cn

PHP:  getcwd();
来源：http://bo.bjjhwx.cn

JS:   process.cwd()
来源：http://kv.nicolike.cn

TS:   process.cwd()
来源：http://dy.szsharing.cn

Java: Path.of("").toAbsolutePath()
来源：http://tg.bookmarksfly.cn

Go:   os.Getwd()
来源：http://rv.jctech888.com.cn

Ruby: Dir.pwd
来源：http://dd.colortex.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ua.hnjuh.cn

[M05] 设置退出码
来源：http://sc.bjjhwx.cn

Py:   sys.exit(1)
来源：http://et.yuntaijiaju.cn

PHP:  exit(1);
来源：http://xi.jianghongdianzi.cn

JS:   process.exit(1)
来源：http://rp.shxzukj.cn

TS:   process.exit(1)
来源：http://kt.wgjwhj.cn

Java: System.exit(1)
来源：http://ci.bookmarksfly.cn

Go:   os.Exit(1)
来源：http://vd.muxihuayi.cn

Ruby: exit 1
来源：http://tj.hahajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ls.hahajie.cn

[M06] 向标准错误输出
来源：http://ex.lnxyls.cn

Py:   print("err", file=sys.stderr)
来源：http://hq.jianghongdianzi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ax.nicolike.cn

JS:   console.error("err")
来源：http://dz.chemitech.net.cn

TS:   console.error("err")
来源：http://bg.shtwfgs.cn

Java: System.err.println("err")
来源：http://vt.colortex.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ms.shxzskj.cn

Ruby: warn "err"
来源：http://vy.wgjwhj.cn

C#:   Console.Error.WriteLine("err")
来源：http://cq.colortex.cn

[M07] 判断是否为主入口
来源：http://go.panjiajie.cn

Py:   if __name__ == "__main__":
来源：http://xs.shtwfgs.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://it.szxytkj.cn

JS:   require.main === module
来源：http://wb.huixiangedu.cn

TS:   require.main === module
来源：http://hu.haigaiapp.cn

Java: public static void main(String[] args)
来源：http://mn.shtwfgs.cn

Go:   func main()
来源：http://eh.chemitech.net.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ze.lnxyls.cn

C#:   static void Main(string[] args)
来源：http://cc.panjiajie.cn


<!-- 参考信息 -->