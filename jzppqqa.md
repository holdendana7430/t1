代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mi.hahajie.cn

JS:   new Date();  Date.now()
来源：http://zj.jianghongdianzi.cn

TS:   new Date();  Date.now()
来源：http://hn.hnjuh.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vb.szsharing.cn

Go:   time.Now()
来源：http://oz.521024.cn

Ruby: Time.now
来源：http://vk.lnxyls.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dl.panjiajie.cn

[J02] 格式化输出
来源：http://cv.9csxet.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://od.huanxung.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://us.szxytkj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://av.bookmarksfly.cn

TS:   d.toISOString()
来源：http://qw.yuntaijiaju.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ak.huanxung.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ch.asd995.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bg.panjiajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sg.nicolike.cn

[J03] 字符串解析为日期
来源：http://ij.gzmigu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sh.hnjuh.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ut.haigaiapp.cn

JS:   new Date("2024-01-02")
来源：http://xv.muxihuayi.cn

TS:   new Date("2024-01-02")
来源：http://xy.yuntaijiaju.cn

Java: LocalDate.parse("2024-01-02")
来源：http://da.bjjhwx.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yw.wgjwhj.cn

Ruby: Date.parse("2024-01-02")
来源：http://pq.lnxyls.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rj.bjjhwx.cn

[J04] 时间戳与日期互转
来源：http://ya.521024.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://es.9csxet.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qp.szxytkj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dm.chemitech.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://nx.haigaiapp.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ef.shxzukj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cf.gzmigu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://au.521024.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ho.shxzukj.cn

[J05] 时间加减（加 7 天）
来源：http://bx.9csxet.cn

Py:   now + timedelta(days=7)
来源：http://hp.nicolike.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://fz.nicolike.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xh.gzmigu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lq.asd995.cn

Java: LocalDate.now().plusDays(7)
来源：http://xm.shxzskj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bz.nszjky.cn

Ruby: Time.now + 7 * 86400
来源：http://nu.yuexingan06.cn

C#:   DateTime.Now.AddDays(7)
来源：http://nu.szxytkj.cn

[J06] 计算两时间之差
来源：http://vd.521024.cn

Py:   (end - start).total_seconds()
来源：http://sk.bjjhwx.cn

PHP:  $end->diff($start)->days;
来源：http://rn.panjiajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://us.hnjuh.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gs.muxihuayi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bn.hnjuh.cn

Go:   end.Sub(start).Hours()
来源：http://sn.huixinmuqiang.cn

Ruby: end - start                 # 返回秒数
来源：http://qa.gzmigu.cn

C#:   (end - start).TotalSeconds
来源：http://nx.bookmarksfly.cn

[J07] 比较两个日期
来源：http://la.panjiajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://qs.shtwfgs.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tu.muxihuayi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://st.hnjuh.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xs.shtwfgs.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wf.gzmigu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cx.nicolike.cn

Ruby: d1 < d2;  d1 == d2
来源：http://eq.wgjwhj.cn

C#:   d1 < d2;  d1 == d2
来源：http://xx.9csxet.cn

[J08] 提取年月日与星期
来源：http://st.hnjuh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mi.bjjhwx.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://aa.yuexingan06.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xe.huixiangedu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ph.9csxet.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ka.yuexingan06.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zv.yuntaijiaju.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qh.yuntaijiaju.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ey.shxzukj.cn

[J09] 时区处理
来源：http://vk.nicolike.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wj.panjiajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fh.shxzskj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sr.muxihuayi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dt.nszjky.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sq.shxzukj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://re.hahajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fg.asd995.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sp.bookmarksfly.cn

[J10] 取今天 / 本月第一天
来源：http://sq.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kk.9csxet.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://np.bjjhwx.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://si.huixiangedu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lm.huixiangedu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dl.shxzukj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lg.jctech888.com.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yi.chemitech.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://za.muxihuayi.cn

================================================================================
来源：http://je.szsharing.cn

K. JSON 与序列化
来源：http://ii.shxzukj.cn

================================================================================
来源：http://tf.newstarts.cn

[K01] 对象转 JSON 字符串
来源：http://br.521024.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fa.lnxyls.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ux.shxzskj.cn

JS:   JSON.stringify(obj)
来源：http://ly.szxytkj.cn

TS:   JSON.stringify(obj)
来源：http://co.yuntaijiaju.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ep.huixinmuqiang.cn

Go:   json.Marshal(obj)
来源：http://ac.shtwfgs.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wb.gzmigu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vv.hahajie.cn

[K02] JSON 字符串转对象
来源：http://do.shxzskj.cn

Py:   json.loads(s)
来源：http://bq.huixiangedu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://md.colortex.cn

JS:   JSON.parse(s)
来源：http://ea.chemitech.net.cn

