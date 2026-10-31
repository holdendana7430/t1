代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wg.jctech888.com.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qi.jctech888.com.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wl.szxytkj.cn

TS:   d.toISOString()
来源：http://wr.jctech888.com.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ss.lnxyls.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bv.huixiangedu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://an.jianghongdianzi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ic.huixiangedu.cn

[J03] 字符串解析为日期
来源：http://ib.newstarts.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://io.wgjwhj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pe.newstarts.cn

JS:   new Date("2024-01-02")
来源：http://mc.huixiangedu.cn

TS:   new Date("2024-01-02")
来源：http://px.9csxet.cn

Java: LocalDate.parse("2024-01-02")
来源：http://uu.asd995.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yk.gzmigu.cn

Ruby: Date.parse("2024-01-02")
来源：http://ia.szxytkj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ym.panjiajie.cn

[J04] 时间戳与日期互转
来源：http://zf.panjiajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sh.panjiajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sy.panjiajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nb.bookmarksfly.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xi.huixiangedu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ms.hahajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bt.yuexingan06.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nm.panjiajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gs.yuexingan06.cn

[J05] 时间加减（加 7 天）
来源：http://om.szsharing.cn

Py:   now + timedelta(days=7)
来源：http://au.9csxet.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ir.bookmarksfly.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xo.hnjuh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qa.jianghongdianzi.cn

Java: LocalDate.now().plusDays(7)
来源：http://bi.chemitech.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pk.wgjwhj.cn

Ruby: Time.now + 7 * 86400
来源：http://gq.huixinmuqiang.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ux.nicolike.cn

[J06] 计算两时间之差
来源：http://ct.shxzskj.cn

Py:   (end - start).total_seconds()
来源：http://nx.nicolike.cn

PHP:  $end->diff($start)->days;
来源：http://el.521024.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pk.shxzskj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wi.bookmarksfly.cn

Java: Duration.between(start, end).toSeconds()
来源：http://nn.shxzukj.cn

Go:   end.Sub(start).Hours()
来源：http://ih.521024.cn

Ruby: end - start                 # 返回秒数
来源：http://kq.szxytkj.cn

C#:   (end - start).TotalSeconds
来源：http://wq.bookmarksfly.cn

[J07] 比较两个日期
来源：http://co.bookmarksfly.cn

Py:   d1 < d2;  d1 == d2
来源：http://fm.huixiangedu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uq.szxytkj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gr.szxytkj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hy.panjiajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gl.gzmigu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ol.wgjwhj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wz.haigaiapp.cn

C#:   d1 < d2;  d1 == d2
来源：http://it.nicolike.cn

[J08] 提取年月日与星期
来源：http://sc.wgjwhj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tg.gzmigu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cf.panjiajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ak.hahajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wb.asd995.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bo.newstarts.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ua.hnjuh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://up.panjiajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://aa.9csxet.cn

[J09] 时区处理
来源：http://tx.huixiangedu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vl.gzmigu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tg.huanxung.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rg.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zv.asd995.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://em.hnjuh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dt.asd995.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://kh.panjiajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zx.lnxyls.cn

[J10] 取今天 / 本月第一天
来源：http://zi.nicolike.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vo.szsharing.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jf.nicolike.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ms.panjiajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nl.huixiangedu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hc.gzmigu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gu.nszjky.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pu.huixiangedu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vx.yuntaijiaju.cn

================================================================================
来源：http://up.bjjhwx.cn

K. JSON 与序列化
来源：http://ol.huixiangedu.cn

================================================================================
来源：http://cs.muxihuayi.cn

[K01] 对象转 JSON 字符串
来源：http://xx.shxzskj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wa.wgjwhj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rm.muxihuayi.cn

JS:   JSON.stringify(obj)
来源：http://es.yuntaijiaju.cn

TS:   JSON.stringify(obj)
来源：http://gk.shxzskj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gw.9csxet.cn

Go:   json.Marshal(obj)
来源：http://hf.colortex.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wo.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://nz.muxihuayi.cn

[K02] JSON 字符串转对象
来源：http://ge.bjjhwx.cn

Py:   json.loads(s)
来源：http://gm.lnxyls.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lv.chemitech.net.cn

JS:   JSON.parse(s)
来源：http://qv.521024.cn

TS:   JSON.parse(s)
来源：http://pj.chemitech.net.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://df.jctech888.com.cn

Go:   json.Unmarshal(data, &v)
来源：http://zg.chemitech.net.cn

Ruby: JSON.parse(s)
来源：http://zi.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ph.haigaiapp.cn

[K03] JSON 美化输出（带缩进）
来源：http://pj.colortex.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xa.shxzskj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ja.haigaiapp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://sq.wgjwhj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cc.asd995.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pi.jctech888.com.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pc.chemitech.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://sl.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mq.asd995.cn

