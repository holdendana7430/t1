代发 wailian999

J. 日期与时间
来源：http://iy.szxytkj.cn

================================================================================
来源：http://pv.shxzukj.cn

[J01] 获取当前时间
来源：http://qv.bookmarksfly.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kx.huixinmuqiang.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wo.huixinmuqiang.cn

JS:   new Date();  Date.now()
来源：http://lk.bjjhwx.cn

TS:   new Date();  Date.now()
来源：http://jw.huixinmuqiang.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mt.hahajie.cn

Go:   time.Now()
来源：http://kj.9csxet.cn

Ruby: Time.now
来源：http://wt.szxytkj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://io.huanxung.cn

[J02] 格式化输出
来源：http://hx.nicolike.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ub.521024.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wm.colortex.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pr.hahajie.cn

TS:   d.toISOString()
来源：http://lv.huanxung.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nm.hnjuh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cp.shtwfgs.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ud.yuntaijiaju.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pf.521024.cn

[J03] 字符串解析为日期
来源：http://te.panjiajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ko.huanxung.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dt.yuexingan06.cn

JS:   new Date("2024-01-02")
来源：http://yp.panjiajie.cn

TS:   new Date("2024-01-02")
来源：http://kx.nszjky.cn

Java: LocalDate.parse("2024-01-02")
来源：http://lc.shxzskj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://be.muxihuayi.cn

Ruby: Date.parse("2024-01-02")
来源：http://kp.chemitech.net.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ta.nicolike.cn

[J04] 时间戳与日期互转
来源：http://pb.shtwfgs.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mu.521024.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://in.shtwfgs.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lj.asd995.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://pw.lnxyls.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uq.colortex.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ru.yuexingan06.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://js.521024.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xv.nicolike.cn

[J05] 时间加减（加 7 天）
来源：http://ft.bookmarksfly.cn

Py:   now + timedelta(days=7)
来源：http://af.shtwfgs.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mz.lnxyls.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://la.yuntaijiaju.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://aw.hahajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://ed.huixiangedu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://me.szsharing.cn

Ruby: Time.now + 7 * 86400
来源：http://ai.wgjwhj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vt.colortex.cn

[J06] 计算两时间之差
来源：http://ve.chemitech.net.cn

Py:   (end - start).total_seconds()
来源：http://ea.huixinmuqiang.cn

PHP:  $end->diff($start)->days;
来源：http://qu.shxzskj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cp.asd995.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://be.huixinmuqiang.cn

Java: Duration.between(start, end).toSeconds()
来源：http://cf.gzmigu.cn

Go:   end.Sub(start).Hours()
来源：http://rz.szsharing.cn

Ruby: end - start                 # 返回秒数
来源：http://dz.shxzskj.cn

C#:   (end - start).TotalSeconds
来源：http://wi.colortex.cn

[J07] 比较两个日期
来源：http://aj.nicolike.cn

Py:   d1 < d2;  d1 == d2
来源：http://as.shxzskj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ms.shxzukj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ui.nszjky.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jz.asd995.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ur.chemitech.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wa.shxzukj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ir.jianghongdianzi.cn

C#:   d1 < d2;  d1 == d2
来源：http://xn.hnjuh.cn

[J08] 提取年月日与星期
来源：http://cw.nicolike.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fz.szxytkj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://iw.nszjky.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mb.521024.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://na.gzmigu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pm.huanxung.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gx.hnjuh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://iv.shtwfgs.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ri.gzmigu.cn

[J09] 时区处理
来源：http://yy.muxihuayi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gv.asd995.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nb.shxzskj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wf.szxytkj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://br.hahajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tz.huanxung.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qx.hnjuh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vn.szxytkj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ni.panjiajie.cn

[J10] 取今天 / 本月第一天
来源：http://od.szsharing.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ak.lnxyls.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xx.jctech888.com.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ys.chemitech.net.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ph.yuntaijiaju.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ak.haigaiapp.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ja.lnxyls.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://en.jctech888.com.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qk.shxzukj.cn

================================================================================
来源：http://or.yuexingan06.cn

K. JSON 与序列化
来源：http://du.yuexingan06.cn

================================================================================
来源：http://dr.muxihuayi.cn

[K01] 对象转 JSON 字符串
来源：http://uk.yuexingan06.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fb.wgjwhj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lp.jctech888.com.cn

JS:   JSON.stringify(obj)
来源：http://uv.hahajie.cn

TS:   JSON.stringify(obj)
来源：http://oj.panjiajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zl.bjjhwx.cn

Go:   json.Marshal(obj)
来源：http://io.huanxung.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gk.521024.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ds.huixiangedu.cn

[K02] JSON 字符串转对象
来源：http://re.nicolike.cn

Py:   json.loads(s)
来源：http://gm.szxytkj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sj.9csxet.cn

