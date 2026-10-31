代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://os.nszjky.cn

JS:   new Date();  Date.now()
来源：http://py.jianghongdianzi.cn

TS:   new Date();  Date.now()
来源：http://tt.jianghongdianzi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rn.bookmarksfly.cn

Go:   time.Now()
来源：http://db.wgjwhj.cn

Ruby: Time.now
来源：http://cm.huanxung.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dy.muxihuayi.cn

[J02] 格式化输出
来源：http://xo.muxihuayi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sn.huanxung.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ij.szxytkj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yd.huixiangedu.cn

TS:   d.toISOString()
来源：http://wl.newstarts.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zj.chemitech.net.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ke.colortex.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xd.9csxet.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xs.haigaiapp.cn

[J03] 字符串解析为日期
来源：http://ws.szxytkj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jw.huixiangedu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://no.521024.cn

JS:   new Date("2024-01-02")
来源：http://ek.bookmarksfly.cn

TS:   new Date("2024-01-02")
来源：http://ww.panjiajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qa.521024.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rk.huixinmuqiang.cn

Ruby: Date.parse("2024-01-02")
来源：http://pg.asd995.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rp.nicolike.cn

[J04] 时间戳与日期互转
来源：http://xf.muxihuayi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xl.panjiajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gz.colortex.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lf.wgjwhj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://aj.gzmigu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ns.huixinmuqiang.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hr.hnjuh.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yy.bjjhwx.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tp.hnjuh.cn

[J05] 时间加减（加 7 天）
来源：http://hc.panjiajie.cn

Py:   now + timedelta(days=7)
来源：http://ta.gzmigu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kc.shxzukj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cv.szsharing.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uq.huanxung.cn

Java: LocalDate.now().plusDays(7)
来源：http://pv.huixiangedu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lr.haigaiapp.cn

Ruby: Time.now + 7 * 86400
来源：http://rk.panjiajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vu.szsharing.cn

[J06] 计算两时间之差
来源：http://yk.bjjhwx.cn

Py:   (end - start).total_seconds()
来源：http://ti.bjjhwx.cn

PHP:  $end->diff($start)->days;
来源：http://jw.colortex.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gy.gzmigu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xd.newstarts.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bi.huixinmuqiang.cn

Go:   end.Sub(start).Hours()
来源：http://yf.lnxyls.cn

Ruby: end - start                 # 返回秒数
来源：http://nx.huixiangedu.cn

C#:   (end - start).TotalSeconds
来源：http://yl.521024.cn

[J07] 比较两个日期
来源：http://up.bookmarksfly.cn

Py:   d1 < d2;  d1 == d2
来源：http://ko.shtwfgs.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://aj.szxytkj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ta.haigaiapp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://dh.bookmarksfly.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wx.nszjky.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ad.521024.cn

Ruby: d1 < d2;  d1 == d2
来源：http://nr.jctech888.com.cn

C#:   d1 < d2;  d1 == d2
来源：http://lx.shxzskj.cn

[J08] 提取年月日与星期
来源：http://ek.wgjwhj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ok.newstarts.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pw.haigaiapp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ax.colortex.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ee.newstarts.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zk.huixiangedu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://og.huixinmuqiang.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sn.9csxet.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tz.haigaiapp.cn

[J09] 时区处理
来源：http://br.panjiajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sa.newstarts.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sy.9csxet.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iu.hahajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hl.lnxyls.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yp.shxzskj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://co.shtwfgs.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hw.muxihuayi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bc.nicolike.cn

[J10] 取今天 / 本月第一天
来源：http://at.hahajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://eu.chemitech.net.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ny.jianghongdianzi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ca.jianghongdianzi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bi.chemitech.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qh.yuexingan06.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lm.hahajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xk.nszjky.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zt.huanxung.cn

================================================================================
来源：http://vh.shtwfgs.cn

K. JSON 与序列化
来源：http://xm.chemitech.net.cn

================================================================================
来源：http://vh.newstarts.cn

[K01] 对象转 JSON 字符串
来源：http://rn.huixiangedu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://og.shxzskj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lr.gzmigu.cn

JS:   JSON.stringify(obj)
来源：http://ww.szsharing.cn

TS:   JSON.stringify(obj)
来源：http://sw.panjiajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pn.szsharing.cn

Go:   json.Marshal(obj)
来源：http://ol.shtwfgs.cn

Ruby: obj.to_json                                     // require "json"
来源：http://tm.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://py.huixinmuqiang.cn

[K02] JSON 字符串转对象
来源：http://vj.chemitech.net.cn

Py:   json.loads(s)
来源：http://fj.shxzukj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://li.colortex.cn

JS:   JSON.parse(s)
来源：http://xo.muxihuayi.cn

TS:   JSON.parse(s)
来源：http://jk.wgjwhj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ju.bookmarksfly.cn