[K04] 读取 JSON 文件
来源：http://su.szxytkj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gz.huixiangedu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kf.wgjwhj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dv.szsharing.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hq.9csxet.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ym.szxytkj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nh.bjjhwx.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ik.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://il.huixiangedu.cn

[K05] 深拷贝对象
来源：http://ez.newstarts.cn

Py:   copy.deepcopy(obj)
来源：http://et.newstarts.cn

PHP:  unserialize(serialize($obj));
来源：http://uy.huixiangedu.cn

JS:   structuredClone(obj)
来源：http://ml.nszjky.cn

TS:   structuredClone(obj)
来源：http://hu.bookmarksfly.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jv.shxzukj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lj.panjiajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ru.hahajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wt.yuntaijiaju.cn

[K06] 解析 URL 查询串
来源：http://ia.shxzukj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jn.jctech888.com.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gf.asd995.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rg.bjjhwx.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hh.panjiajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yx.shxzukj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gr.yuntaijiaju.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ox.huixinmuqiang.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://oj.jctech888.com.cn

[K07] 进制转换
来源：http://wd.szxytkj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ej.huixiangedu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://at.jianghongdianzi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ui.haigaiapp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fd.jianghongdianzi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pj.colortex.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qm.hahajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qr.shtwfgs.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hd.haigaiapp.cn

[K08] 二进制序列化（非 JSON）
来源：http://xs.haigaiapp.cn

Py:   pickle.dumps(obj)
来源：http://gf.muxihuayi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ga.hahajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://hs.bjjhwx.cn

TS:   v8.serialize(obj)        // Node
来源：http://jm.asd995.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ov.chemitech.net.cn

Go:   encoding/gob
来源：http://wl.nicolike.cn

Ruby: Marshal.dump(obj)
来源：http://wy.nszjky.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://po.panjiajie.cn

================================================================================
来源：http://vv.szsharing.cn

L. 网络请求
来源：http://bk.newstarts.cn

================================================================================
来源：http://qz.huixinmuqiang.cn

[L01] 发送 GET 请求
来源：http://lq.huixiangedu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pb.huixiangedu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ee.yuntaijiaju.cn

JS:   await fetch(url)
来源：http://li.jianghongdianzi.cn

TS:   await fetch(url)
来源：http://bs.nicolike.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://me.szsharing.cn

Go:   resp, err := http.Get(url)
来源：http://eu.bjjhwx.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ma.lnxyls.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ac.muxihuayi.cn

[L02] 发送 POST JSON
来源：http://uk.jianghongdianzi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://yb.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ec.jianghongdianzi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nw.szxytkj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ee.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zo.lnxyls.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xf.colortex.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kv.nicolike.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vt.szxytkj.cn

[L03] 设置自定义请求头
来源：http://qb.jianghongdianzi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wz.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://so.jianghongdianzi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zq.jctech888.com.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vq.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vh.asd995.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ai.hahajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fn.muxihuayi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://da.panjiajie.cn

[L04] 设置超时
来源：http://wz.521024.cn

Py:   requests.get(url, timeout=5)
来源：http://uk.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zu.lnxyls.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wb.colortex.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://im.asd995.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xq.haigaiapp.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tt.huixiangedu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gn.shxzukj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rk.yuexingan06.cn

[L05] 上传文件（multipart）
来源：http://jw.shxzukj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zz.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yd.haigaiapp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zi.panjiajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fp.hahajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mt.huanxung.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://td.huixinmuqiang.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cz.nszjky.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fj.szsharing.cn

[L06] 解析响应为 JSON
来源：http://sf.szsharing.cn

Py:   resp.json()
来源：http://hn.szxytkj.cn

PHP:  json_decode($body, true);
来源：http://bc.shxzskj.cn

JS:   await resp.json()
来源：http://ku.gzmigu.cn

TS:   await resp.json()
来源：http://yy.lnxyls.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tt.szsharing.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ux.haigaiapp.cn

Ruby: JSON.parse(resp.body)
来源：http://gj.chemitech.net.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uz.muxihuayi.cn

[L07] 处理 HTTP 状态码
来源：http://jm.jianghongdianzi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://je.chemitech.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xj.shtwfgs.cn

JS:   resp.ok;  resp.status
来源：http://uu.asd995.cn

TS:   resp.ok;  resp.status
来源：http://rx.panjiajie.cn

Java: resp.statusCode()
来源：http://xp.bookmarksfly.cn

Go:   resp.StatusCode
来源：http://rz.jctech888.com.cn

Ruby: resp.code.to_i
来源：http://wi.huanxung.cn

C#:   (int)resp.StatusCode
来源：http://vg.chemitech.net.cn

[L08] 并发请求多个地址
来源：http://qm.jianghongdianzi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sj.shxzukj.cn