JS:   JSON.parse(s)
来源：http://wp.jianghongdianzi.cn

TS:   JSON.parse(s)
来源：http://zg.nicolike.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jp.colortex.cn

Go:   json.Unmarshal(data, &v)
来源：http://ap.hnjuh.cn

Ruby: JSON.parse(s)
来源：http://sy.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://md.asd995.cn

[K03] JSON 美化输出（带缩进）
来源：http://xw.colortex.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bu.newstarts.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vy.huanxung.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://do.yuexingan06.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cs.hnjuh.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hn.chemitech.net.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rl.521024.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qj.huanxung.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ao.lnxyls.cn

[K04] 读取 JSON 文件
来源：http://bu.wgjwhj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tq.jctech888.com.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nf.huixiangedu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://or.newstarts.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nt.gzmigu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sp.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sn.newstarts.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://lf.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qv.haigaiapp.cn

[K05] 深拷贝对象
来源：http://fj.yuntaijiaju.cn

Py:   copy.deepcopy(obj)
来源：http://gy.yuntaijiaju.cn

PHP:  unserialize(serialize($obj));
来源：http://xi.chemitech.net.cn

JS:   structuredClone(obj)
来源：http://hx.haigaiapp.cn

TS:   structuredClone(obj)
来源：http://qw.szxytkj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wb.jctech888.com.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ma.yuexingan06.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://oi.panjiajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cr.9csxet.cn

[K06] 解析 URL 查询串
来源：http://fv.jianghongdianzi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dg.jianghongdianzi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mv.wgjwhj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ly.huanxung.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://se.shtwfgs.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ps.nicolike.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cn.colortex.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pu.huanxung.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ue.nicolike.cn

[K07] 进制转换
来源：http://fp.bjjhwx.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fr.huanxung.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://os.bookmarksfly.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://im.szxytkj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vh.panjiajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wb.hahajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pn.chemitech.net.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kq.yuntaijiaju.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wh.huixiangedu.cn

[K08] 二进制序列化（非 JSON）
来源：http://rh.szsharing.cn

Py:   pickle.dumps(obj)
来源：http://dm.szsharing.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gr.jctech888.com.cn

JS:   v8.serialize(obj)        // Node
来源：http://aj.shtwfgs.cn

TS:   v8.serialize(obj)        // Node
来源：http://vg.shxzukj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gl.lnxyls.cn

Go:   encoding/gob
来源：http://jg.shxzukj.cn

Ruby: Marshal.dump(obj)
来源：http://qq.hahajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://so.newstarts.cn

================================================================================
来源：http://iw.huanxung.cn

L. 网络请求
来源：http://as.newstarts.cn

================================================================================
来源：http://iw.haigaiapp.cn

[L01] 发送 GET 请求
来源：http://fv.huixinmuqiang.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xa.hahajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jr.wgjwhj.cn

JS:   await fetch(url)
来源：http://sb.521024.cn

TS:   await fetch(url)
来源：http://vl.chemitech.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wf.szsharing.cn

Go:   resp, err := http.Get(url)
来源：http://tt.colortex.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ev.panjiajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ef.chemitech.net.cn

[L02] 发送 POST JSON
来源：http://xj.shtwfgs.cn

Py:   requests.post(url, json={"a": 1})
来源：http://uc.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qw.muxihuayi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nt.chemitech.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cb.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ds.nicolike.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gt.muxihuayi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ox.huanxung.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fw.yuexingan06.cn

[L03] 设置自定义请求头
来源：http://qd.nicolike.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ws.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fl.chemitech.net.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ew.muxihuayi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://le.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sj.bookmarksfly.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bc.asd995.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ye.huixiangedu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ju.haigaiapp.cn

[L04] 设置超时
来源：http://wf.haigaiapp.cn

Py:   requests.get(url, timeout=5)
来源：http://ok.521024.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://st.9csxet.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ke.szsharing.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rz.nszjky.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nz.gzmigu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sf.9csxet.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qk.jianghongdianzi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uu.9csxet.cn

[L05] 上传文件（multipart）
来源：http://jv.hnjuh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sa.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cj.nszjky.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sg.lnxyls.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://py.shtwfgs.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bi.muxihuayi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ub.yuntaijiaju.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tk.muxihuayi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zi.colortex.cn

[L06] 解析响应为 JSON
来源：http://fp.shxzskj.cn

Py:   resp.json()
来源：http://gq.huixiangedu.cn

PHP:  json_decode($body, true);
来源：http://rt.newstarts.cn

JS:   await resp.json()
来源：http://qy.lnxyls.cn

TS:   await resp.json()
来源：http://cs.muxihuayi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cx.hnjuh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://as.nicolike.cn

Ruby: JSON.parse(resp.body)
来源：http://di.hahajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kx.hnjuh.cn

