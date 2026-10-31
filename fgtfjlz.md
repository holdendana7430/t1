代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ey.asd995.cn

JS:   new Date();  Date.now()
来源：http://nh.hahajie.cn

TS:   new Date();  Date.now()
来源：http://qe.jianghongdianzi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ef.bjjhwx.cn

Go:   time.Now()
来源：http://ok.nicolike.cn

Ruby: Time.now
来源：http://kz.yuntaijiaju.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ri.huixinmuqiang.cn

[J02] 格式化输出
来源：http://kt.shxzskj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xu.shtwfgs.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gc.jianghongdianzi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ex.newstarts.cn

TS:   d.toISOString()
来源：http://en.panjiajie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://oe.colortex.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gw.colortex.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hw.huanxung.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ol.szxytkj.cn

[J03] 字符串解析为日期
来源：http://xh.nicolike.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jm.muxihuayi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mn.hnjuh.cn

JS:   new Date("2024-01-02")
来源：http://lv.colortex.cn

TS:   new Date("2024-01-02")
来源：http://dh.asd995.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ah.huanxung.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ob.jctech888.com.cn

Ruby: Date.parse("2024-01-02")
来源：http://gt.colortex.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zw.bookmarksfly.cn

[J04] 时间戳与日期互转
来源：http://zy.newstarts.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uu.shxzskj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qv.lnxyls.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ia.wgjwhj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qs.wgjwhj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rl.haigaiapp.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wl.nszjky.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ts.chemitech.net.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qu.lnxyls.cn

[J05] 时间加减（加 7 天）
来源：http://en.yuntaijiaju.cn

Py:   now + timedelta(days=7)
来源：http://td.szsharing.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ll.nszjky.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ob.szsharing.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://av.gzmigu.cn

Java: LocalDate.now().plusDays(7)
来源：http://qf.nicolike.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ps.muxihuayi.cn

Ruby: Time.now + 7 * 86400
来源：http://nu.bjjhwx.cn

C#:   DateTime.Now.AddDays(7)
来源：http://lr.szxytkj.cn

[J06] 计算两时间之差
来源：http://aq.shxzukj.cn

Py:   (end - start).total_seconds()
来源：http://hp.hnjuh.cn

PHP:  $end->diff($start)->days;
来源：http://uk.yuexingan06.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cv.chemitech.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rz.yuntaijiaju.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ba.yuntaijiaju.cn

Go:   end.Sub(start).Hours()
来源：http://jk.yuntaijiaju.cn

Ruby: end - start                 # 返回秒数
来源：http://oi.nicolike.cn

C#:   (end - start).TotalSeconds
来源：http://ul.gzmigu.cn

[J07] 比较两个日期
来源：http://rh.bjjhwx.cn

Py:   d1 < d2;  d1 == d2
来源：http://dp.bookmarksfly.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://eq.shtwfgs.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ba.szsharing.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qf.colortex.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vs.bookmarksfly.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://js.szxytkj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mw.bjjhwx.cn

C#:   d1 < d2;  d1 == d2
来源：http://yo.huanxung.cn

[J08] 提取年月日与星期
来源：http://gh.wgjwhj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wr.shxzskj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jd.gzmigu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wa.yuexingan06.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lu.nszjky.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wz.szsharing.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mh.panjiajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lv.lnxyls.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hy.szxytkj.cn

[J09] 时区处理
来源：http://et.huanxung.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pl.shxzukj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fh.huixinmuqiang.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://my.yuexingan06.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kk.9csxet.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yd.bjjhwx.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qx.chemitech.net.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jq.521024.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xu.hahajie.cn

[J10] 取今天 / 本月第一天
来源：http://ha.hahajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://id.yuexingan06.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dy.bjjhwx.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ak.shxzskj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ql.bookmarksfly.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bx.szxytkj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ru.huixiangedu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ik.bjjhwx.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://np.huixiangedu.cn

================================================================================
来源：http://sn.shxzskj.cn

K. JSON 与序列化
来源：http://pq.wgjwhj.cn

================================================================================
来源：http://st.szsharing.cn

[K01] 对象转 JSON 字符串
来源：http://ph.hnjuh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mb.hahajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tg.lnxyls.cn

JS:   JSON.stringify(obj)
来源：http://dc.bjjhwx.cn

TS:   JSON.stringify(obj)
来源：http://eq.panjiajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yb.szsharing.cn

Go:   json.Marshal(obj)
来源：http://za.bookmarksfly.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qo.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rq.yuexingan06.cn

[K02] JSON 字符串转对象
来源：http://ll.jctech888.com.cn

Py:   json.loads(s)
来源：http://vk.nicolike.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ko.huixinmuqiang.cn

JS:   JSON.parse(s)
来源：http://ex.yuexingan06.cn

