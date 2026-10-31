代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://er.hnjuh.cn

JS:   new Date();  Date.now()
来源：http://wf.asd995.cn

TS:   new Date();  Date.now()
来源：http://qf.huixinmuqiang.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lb.gzmigu.cn

Go:   time.Now()
来源：http://my.gzmigu.cn

Ruby: Time.now
来源：http://ih.nicolike.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nz.jctech888.com.cn

[J02] 格式化输出
来源：http://yz.huanxung.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hs.shtwfgs.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://co.chemitech.net.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://je.shtwfgs.cn

TS:   d.toISOString()
来源：http://mq.bookmarksfly.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ho.shxzskj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qc.shxzskj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ev.bjjhwx.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://of.szxytkj.cn

[J03] 字符串解析为日期
来源：http://ph.shxzukj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dj.newstarts.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wj.wgjwhj.cn

JS:   new Date("2024-01-02")
来源：http://ec.chemitech.net.cn

TS:   new Date("2024-01-02")
来源：http://fa.hnjuh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qg.huanxung.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qt.nszjky.cn

Ruby: Date.parse("2024-01-02")
来源：http://gz.shxzskj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wq.haigaiapp.cn

[J04] 时间戳与日期互转
来源：http://pe.huixiangedu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ug.asd995.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://re.nicolike.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ac.huanxung.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cb.haigaiapp.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yo.bookmarksfly.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gu.chemitech.net.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qd.hahajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yw.huixinmuqiang.cn

[J05] 时间加减（加 7 天）
来源：http://xk.nicolike.cn

Py:   now + timedelta(days=7)
来源：http://zi.muxihuayi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ve.huixinmuqiang.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fn.muxihuayi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ns.yuexingan06.cn

Java: LocalDate.now().plusDays(7)
来源：http://fn.hnjuh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ie.shxzskj.cn

Ruby: Time.now + 7 * 86400
来源：http://uh.9csxet.cn

C#:   DateTime.Now.AddDays(7)
来源：http://od.asd995.cn

[J06] 计算两时间之差
来源：http://ex.521024.cn

Py:   (end - start).total_seconds()
来源：http://nl.huixiangedu.cn

PHP:  $end->diff($start)->days;
来源：http://ou.bjjhwx.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tf.jianghongdianzi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cu.haigaiapp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bw.shtwfgs.cn

Go:   end.Sub(start).Hours()
来源：http://ss.jianghongdianzi.cn

Ruby: end - start                 # 返回秒数
来源：http://lj.lnxyls.cn

C#:   (end - start).TotalSeconds
来源：http://ew.szxytkj.cn

[J07] 比较两个日期
来源：http://zo.shxzskj.cn

Py:   d1 < d2;  d1 == d2
来源：http://tg.hahajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://iv.haigaiapp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fo.huixiangedu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ka.nszjky.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ks.9csxet.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fm.colortex.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vf.jianghongdianzi.cn

C#:   d1 < d2;  d1 == d2
来源：http://yj.shxzukj.cn

[J08] 提取年月日与星期
来源：http://nu.521024.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bx.panjiajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nv.szxytkj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xc.shxzskj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://eq.nicolike.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lm.shtwfgs.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jv.huanxung.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sy.jianghongdianzi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tf.huixinmuqiang.cn

[J09] 时区处理
来源：http://cn.wgjwhj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lw.newstarts.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wf.shxzukj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ah.huanxung.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wi.jianghongdianzi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gx.521024.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nl.nicolike.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gb.521024.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uq.jianghongdianzi.cn

[J10] 取今天 / 本月第一天
来源：http://ms.huixinmuqiang.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zh.haigaiapp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wd.yuntaijiaju.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://va.gzmigu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pt.huixiangedu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cf.panjiajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ik.panjiajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xo.jctech888.com.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ar.9csxet.cn

================================================================================
来源：http://zy.shxzskj.cn

K. JSON 与序列化
来源：http://op.huixiangedu.cn

================================================================================
来源：http://ij.jianghongdianzi.cn

[K01] 对象转 JSON 字符串
来源：http://wk.wgjwhj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ka.szsharing.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cl.hnjuh.cn

JS:   JSON.stringify(obj)
来源：http://ga.jctech888.com.cn

TS:   JSON.stringify(obj)
来源：http://wr.hahajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bf.newstarts.cn

Go:   json.Marshal(obj)
来源：http://ig.szxytkj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ss.panjiajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vk.shtwfgs.cn

[K02] JSON 字符串转对象
来源：http://wb.szsharing.cn

Py:   json.loads(s)
来源：http://du.asd995.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kn.huixinmuqiang.cn

JS:   JSON.parse(s)
来源：http://kv.szxytkj.cn

TS:   JSON.parse(s)
来源：http://ml.nszjky.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zj.nszjky.cn