Go:   json.Unmarshal(data, &v)
来源：http://kx.newstarts.cn

Ruby: JSON.parse(s)
来源：http://ye.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yp.muxihuayi.cn

[K03] JSON 美化输出（带缩进）
来源：http://ek.chemitech.net.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pc.nszjky.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wp.asd995.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://is.yuexingan06.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xm.yuntaijiaju.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wu.asd995.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fz.panjiajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://yw.szxytkj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wx.shtwfgs.cn

[K04] 读取 JSON 文件
来源：http://bp.yuntaijiaju.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fs.hnjuh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lw.lnxyls.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zv.haigaiapp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xz.huanxung.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hn.521024.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xn.haigaiapp.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://at.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lt.jianghongdianzi.cn

[K05] 深拷贝对象
来源：http://od.yuexingan06.cn

Py:   copy.deepcopy(obj)
来源：http://la.gzmigu.cn

PHP:  unserialize(serialize($obj));
来源：http://vx.newstarts.cn

JS:   structuredClone(obj)
来源：http://ul.asd995.cn

TS:   structuredClone(obj)
来源：http://fb.bookmarksfly.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ov.gzmigu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://eh.szxytkj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ij.asd995.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mz.shxzskj.cn

[K06] 解析 URL 查询串
来源：http://ut.chemitech.net.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ui.wgjwhj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fi.yuntaijiaju.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lq.colortex.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ni.huanxung.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://om.huixinmuqiang.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zv.nszjky.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://du.lnxyls.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://va.bookmarksfly.cn

[K07] 进制转换
来源：http://gy.colortex.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ic.wgjwhj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ul.wgjwhj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rz.bookmarksfly.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wu.asd995.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://np.muxihuayi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hf.jianghongdianzi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://po.lnxyls.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uu.shxzskj.cn

[K08] 二进制序列化（非 JSON）
来源：http://yx.shtwfgs.cn

Py:   pickle.dumps(obj)
来源：http://ef.huixiangedu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ql.huanxung.cn

JS:   v8.serialize(obj)        // Node
来源：http://cp.yuexingan06.cn

TS:   v8.serialize(obj)        // Node
来源：http://ea.chemitech.net.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://si.haigaiapp.cn

Go:   encoding/gob
来源：http://cq.nicolike.cn

Ruby: Marshal.dump(obj)
来源：http://ff.chemitech.net.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xb.shtwfgs.cn

================================================================================
来源：http://yp.huixinmuqiang.cn

L. 网络请求
来源：http://kz.nszjky.cn

================================================================================
来源：http://pu.newstarts.cn

[L01] 发送 GET 请求
来源：http://nm.521024.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bk.bjjhwx.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ht.521024.cn

JS:   await fetch(url)
来源：http://iu.shxzskj.cn

TS:   await fetch(url)
来源：http://ia.asd995.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ak.szxytkj.cn

Go:   resp, err := http.Get(url)
来源：http://wy.huixinmuqiang.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://mv.bookmarksfly.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zj.huanxung.cn

[L02] 发送 POST JSON
来源：http://jb.bjjhwx.cn

Py:   requests.post(url, json={"a": 1})
来源：http://dl.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://id.521024.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dc.szsharing.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://do.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fv.szxytkj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fa.lnxyls.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pn.asd995.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cw.huixinmuqiang.cn

[L03] 设置自定义请求头
来源：http://in.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zz.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://up.9csxet.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ep.bookmarksfly.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ip.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://da.panjiajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pz.huixinmuqiang.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://oa.szsharing.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ql.huixinmuqiang.cn

[L04] 设置超时
来源：http://kz.bjjhwx.cn

Py:   requests.get(url, timeout=5)
来源：http://vc.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://li.muxihuayi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ot.yuexingan06.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://og.newstarts.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nl.haigaiapp.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ho.lnxyls.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zj.jianghongdianzi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yt.szsharing.cn

[L05] 上传文件（multipart）
来源：http://du.huixinmuqiang.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nr.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://at.huanxung.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yr.szxytkj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kv.yuexingan06.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ru.nicolike.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mt.jctech888.com.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hy.haigaiapp.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gt.szsharing.cn

[L06] 解析响应为 JSON
来源：http://lw.szsharing.cn

Py:   resp.json()
来源：http://lb.hahajie.cn

PHP:  json_decode($body, true);
来源：http://xx.newstarts.cn

JS:   await resp.json()
来源：http://qy.521024.cn

TS:   await resp.json()
来源：http://qd.shxzukj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zu.hnjuh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ql.bookmarksfly.cn

Ruby: JSON.parse(resp.body)
来源：http://dl.panjiajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vx.newstarts.cn

[L07] 处理 HTTP 状态码
来源：http://kh.521024.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lj.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lb.shxzskj.cn

JS:   resp.ok;  resp.status
来源：http://em.huanxung.cn