TS:   JSON.parse(s)
来源：http://ss.gzmigu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pi.haigaiapp.cn

Go:   json.Unmarshal(data, &v)
来源：http://gl.hnjuh.cn

Ruby: JSON.parse(s)
来源：http://aw.521024.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yh.huanxung.cn

[K03] JSON 美化输出（带缩进）
来源：http://zu.szxytkj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nj.nszjky.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dl.nszjky.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://oq.asd995.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fb.newstarts.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vf.shtwfgs.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vq.9csxet.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ib.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ev.shxzukj.cn

[K04] 读取 JSON 文件
来源：http://wa.521024.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vk.hnjuh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://oy.bookmarksfly.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xs.huanxung.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lk.bjjhwx.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sd.lnxyls.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pb.jctech888.com.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://tl.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yd.bookmarksfly.cn

[K05] 深拷贝对象
来源：http://ak.chemitech.net.cn

Py:   copy.deepcopy(obj)
来源：http://oj.panjiajie.cn

PHP:  unserialize(serialize($obj));
来源：http://xa.newstarts.cn

JS:   structuredClone(obj)
来源：http://tp.gzmigu.cn

TS:   structuredClone(obj)
来源：http://wv.9csxet.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qd.shtwfgs.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pg.chemitech.net.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fm.jctech888.com.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yc.shxzskj.cn

[K06] 解析 URL 查询串
来源：http://al.muxihuayi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xt.shxzukj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://it.jctech888.com.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nb.lnxyls.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ij.wgjwhj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sw.yuntaijiaju.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ee.bookmarksfly.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pg.chemitech.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kl.szsharing.cn

[K07] 进制转换
来源：http://re.9csxet.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://my.szsharing.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mt.jianghongdianzi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pp.asd995.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ai.shxzukj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uf.huanxung.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vt.szxytkj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qf.jianghongdianzi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://eb.shxzukj.cn

[K08] 二进制序列化（非 JSON）
来源：http://sg.haigaiapp.cn

Py:   pickle.dumps(obj)
来源：http://wt.chemitech.net.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yw.wgjwhj.cn

JS:   v8.serialize(obj)        // Node
来源：http://wh.lnxyls.cn

TS:   v8.serialize(obj)        // Node
来源：http://fn.shtwfgs.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qp.shxzukj.cn

Go:   encoding/gob
来源：http://bg.hahajie.cn

Ruby: Marshal.dump(obj)
来源：http://tm.shxzukj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ll.jianghongdianzi.cn

================================================================================
来源：http://pr.gzmigu.cn

L. 网络请求
来源：http://sf.huanxung.cn

================================================================================
来源：http://ug.yuexingan06.cn

[L01] 发送 GET 请求
来源：http://lv.wgjwhj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dr.szxytkj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xl.jianghongdianzi.cn

JS:   await fetch(url)
来源：http://au.szxytkj.cn

TS:   await fetch(url)
来源：http://oe.jctech888.com.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rg.chemitech.net.cn

Go:   resp, err := http.Get(url)
来源：http://vq.bookmarksfly.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hw.panjiajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pu.521024.cn

[L02] 发送 POST JSON
来源：http://qt.jianghongdianzi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fm.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cy.jctech888.com.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jf.panjiajie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tc.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cb.huanxung.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tt.panjiajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ht.nicolike.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cc.huanxung.cn

[L03] 设置自定义请求头
来源：http://vu.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://no.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qe.9csxet.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ii.9csxet.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ht.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kl.jianghongdianzi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wg.huanxung.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ew.muxihuayi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cq.wgjwhj.cn

[L04] 设置超时
来源：http://ez.gzmigu.cn

Py:   requests.get(url, timeout=5)
来源：http://ld.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wi.shxzukj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ji.huixiangedu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gw.haigaiapp.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wp.gzmigu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://aq.huixinmuqiang.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nk.asd995.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xl.wgjwhj.cn

[L05] 上传文件（multipart）
来源：http://jl.colortex.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fb.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wc.jianghongdianzi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ms.shxzskj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lp.yuntaijiaju.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://oz.huixiangedu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dy.yuntaijiaju.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zc.nicolike.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pj.huanxung.cn

[L06] 解析响应为 JSON
来源：http://lg.huixinmuqiang.cn

Py:   resp.json()
来源：http://ly.muxihuayi.cn

PHP:  json_decode($body, true);
来源：http://gz.szsharing.cn

JS:   await resp.json()
来源：http://il.bjjhwx.cn

TS:   await resp.json()
来源：http://jk.newstarts.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qh.bjjhwx.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mk.huanxung.cn

Ruby: JSON.parse(resp.body)
来源：http://go.shxzukj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ha.shtwfgs.cn