Go:   json.Unmarshal(data, &v)
来源：http://sw.gzmigu.cn

Ruby: JSON.parse(s)
来源：http://hk.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yy.haigaiapp.cn

[K03] JSON 美化输出（带缩进）
来源：http://lg.lnxyls.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://en.huixiangedu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dr.chemitech.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bw.shtwfgs.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gt.chemitech.net.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fh.shtwfgs.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vf.shxzukj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://se.nszjky.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wd.chemitech.net.cn

[K04] 读取 JSON 文件
来源：http://lq.muxihuayi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wg.shtwfgs.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iy.521024.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ux.shxzskj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ov.huixiangedu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pw.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wf.newstarts.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zg.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ik.colortex.cn

[K05] 深拷贝对象
来源：http://tr.colortex.cn

Py:   copy.deepcopy(obj)
来源：http://cp.hnjuh.cn

PHP:  unserialize(serialize($obj));
来源：http://ft.hahajie.cn

JS:   structuredClone(obj)
来源：http://ku.jctech888.com.cn

TS:   structuredClone(obj)
来源：http://nm.jianghongdianzi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://nk.szsharing.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kc.colortex.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vi.huanxung.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ru.hahajie.cn

[K06] 解析 URL 查询串
来源：http://fq.huixiangedu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://eg.colortex.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ur.hahajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zx.wgjwhj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sn.muxihuayi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://py.nszjky.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zb.asd995.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ne.huixiangedu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mr.shxzskj.cn

[K07] 进制转换
来源：http://ag.szxytkj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mw.jianghongdianzi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jl.colortex.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pw.nicolike.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fp.huixinmuqiang.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.bookmarksfly.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ce.wgjwhj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zr.bookmarksfly.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ah.huixinmuqiang.cn

[K08] 二进制序列化（非 JSON）
来源：http://tx.szsharing.cn

Py:   pickle.dumps(obj)
来源：http://li.shxzskj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dz.wgjwhj.cn

JS:   v8.serialize(obj)        // Node
来源：http://zg.yuexingan06.cn

TS:   v8.serialize(obj)        // Node
来源：http://tq.szxytkj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zp.521024.cn

Go:   encoding/gob
来源：http://vk.newstarts.cn

Ruby: Marshal.dump(obj)
来源：http://hq.yuntaijiaju.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pj.asd995.cn

================================================================================
来源：http://ac.shxzukj.cn

L. 网络请求
来源：http://to.newstarts.cn

================================================================================
来源：http://pr.szsharing.cn

[L01] 发送 GET 请求
来源：http://rc.huixiangedu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bh.huixinmuqiang.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://as.yuntaijiaju.cn

JS:   await fetch(url)
来源：http://rh.521024.cn

TS:   await fetch(url)
来源：http://jy.yuntaijiaju.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://et.chemitech.net.cn

Go:   resp, err := http.Get(url)
来源：http://lt.wgjwhj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rv.gzmigu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oi.9csxet.cn

[L02] 发送 POST JSON
来源：http://od.lnxyls.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xc.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ct.yuexingan06.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hx.lnxyls.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gv.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://av.szxytkj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://br.hahajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://oq.9csxet.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kd.asd995.cn

[L03] 设置自定义请求头
来源：http://pv.jianghongdianzi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ny.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mf.9csxet.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fm.lnxyls.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nn.asd995.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ug.gzmigu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ie.hnjuh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gi.muxihuayi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qv.jianghongdianzi.cn

[L04] 设置超时
来源：http://ym.shtwfgs.cn

Py:   requests.get(url, timeout=5)
来源：http://sb.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sj.chemitech.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ku.shtwfgs.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rw.bookmarksfly.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ra.wgjwhj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sb.chemitech.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hq.yuexingan06.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tt.shxzskj.cn

[L05] 上传文件（multipart）
来源：http://yj.hnjuh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rc.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://di.521024.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://iz.colortex.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pa.hnjuh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dr.wgjwhj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://to.haigaiapp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sg.shxzskj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hl.hnjuh.cn

[L06] 解析响应为 JSON
来源：http://gf.wgjwhj.cn

Py:   resp.json()
来源：http://if.huixiangedu.cn

PHP:  json_decode($body, true);
来源：http://pq.yuntaijiaju.cn

JS:   await resp.json()
来源：http://bs.shxzskj.cn

TS:   await resp.json()
来源：http://ks.gzmigu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ft.bjjhwx.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ih.521024.cn

Ruby: JSON.parse(resp.body)
来源：http://gb.bookmarksfly.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yq.wgjwhj.cn

[L07] 处理 HTTP 状态码
来源：http://vy.panjiajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pv.hnjuh.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gl.haigaiapp.cn