TS:   JSON.parse(s)
来源：http://hk.wgjwhj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ap.hnjuh.cn

Go:   json.Unmarshal(data, &v)
来源：http://oa.newstarts.cn

Ruby: JSON.parse(s)
来源：http://an.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://oj.wgjwhj.cn

[K03] JSON 美化输出（带缩进）
来源：http://kh.shxzukj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hb.9csxet.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zo.hahajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zz.shxzukj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tj.bookmarksfly.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qa.nicolike.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bh.szsharing.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gj.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fx.huixinmuqiang.cn

[K04] 读取 JSON 文件
来源：http://xa.huanxung.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fj.jianghongdianzi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ua.huixinmuqiang.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mz.yuexingan06.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dm.szxytkj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yv.nicolike.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tg.huanxung.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qs.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dt.lnxyls.cn

[K05] 深拷贝对象
来源：http://cg.colortex.cn

Py:   copy.deepcopy(obj)
来源：http://gq.muxihuayi.cn

PHP:  unserialize(serialize($obj));
来源：http://gq.bookmarksfly.cn

JS:   structuredClone(obj)
来源：http://md.yuntaijiaju.cn

TS:   structuredClone(obj)
来源：http://yg.haigaiapp.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tg.szxytkj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tz.haigaiapp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zf.gzmigu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gl.yuntaijiaju.cn

[K06] 解析 URL 查询串
来源：http://ng.shtwfgs.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wj.shxzskj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://me.huanxung.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mi.yuntaijiaju.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iw.panjiajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ed.newstarts.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cx.colortex.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rn.shxzskj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kg.hnjuh.cn

[K07] 进制转换
来源：http://mq.muxihuayi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ac.521024.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ol.wgjwhj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qg.huanxung.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gk.bookmarksfly.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rg.huixiangedu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ut.jctech888.com.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rb.hahajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hx.huixiangedu.cn

[K08] 二进制序列化（非 JSON）
来源：http://ew.huixiangedu.cn

Py:   pickle.dumps(obj)
来源：http://jh.bookmarksfly.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://es.yuntaijiaju.cn

JS:   v8.serialize(obj)        // Node
来源：http://lz.yuexingan06.cn

TS:   v8.serialize(obj)        // Node
来源：http://oc.asd995.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pk.szsharing.cn

Go:   encoding/gob
来源：http://hw.hahajie.cn

Ruby: Marshal.dump(obj)
来源：http://qr.hnjuh.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://eu.newstarts.cn

================================================================================
来源：http://kp.haigaiapp.cn

L. 网络请求
来源：http://ko.szsharing.cn

================================================================================
来源：http://tw.szxytkj.cn

[L01] 发送 GET 请求
来源：http://di.yuntaijiaju.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qt.yuntaijiaju.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://es.szsharing.cn

JS:   await fetch(url)
来源：http://gf.shtwfgs.cn

TS:   await fetch(url)
来源：http://yt.huixiangedu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dh.szsharing.cn

Go:   resp, err := http.Get(url)
来源：http://gd.shtwfgs.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://vv.haigaiapp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yf.newstarts.cn

[L02] 发送 POST JSON
来源：http://qo.jctech888.com.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ee.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://he.yuntaijiaju.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gr.szxytkj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vq.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ud.gzmigu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ar.huixiangedu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lf.jianghongdianzi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pd.nszjky.cn

[L03] 设置自定义请求头
来源：http://bf.yuexingan06.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sw.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mh.chemitech.net.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://at.shtwfgs.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://st.asd995.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://au.szsharing.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://km.panjiajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mj.hahajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kg.jianghongdianzi.cn

[L04] 设置超时
来源：http://qp.lnxyls.cn

Py:   requests.get(url, timeout=5)
来源：http://zc.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zs.szsharing.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fo.jianghongdianzi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hx.szsharing.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://db.asd995.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ik.shtwfgs.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cs.muxihuayi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qj.muxihuayi.cn

[L05] 上传文件（multipart）
来源：http://yj.yuntaijiaju.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bk.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://eg.szsharing.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ct.newstarts.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mg.jctech888.com.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pq.hahajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bg.gzmigu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://go.lnxyls.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ax.gzmigu.cn

[L06] 解析响应为 JSON
来源：http://fy.shxzukj.cn

Py:   resp.json()
来源：http://mp.shxzskj.cn

PHP:  json_decode($body, true);
来源：http://pg.szsharing.cn

JS:   await resp.json()
来源：http://wp.jianghongdianzi.cn

TS:   await resp.json()
来源：http://gi.huixinmuqiang.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ik.panjiajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://si.nicolike.cn

Ruby: JSON.parse(resp.body)
来源：http://oa.yuexingan06.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cq.shtwfgs.cn