[L07] 处理 HTTP 状态码
来源：http://vc.chemitech.net.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lc.shxzskj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dv.hnjuh.cn

JS:   resp.ok;  resp.status
来源：http://dj.hahajie.cn

TS:   resp.ok;  resp.status
来源：http://qs.panjiajie.cn

Java: resp.statusCode()
来源：http://ni.yuntaijiaju.cn

Go:   resp.StatusCode
来源：http://uu.szsharing.cn

Ruby: resp.code.to_i
来源：http://ax.haigaiapp.cn

C#:   (int)resp.StatusCode
来源：http://gm.jianghongdianzi.cn

[L08] 并发请求多个地址
来源：http://sa.newstarts.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ez.szsharing.cn

PHP:  curl_multi_init() 系列
来源：http://hg.wgjwhj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xe.9csxet.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ur.shxzskj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yz.panjiajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nr.nicolike.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sm.chemitech.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zl.huixinmuqiang.cn

================================================================================
来源：http://hp.nicolike.cn

M. 命令行 / 进程 / 环境
来源：http://hd.muxihuayi.cn

================================================================================
来源：http://ir.huanxung.cn

[M01] 读取命令行参数
来源：http://ks.bookmarksfly.cn

Py:   sys.argv[1:]
来源：http://lg.wgjwhj.cn

PHP:  $argv;  $argc;
来源：http://un.nszjky.cn

JS:   process.argv.slice(2)
来源：http://bz.lnxyls.cn

TS:   process.argv.slice(2)
来源：http://xy.asd995.cn

Java: args 数组（main 方法参数）
来源：http://yy.szsharing.cn

Go:   os.Args[1:]
来源：http://ep.huixiangedu.cn

Ruby: ARGV
来源：http://hj.szsharing.cn

C#:   args 数组（Main 方法参数）
来源：http://kw.chemitech.net.cn

[M02] 读取环境变量
来源：http://hr.jianghongdianzi.cn

Py:   os.environ.get("HOME")
来源：http://ip.newstarts.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hv.chemitech.net.cn

JS:   process.env.HOME
来源：http://pf.yuntaijiaju.cn

TS:   process.env.HOME
来源：http://tz.chemitech.net.cn

Java: System.getenv("HOME")
来源：http://jf.nicolike.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vg.gzmigu.cn

Ruby: ENV["HOME"]
来源：http://bh.hnjuh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mp.muxihuayi.cn

[M03] 执行外部命令
来源：http://ai.521024.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zf.9csxet.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ig.jianghongdianzi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://cp.jctech888.com.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vk.huanxung.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rb.huixinmuqiang.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ew.hahajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://af.bookmarksfly.cn

C#:   Process.Start("ls", "-l");
来源：http://lq.hnjuh.cn

[M04] 获取当前工作目录
来源：http://fd.jianghongdianzi.cn

Py:   os.getcwd()
来源：http://cv.gzmigu.cn

PHP:  getcwd();
来源：http://yf.bookmarksfly.cn

JS:   process.cwd()
来源：http://vi.huixiangedu.cn

TS:   process.cwd()
来源：http://ag.panjiajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://mw.huanxung.cn

Go:   os.Getwd()
来源：http://rm.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://ky.hnjuh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yy.jianghongdianzi.cn

[M05] 设置退出码
来源：http://gs.nszjky.cn

Py:   sys.exit(1)
来源：http://qo.huanxung.cn

PHP:  exit(1);
来源：http://ww.colortex.cn

JS:   process.exit(1)
来源：http://yf.yuexingan06.cn

TS:   process.exit(1)
来源：http://dr.bookmarksfly.cn

Java: System.exit(1)
来源：http://bn.shxzskj.cn

Go:   os.Exit(1)
来源：http://gk.colortex.cn

Ruby: exit 1
来源：http://tk.521024.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xv.lnxyls.cn

[M06] 向标准错误输出
来源：http://np.bjjhwx.cn

Py:   print("err", file=sys.stderr)
来源：http://sd.gzmigu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ac.colortex.cn

JS:   console.error("err")
来源：http://wg.muxihuayi.cn

TS:   console.error("err")
来源：http://yv.huanxung.cn

Java: System.err.println("err")
来源：http://sv.lnxyls.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tz.panjiajie.cn

Ruby: warn "err"
来源：http://gb.muxihuayi.cn

C#:   Console.Error.WriteLine("err")
来源：http://uv.jianghongdianzi.cn

[M07] 判断是否为主入口
来源：http://vw.huixinmuqiang.cn

Py:   if __name__ == "__main__":
来源：http://ns.colortex.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dd.huixiangedu.cn

JS:   require.main === module
来源：http://ey.asd995.cn

TS:   require.main === module
来源：http://jf.hnjuh.cn


<!-- 参考信息 -->