JS:   resp.ok;  resp.status
来源：http://qn.huixinmuqiang.cn

TS:   resp.ok;  resp.status
来源：http://ji.bookmarksfly.cn

Java: resp.statusCode()
来源：http://cr.shxzukj.cn

Go:   resp.StatusCode
来源：http://rv.wgjwhj.cn

Ruby: resp.code.to_i
来源：http://pk.szsharing.cn

C#:   (int)resp.StatusCode
来源：http://um.shtwfgs.cn

[L08] 并发请求多个地址
来源：http://sq.bookmarksfly.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kg.shxzskj.cn

PHP:  curl_multi_init() 系列
来源：http://ew.haigaiapp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qj.asd995.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yw.jianghongdianzi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://oj.gzmigu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yx.panjiajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dh.asd995.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://is.colortex.cn

================================================================================
来源：http://by.wgjwhj.cn

M. 命令行 / 进程 / 环境
来源：http://lv.haigaiapp.cn

================================================================================
来源：http://tl.nicolike.cn

[M01] 读取命令行参数
来源：http://ty.szxytkj.cn

Py:   sys.argv[1:]
来源：http://ur.hnjuh.cn

PHP:  $argv;  $argc;
来源：http://zx.shtwfgs.cn

JS:   process.argv.slice(2)
来源：http://aq.gzmigu.cn

TS:   process.argv.slice(2)
来源：http://cz.nicolike.cn

Java: args 数组（main 方法参数）
来源：http://ps.yuexingan06.cn

Go:   os.Args[1:]
来源：http://yb.muxihuayi.cn

Ruby: ARGV
来源：http://uj.jctech888.com.cn

C#:   args 数组（Main 方法参数）
来源：http://cf.szsharing.cn

[M02] 读取环境变量
来源：http://kg.huixinmuqiang.cn

Py:   os.environ.get("HOME")
来源：http://nx.asd995.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://os.521024.cn

JS:   process.env.HOME
来源：http://oz.huixinmuqiang.cn

TS:   process.env.HOME
来源：http://sy.huanxung.cn

Java: System.getenv("HOME")
来源：http://px.haigaiapp.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gx.colortex.cn

Ruby: ENV["HOME"]
来源：http://zb.colortex.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ee.shxzukj.cn

[M03] 执行外部命令
来源：http://rx.asd995.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nm.shtwfgs.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bk.szsharing.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://lj.huanxung.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://du.521024.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jz.wgjwhj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qo.chemitech.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://id.521024.cn

C#:   Process.Start("ls", "-l");
来源：http://rs.szxytkj.cn

[M04] 获取当前工作目录
来源：http://ho.bjjhwx.cn

Py:   os.getcwd()
来源：http://xf.bjjhwx.cn

PHP:  getcwd();
来源：http://ye.szsharing.cn

JS:   process.cwd()
来源：http://wt.colortex.cn

TS:   process.cwd()
来源：http://hu.wgjwhj.cn

Java: Path.of("").toAbsolutePath()
来源：http://si.newstarts.cn

Go:   os.Getwd()
来源：http://uf.9csxet.cn

Ruby: Dir.pwd
来源：http://rb.nicolike.cn

C#:   Directory.GetCurrentDirectory()
来源：http://or.yuntaijiaju.cn

[M05] 设置退出码
来源：http://jt.9csxet.cn

Py:   sys.exit(1)
来源：http://pa.shtwfgs.cn

PHP:  exit(1);
来源：http://di.szxytkj.cn

JS:   process.exit(1)
来源：http://sb.hahajie.cn

TS:   process.exit(1)
来源：http://qs.huixiangedu.cn

Java: System.exit(1)
来源：http://ps.panjiajie.cn

Go:   os.Exit(1)
来源：http://ts.shxzukj.cn

Ruby: exit 1
来源：http://jk.haigaiapp.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hx.chemitech.net.cn

[M06] 向标准错误输出
来源：http://wo.colortex.cn

Py:   print("err", file=sys.stderr)
来源：http://vi.colortex.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://us.szsharing.cn

JS:   console.error("err")
来源：http://xa.muxihuayi.cn

TS:   console.error("err")
来源：http://ep.gzmigu.cn

Java: System.err.println("err")
来源：http://jl.nicolike.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fk.jctech888.com.cn

Ruby: warn "err"
来源：http://dj.jctech888.com.cn

C#:   Console.Error.WriteLine("err")
来源：http://ji.huanxung.cn

[M07] 判断是否为主入口
来源：http://ai.nicolike.cn

Py:   if __name__ == "__main__":
来源：http://ib.9csxet.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rp.panjiajie.cn

JS:   require.main === module
来源：http://yx.hahajie.cn

TS:   require.main === module
来源：http://un.panjiajie.cn


<!-- 参考信息 -->