[L07] 处理 HTTP 状态码
来源：http://gf.hahajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cz.bookmarksfly.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sj.huixinmuqiang.cn

JS:   resp.ok;  resp.status
来源：http://al.jctech888.com.cn

TS:   resp.ok;  resp.status
来源：http://un.chemitech.net.cn

Java: resp.statusCode()
来源：http://hv.huanxung.cn

Go:   resp.StatusCode
来源：http://ih.hnjuh.cn

Ruby: resp.code.to_i
来源：http://ci.jctech888.com.cn

C#:   (int)resp.StatusCode
来源：http://ej.bjjhwx.cn

[L08] 并发请求多个地址
来源：http://ik.521024.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mt.shxzukj.cn

PHP:  curl_multi_init() 系列
来源：http://gb.jctech888.com.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lu.hahajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xd.jianghongdianzi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gj.shxzukj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ok.chemitech.net.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kx.haigaiapp.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lx.yuexingan06.cn

================================================================================
来源：http://am.shxzukj.cn

M. 命令行 / 进程 / 环境
来源：http://cy.huixiangedu.cn

================================================================================
来源：http://ps.shxzukj.cn

[M01] 读取命令行参数
来源：http://oa.shxzskj.cn

Py:   sys.argv[1:]
来源：http://cw.jianghongdianzi.cn

PHP:  $argv;  $argc;
来源：http://as.hahajie.cn

JS:   process.argv.slice(2)
来源：http://jk.wgjwhj.cn

TS:   process.argv.slice(2)
来源：http://aa.szxytkj.cn

Java: args 数组（main 方法参数）
来源：http://vy.521024.cn

Go:   os.Args[1:]
来源：http://ap.colortex.cn

Ruby: ARGV
来源：http://xs.szsharing.cn

C#:   args 数组（Main 方法参数）
来源：http://tb.gzmigu.cn

[M02] 读取环境变量
来源：http://tw.bjjhwx.cn

Py:   os.environ.get("HOME")
来源：http://yr.yuexingan06.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://an.huanxung.cn

JS:   process.env.HOME
来源：http://pk.chemitech.net.cn

TS:   process.env.HOME
来源：http://yl.lnxyls.cn

Java: System.getenv("HOME")
来源：http://oq.yuexingan06.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ze.521024.cn

Ruby: ENV["HOME"]
来源：http://ld.jianghongdianzi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://em.lnxyls.cn

[M03] 执行外部命令
来源：http://kl.jianghongdianzi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wx.szsharing.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fb.panjiajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://bs.521024.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://sv.bookmarksfly.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nc.shxzskj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dq.colortex.cn

Ruby: system("ls -l");  `ls -l`
来源：http://la.szxytkj.cn

C#:   Process.Start("ls", "-l");
来源：http://jy.jianghongdianzi.cn

[M04] 获取当前工作目录
来源：http://bt.haigaiapp.cn

Py:   os.getcwd()
来源：http://bj.haigaiapp.cn

PHP:  getcwd();
来源：http://ew.jctech888.com.cn

JS:   process.cwd()
来源：http://fp.newstarts.cn

TS:   process.cwd()
来源：http://xf.huixiangedu.cn

Java: Path.of("").toAbsolutePath()
来源：http://mn.jctech888.com.cn

Go:   os.Getwd()
来源：http://xa.huixinmuqiang.cn

Ruby: Dir.pwd
来源：http://uf.haigaiapp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sv.newstarts.cn

[M05] 设置退出码
来源：http://ys.huixiangedu.cn

Py:   sys.exit(1)
来源：http://gq.wgjwhj.cn

PHP:  exit(1);
来源：http://wy.9csxet.cn

JS:   process.exit(1)
来源：http://gx.jctech888.com.cn

TS:   process.exit(1)
来源：http://ts.yuntaijiaju.cn

Java: System.exit(1)
来源：http://gi.haigaiapp.cn

Go:   os.Exit(1)
来源：http://xl.newstarts.cn

Ruby: exit 1
来源：http://nr.bookmarksfly.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://iw.newstarts.cn

[M06] 向标准错误输出
来源：http://vr.muxihuayi.cn

Py:   print("err", file=sys.stderr)
来源：http://tu.bookmarksfly.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cs.wgjwhj.cn

JS:   console.error("err")
来源：http://fv.lnxyls.cn

TS:   console.error("err")
来源：http://tt.shxzskj.cn

Java: System.err.println("err")
来源：http://ro.521024.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://li.muxihuayi.cn

Ruby: warn "err"
来源：http://he.hnjuh.cn

C#:   Console.Error.WriteLine("err")
来源：http://ct.newstarts.cn

[M07] 判断是否为主入口
来源：http://as.lnxyls.cn


<!-- 参考信息 -->