[L07] 处理 HTTP 状态码
来源：http://ks.jctech888.com.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hq.bookmarksfly.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lu.gzmigu.cn

JS:   resp.ok;  resp.status
来源：http://yj.huanxung.cn

TS:   resp.ok;  resp.status
来源：http://kq.bookmarksfly.cn

Java: resp.statusCode()
来源：http://xl.yuexingan06.cn

Go:   resp.StatusCode
来源：http://ow.lnxyls.cn

Ruby: resp.code.to_i
来源：http://vd.chemitech.net.cn

C#:   (int)resp.StatusCode
来源：http://eo.shxzukj.cn

[L08] 并发请求多个地址
来源：http://og.521024.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ke.chemitech.net.cn

PHP:  curl_multi_init() 系列
来源：http://zv.newstarts.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kb.jctech888.com.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://al.chemitech.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ji.521024.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zo.hahajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ms.shxzskj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hs.521024.cn

================================================================================
来源：http://gz.chemitech.net.cn

M. 命令行 / 进程 / 环境
来源：http://rz.muxihuayi.cn

================================================================================
来源：http://xh.szsharing.cn

[M01] 读取命令行参数
来源：http://lv.huixinmuqiang.cn

Py:   sys.argv[1:]
来源：http://dn.yuexingan06.cn

PHP:  $argv;  $argc;
来源：http://cn.huixiangedu.cn

JS:   process.argv.slice(2)
来源：http://qi.521024.cn

TS:   process.argv.slice(2)
来源：http://tz.gzmigu.cn

Java: args 数组（main 方法参数）
来源：http://xf.9csxet.cn

Go:   os.Args[1:]
来源：http://qb.bjjhwx.cn

Ruby: ARGV
来源：http://np.jianghongdianzi.cn

C#:   args 数组（Main 方法参数）
来源：http://jl.newstarts.cn

[M02] 读取环境变量
来源：http://tf.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://da.nicolike.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ib.nicolike.cn

JS:   process.env.HOME
来源：http://yg.bookmarksfly.cn

TS:   process.env.HOME
来源：http://jm.shxzskj.cn

Java: System.getenv("HOME")
来源：http://hi.asd995.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yn.shtwfgs.cn

Ruby: ENV["HOME"]
来源：http://od.gzmigu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dj.wgjwhj.cn

[M03] 执行外部命令
来源：http://vp.hahajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ef.nszjky.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bi.yuntaijiaju.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://rw.huixiangedu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vw.hnjuh.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://to.newstarts.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://bd.wgjwhj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pq.huixiangedu.cn

C#:   Process.Start("ls", "-l");
来源：http://jl.huixiangedu.cn

[M04] 获取当前工作目录
来源：http://ve.shtwfgs.cn

Py:   os.getcwd()
来源：http://kc.shxzukj.cn

PHP:  getcwd();
来源：http://wa.nicolike.cn

JS:   process.cwd()
来源：http://eg.huixinmuqiang.cn

TS:   process.cwd()
来源：http://ug.bjjhwx.cn

Java: Path.of("").toAbsolutePath()
来源：http://ny.shxzskj.cn

Go:   os.Getwd()
来源：http://zr.szsharing.cn

Ruby: Dir.pwd
来源：http://ds.chemitech.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hf.muxihuayi.cn

[M05] 设置退出码
来源：http://kg.hnjuh.cn

Py:   sys.exit(1)
来源：http://av.jctech888.com.cn

PHP:  exit(1);
来源：http://wj.colortex.cn

JS:   process.exit(1)
来源：http://tx.yuexingan06.cn

TS:   process.exit(1)
来源：http://eq.521024.cn

Java: System.exit(1)
来源：http://kq.huixiangedu.cn

Go:   os.Exit(1)
来源：http://hh.nicolike.cn

Ruby: exit 1
来源：http://yc.szxytkj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://an.panjiajie.cn

[M06] 向标准错误输出
来源：http://mc.hahajie.cn

Py:   print("err", file=sys.stderr)
来源：http://xz.haigaiapp.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://td.nicolike.cn

JS:   console.error("err")
来源：http://tb.lnxyls.cn

TS:   console.error("err")
来源：http://tz.bookmarksfly.cn

Java: System.err.println("err")
来源：http://ga.szsharing.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qt.wgjwhj.cn

Ruby: warn "err"
来源：http://jk.9csxet.cn

C#:   Console.Error.WriteLine("err")
来源：http://sa.haigaiapp.cn

[M07] 判断是否为主入口
来源：http://ax.huanxung.cn

Py:   if __name__ == "__main__":
来源：http://pk.hnjuh.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vu.yuexingan06.cn

JS:   require.main === module
来源：http://mg.newstarts.cn

TS:   require.main === module
来源：http://af.szsharing.cn


<!-- 参考信息 -->