TS:   resp.ok;  resp.status
来源：http://cw.chemitech.net.cn

Java: resp.statusCode()
来源：http://de.panjiajie.cn

Go:   resp.StatusCode
来源：http://ss.colortex.cn

Ruby: resp.code.to_i
来源：http://uo.jianghongdianzi.cn

C#:   (int)resp.StatusCode
来源：http://xq.szxytkj.cn

[L08] 并发请求多个地址
来源：http://nt.yuexingan06.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kp.haigaiapp.cn

PHP:  curl_multi_init() 系列
来源：http://ug.nszjky.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xm.panjiajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gw.asd995.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mh.bookmarksfly.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bd.szxytkj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vm.jianghongdianzi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://km.lnxyls.cn

================================================================================
来源：http://wx.szsharing.cn

M. 命令行 / 进程 / 环境
来源：http://ks.jctech888.com.cn

================================================================================
来源：http://sn.lnxyls.cn

[M01] 读取命令行参数
来源：http://fu.szsharing.cn

Py:   sys.argv[1:]
来源：http://as.jctech888.com.cn

PHP:  $argv;  $argc;
来源：http://od.bookmarksfly.cn

JS:   process.argv.slice(2)
来源：http://jx.jctech888.com.cn

TS:   process.argv.slice(2)
来源：http://fa.wgjwhj.cn

Java: args 数组（main 方法参数）
来源：http://rb.nszjky.cn

Go:   os.Args[1:]
来源：http://oc.szxytkj.cn

Ruby: ARGV
来源：http://bl.521024.cn

C#:   args 数组（Main 方法参数）
来源：http://jz.gzmigu.cn

[M02] 读取环境变量
来源：http://fu.shtwfgs.cn

Py:   os.environ.get("HOME")
来源：http://ol.hnjuh.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zb.huixinmuqiang.cn

JS:   process.env.HOME
来源：http://nf.muxihuayi.cn

TS:   process.env.HOME
来源：http://ey.huixinmuqiang.cn

Java: System.getenv("HOME")
来源：http://dp.jianghongdianzi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ck.9csxet.cn

Ruby: ENV["HOME"]
来源：http://gz.yuntaijiaju.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dm.yuexingan06.cn

[M03] 执行外部命令
来源：http://zm.yuntaijiaju.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://oy.shxzskj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qt.asd995.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://sm.shtwfgs.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://va.jctech888.com.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mx.newstarts.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://js.huixinmuqiang.cn

Ruby: system("ls -l");  `ls -l`
来源：http://mr.shtwfgs.cn

C#:   Process.Start("ls", "-l");
来源：http://lz.newstarts.cn

[M04] 获取当前工作目录
来源：http://zl.chemitech.net.cn

Py:   os.getcwd()
来源：http://ir.asd995.cn

PHP:  getcwd();
来源：http://pu.panjiajie.cn

JS:   process.cwd()
来源：http://kg.wgjwhj.cn

TS:   process.cwd()
来源：http://gh.lnxyls.cn

Java: Path.of("").toAbsolutePath()
来源：http://im.newstarts.cn

Go:   os.Getwd()
来源：http://pd.lnxyls.cn

Ruby: Dir.pwd
来源：http://em.yuntaijiaju.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rf.chemitech.net.cn

[M05] 设置退出码
来源：http://uk.9csxet.cn

Py:   sys.exit(1)
来源：http://bi.shtwfgs.cn

PHP:  exit(1);
来源：http://cf.jianghongdianzi.cn

JS:   process.exit(1)
来源：http://mc.hnjuh.cn

TS:   process.exit(1)
来源：http://pq.jianghongdianzi.cn

Java: System.exit(1)
来源：http://xz.shxzskj.cn

Go:   os.Exit(1)
来源：http://bd.hnjuh.cn

Ruby: exit 1
来源：http://rh.hnjuh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bx.nicolike.cn

[M06] 向标准错误输出
来源：http://ea.muxihuayi.cn

Py:   print("err", file=sys.stderr)
来源：http://wk.wgjwhj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://iy.bjjhwx.cn

JS:   console.error("err")
来源：http://zh.chemitech.net.cn

TS:   console.error("err")
来源：http://jj.gzmigu.cn

Java: System.err.println("err")
来源：http://ea.muxihuayi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gz.hnjuh.cn

Ruby: warn "err"
来源：http://ha.colortex.cn

C#:   Console.Error.WriteLine("err")
来源：http://mz.huixinmuqiang.cn

[M07] 判断是否为主入口
来源：http://se.9csxet.cn

Py:   if __name__ == "__main__":
来源：http://tv.521024.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ob.asd995.cn

JS:   require.main === module
来源：http://ey.colortex.cn

TS:   require.main === module
来源：http://db.shtwfgs.cn


<!-- 参考信息 -->