PHP:  curl_multi_init() 系列
来源：http://mg.huixiangedu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sy.shxzukj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cc.jctech888.com.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tl.muxihuayi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://us.yuntaijiaju.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ov.jctech888.com.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sr.shtwfgs.cn

================================================================================
来源：http://to.huixinmuqiang.cn

M. 命令行 / 进程 / 环境
来源：http://bv.gzmigu.cn

================================================================================
来源：http://va.muxihuayi.cn

[M01] 读取命令行参数
来源：http://ec.szxytkj.cn

Py:   sys.argv[1:]
来源：http://qc.nicolike.cn

PHP:  $argv;  $argc;
来源：http://ue.shxzukj.cn

JS:   process.argv.slice(2)
来源：http://eo.muxihuayi.cn

TS:   process.argv.slice(2)
来源：http://bm.szxytkj.cn

Java: args 数组（main 方法参数）
来源：http://ao.yuntaijiaju.cn

Go:   os.Args[1:]
来源：http://mp.wgjwhj.cn

Ruby: ARGV
来源：http://xy.huixinmuqiang.cn

C#:   args 数组（Main 方法参数）
来源：http://co.yuntaijiaju.cn

[M02] 读取环境变量
来源：http://xs.muxihuayi.cn

Py:   os.environ.get("HOME")
来源：http://dh.panjiajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://na.panjiajie.cn

JS:   process.env.HOME
来源：http://qq.521024.cn

TS:   process.env.HOME
来源：http://lx.asd995.cn

Java: System.getenv("HOME")
来源：http://rx.shxzskj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xy.shxzukj.cn

Ruby: ENV["HOME"]
来源：http://ve.bjjhwx.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bk.nicolike.cn

[M03] 执行外部命令
来源：http://qh.jctech888.com.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fq.yuntaijiaju.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://de.panjiajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gh.hahajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ok.gzmigu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bs.haigaiapp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://no.nszjky.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zp.yuexingan06.cn

C#:   Process.Start("ls", "-l");
来源：http://zu.hahajie.cn

[M04] 获取当前工作目录
来源：http://qa.muxihuayi.cn

Py:   os.getcwd()
来源：http://vu.asd995.cn

PHP:  getcwd();
来源：http://hp.huixiangedu.cn

JS:   process.cwd()
来源：http://jn.hahajie.cn

TS:   process.cwd()
来源：http://ku.szxytkj.cn

Java: Path.of("").toAbsolutePath()
来源：http://qq.yuntaijiaju.cn

Go:   os.Getwd()
来源：http://of.huanxung.cn

Ruby: Dir.pwd
来源：http://uf.newstarts.cn

C#:   Directory.GetCurrentDirectory()
来源：http://uc.muxihuayi.cn

[M05] 设置退出码
来源：http://to.jianghongdianzi.cn

Py:   sys.exit(1)
来源：http://ul.shxzukj.cn

PHP:  exit(1);
来源：http://hh.muxihuayi.cn

JS:   process.exit(1)
来源：http://ui.9csxet.cn

TS:   process.exit(1)
来源：http://mv.nicolike.cn

Java: System.exit(1)
来源：http://ij.nicolike.cn

Go:   os.Exit(1)
来源：http://jf.asd995.cn

Ruby: exit 1
来源：http://yi.panjiajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gl.huixiangedu.cn

[M06] 向标准错误输出
来源：http://sq.huixiangedu.cn

Py:   print("err", file=sys.stderr)
来源：http://uy.hahajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cj.newstarts.cn

JS:   console.error("err")
来源：http://or.shxzukj.cn

TS:   console.error("err")
来源：http://dx.shxzukj.cn

Java: System.err.println("err")
来源：http://il.asd995.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wh.wgjwhj.cn

Ruby: warn "err"
来源：http://mi.yuntaijiaju.cn

C#:   Console.Error.WriteLine("err")
来源：http://mn.shxzskj.cn

[M07] 判断是否为主入口
来源：http://vh.lnxyls.cn

Py:   if __name__ == "__main__":
来源：http://vz.yuexingan06.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yz.9csxet.cn

JS:   require.main === module
来源：http://rd.colortex.cn

TS:   require.main === module
来源：http://sn.521024.cn

Java: public static void main(String[] args)
来源：http://cr.muxihuayi.cn

Go:   func main()
来源：http://ew.yuexingan06.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sm.szxytkj.cn

C#:   static void Main(string[] args)
来源：http://ik.bookmarksfly.cn

[M08] 获取系统与运行时信息
来源：http://ok.9csxet.cn

Py:   platform.system();  platform.python_version()
来源：http://pm.wgjwhj.cn

PHP:  PHP_OS;  phpversion();
来源：http://iz.9csxet.cn

JS:   process.platform;  process.version
来源：http://sw.bookmarksfly.cn


<!-- 参考信息 -->