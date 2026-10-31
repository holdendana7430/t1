代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yz.bjjhwx.cn

JS:   new Date();  Date.now()
来源：http://bn.huixiangedu.cn

TS:   new Date();  Date.now()
来源：http://sk.jctech888.com.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jb.shxzukj.cn

Go:   time.Now()
来源：http://li.newstarts.cn

Ruby: Time.now
来源：http://ix.shxzukj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zn.shxzukj.cn

[J02] 格式化输出
来源：http://ju.shtwfgs.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dv.jctech888.com.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qj.wgjwhj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tb.jctech888.com.cn

TS:   d.toISOString()
来源：http://id.wgjwhj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://do.wgjwhj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bb.asd995.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zr.panjiajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ai.haigaiapp.cn

[J03] 字符串解析为日期
来源：http://bi.521024.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kq.panjiajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://aa.bookmarksfly.cn

JS:   new Date("2024-01-02")
来源：http://nj.szsharing.cn

TS:   new Date("2024-01-02")
来源：http://ku.muxihuayi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ue.newstarts.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fy.szxytkj.cn

Ruby: Date.parse("2024-01-02")
来源：http://pn.gzmigu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://em.panjiajie.cn

[J04] 时间戳与日期互转
来源：http://iy.chemitech.net.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yb.wgjwhj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jj.gzmigu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://iq.hnjuh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xa.panjiajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sn.bookmarksfly.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cf.jctech888.com.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lp.hnjuh.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pt.shxzskj.cn

[J05] 时间加减（加 7 天）
来源：http://yn.jctech888.com.cn

Py:   now + timedelta(days=7)
来源：http://bo.9csxet.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://db.huixinmuqiang.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ef.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ie.huanxung.cn

Java: LocalDate.now().plusDays(7)
来源：http://qb.shxzukj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jl.shxzskj.cn

Ruby: Time.now + 7 * 86400
来源：http://oo.nszjky.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pz.bookmarksfly.cn

[J06] 计算两时间之差
来源：http://li.chemitech.net.cn

Py:   (end - start).total_seconds()
来源：http://fn.jctech888.com.cn

PHP:  $end->diff($start)->days;
来源：http://za.huixinmuqiang.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qi.huixiangedu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kl.shxzskj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ik.bookmarksfly.cn

Go:   end.Sub(start).Hours()
来源：http://vr.szxytkj.cn

Ruby: end - start                 # 返回秒数
来源：http://na.nszjky.cn

C#:   (end - start).TotalSeconds
来源：http://wt.jianghongdianzi.cn

[J07] 比较两个日期
来源：http://hj.huanxung.cn

Py:   d1 < d2;  d1 == d2
来源：http://mw.nszjky.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ra.panjiajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vf.huanxung.cn

TS:   d1.getTime() < d2.getTime()
来源：http://cx.huixiangedu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wd.szsharing.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sc.haigaiapp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xm.jianghongdianzi.cn

C#:   d1 < d2;  d1 == d2
来源：http://ly.huixiangedu.cn

[J08] 提取年月日与星期
来源：http://ak.haigaiapp.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ac.muxihuayi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vi.huixiangedu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tb.huixiangedu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pf.wgjwhj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bd.panjiajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vf.hnjuh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://um.521024.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uv.yuexingan06.cn

[J09] 时区处理
来源：http://jp.shxzskj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uq.lnxyls.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pe.lnxyls.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kd.lnxyls.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qt.nszjky.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hn.hnjuh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cv.hnjuh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tg.hnjuh.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sl.hnjuh.cn

[J10] 取今天 / 本月第一天
来源：http://tc.bookmarksfly.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ay.nicolike.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://he.521024.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uu.hnjuh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ky.shtwfgs.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wx.yuntaijiaju.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ef.shxzukj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://so.haigaiapp.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gp.shxzukj.cn

================================================================================
来源：http://ca.muxihuayi.cn

K. JSON 与序列化
来源：http://jm.gzmigu.cn

================================================================================
来源：http://hb.shtwfgs.cn

[K01] 对象转 JSON 字符串
来源：http://ux.szxytkj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lc.huixiangedu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bx.chemitech.net.cn

JS:   JSON.stringify(obj)
来源：http://zl.bookmarksfly.cn

TS:   JSON.stringify(obj)
来源：http://rp.shtwfgs.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pw.nszjky.cn

Go:   json.Marshal(obj)
来源：http://pl.jianghongdianzi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gr.panjiajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ul.hnjuh.cn

[K02] JSON 字符串转对象
来源：http://to.muxihuayi.cn

Py:   json.loads(s)
来源：http://dc.newstarts.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kq.jctech888.com.cn

JS:   JSON.parse(s)
来源：http://yj.yuntaijiaju.cn

TS:   JSON.parse(s)
来源：http://zs.hahajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ba.jianghongdianzi.cn

Go:   json.Unmarshal(data, &v)
来源：http://bk.haigaiapp.cn

Ruby: JSON.parse(s)
来源：http://ps.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fw.szsharing.cn

[K03] JSON 美化输出（带缩进）
来源：http://hn.bjjhwx.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://go.asd995.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hc.colortex.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xf.colortex.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://js.nszjky.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pz.bookmarksfly.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mk.asd995.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ni.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://in.nicolike.cn

[K04] 读取 JSON 文件
来源：http://iu.panjiajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://le.asd995.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ou.huixinmuqiang.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xz.shtwfgs.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ll.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://oa.bookmarksfly.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mj.chemitech.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jo.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dn.hahajie.cn

[K05] 深拷贝对象
来源：http://qh.szsharing.cn

Py:   copy.deepcopy(obj)
来源：http://rk.jianghongdianzi.cn

PHP:  unserialize(serialize($obj));
来源：http://nw.huanxung.cn

JS:   structuredClone(obj)
来源：http://qo.gzmigu.cn

TS:   structuredClone(obj)
来源：http://cl.hnjuh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gr.yuexingan06.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://um.panjiajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vy.haigaiapp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://eq.shtwfgs.cn

[K06] 解析 URL 查询串
来源：http://ke.chemitech.net.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hl.huanxung.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vm.huixiangedu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ye.shxzukj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tj.bookmarksfly.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vo.hahajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://yy.haigaiapp.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vl.colortex.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vy.nicolike.cn

[K07] 进制转换
来源：http://kq.newstarts.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://oz.szxytkj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gq.shtwfgs.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ok.muxihuayi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xw.szxytkj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jq.bjjhwx.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ee.asd995.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cp.bjjhwx.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xi.asd995.cn

[K08] 二进制序列化（非 JSON）
来源：http://yw.hnjuh.cn

Py:   pickle.dumps(obj)
来源：http://rw.shtwfgs.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yi.lnxyls.cn

JS:   v8.serialize(obj)        // Node
来源：http://oi.colortex.cn

TS:   v8.serialize(obj)        // Node
来源：http://it.bookmarksfly.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yj.jctech888.com.cn

Go:   encoding/gob
来源：http://fa.huixinmuqiang.cn

Ruby: Marshal.dump(obj)
来源：http://jf.bjjhwx.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://np.shxzskj.cn

================================================================================
来源：http://dz.wgjwhj.cn

L. 网络请求
来源：http://qv.muxihuayi.cn

================================================================================
来源：http://qv.huixinmuqiang.cn

[L01] 发送 GET 请求
来源：http://uc.gzmigu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pt.szsharing.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lb.huixiangedu.cn

JS:   await fetch(url)
来源：http://fl.yuntaijiaju.cn

TS:   await fetch(url)
来源：http://ch.lnxyls.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uu.wgjwhj.cn

Go:   resp, err := http.Get(url)
来源：http://pw.nszjky.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zr.huanxung.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pw.shtwfgs.cn

[L02] 发送 POST JSON
来源：http://cr.panjiajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://dy.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tf.gzmigu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gl.colortex.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://um.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lv.huixiangedu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lr.lnxyls.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fy.shxzukj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zf.nszjky.cn

[L03] 设置自定义请求头
来源：http://bm.shxzukj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://da.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yf.9csxet.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ue.nicolike.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gu.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://km.huanxung.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xy.newstarts.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uz.huixiangedu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pn.jctech888.com.cn

[L04] 设置超时
来源：http://ge.wgjwhj.cn

Py:   requests.get(url, timeout=5)
来源：http://ub.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qz.szsharing.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bb.gzmigu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ra.panjiajie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xl.huixiangedu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zl.haigaiapp.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gt.newstarts.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jg.jianghongdianzi.cn

[L05] 上传文件（multipart）
来源：http://ka.chemitech.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://su.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yx.hahajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://po.hnjuh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jn.wgjwhj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hi.hahajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xi.lnxyls.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ad.huixinmuqiang.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ta.lnxyls.cn

[L06] 解析响应为 JSON
来源：http://yw.gzmigu.cn

Py:   resp.json()
来源：http://qv.gzmigu.cn

PHP:  json_decode($body, true);
来源：http://at.panjiajie.cn

JS:   await resp.json()
来源：http://pb.jianghongdianzi.cn

TS:   await resp.json()
来源：http://zr.haigaiapp.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qz.bookmarksfly.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rf.yuexingan06.cn

Ruby: JSON.parse(resp.body)
来源：http://cw.wgjwhj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uy.bjjhwx.cn

[L07] 处理 HTTP 状态码
来源：http://ou.asd995.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ok.nicolike.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mz.yuexingan06.cn

JS:   resp.ok;  resp.status
来源：http://tr.chemitech.net.cn

TS:   resp.ok;  resp.status
来源：http://fo.gzmigu.cn

Java: resp.statusCode()
来源：http://ze.szxytkj.cn

Go:   resp.StatusCode
来源：http://yh.bookmarksfly.cn

Ruby: resp.code.to_i
来源：http://fy.colortex.cn

C#:   (int)resp.StatusCode
来源：http://ua.huixiangedu.cn

[L08] 并发请求多个地址
来源：http://xa.wgjwhj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ym.colortex.cn

PHP:  curl_multi_init() 系列
来源：http://wa.yuexingan06.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zz.newstarts.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kg.huanxung.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hj.huixiangedu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wb.haigaiapp.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rr.hnjuh.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bw.nszjky.cn

================================================================================
来源：http://bb.colortex.cn

M. 命令行 / 进程 / 环境
来源：http://sm.bookmarksfly.cn

================================================================================
来源：http://ik.jctech888.com.cn

[M01] 读取命令行参数
来源：http://hx.chemitech.net.cn

Py:   sys.argv[1:]
来源：http://ug.jctech888.com.cn

PHP:  $argv;  $argc;
来源：http://ib.lnxyls.cn

JS:   process.argv.slice(2)
来源：http://wo.panjiajie.cn

TS:   process.argv.slice(2)
来源：http://uc.521024.cn

Java: args 数组（main 方法参数）
来源：http://cn.lnxyls.cn

Go:   os.Args[1:]
来源：http://hk.yuexingan06.cn

Ruby: ARGV
来源：http://cd.szsharing.cn

C#:   args 数组（Main 方法参数）
来源：http://ih.nszjky.cn

[M02] 读取环境变量
来源：http://bg.huanxung.cn

Py:   os.environ.get("HOME")
来源：http://xb.colortex.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pg.bookmarksfly.cn

JS:   process.env.HOME
来源：http://ld.yuntaijiaju.cn

TS:   process.env.HOME
来源：http://do.haigaiapp.cn

Java: System.getenv("HOME")
来源：http://sr.lnxyls.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lx.szxytkj.cn

Ruby: ENV["HOME"]
来源：http://yl.muxihuayi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dx.gzmigu.cn

[M03] 执行外部命令
来源：http://by.bookmarksfly.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cz.jianghongdianzi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rp.bjjhwx.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pd.huixinmuqiang.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://kq.gzmigu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mx.asd995.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qx.shxzskj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bv.bookmarksfly.cn

C#:   Process.Start("ls", "-l");
来源：http://wq.colortex.cn

[M04] 获取当前工作目录
来源：http://jw.9csxet.cn

Py:   os.getcwd()
来源：http://he.lnxyls.cn

PHP:  getcwd();
来源：http://lb.hahajie.cn

JS:   process.cwd()
来源：http://vo.panjiajie.cn

TS:   process.cwd()
来源：http://bb.szsharing.cn

Java: Path.of("").toAbsolutePath()
来源：http://xz.bjjhwx.cn

Go:   os.Getwd()
来源：http://nm.szxytkj.cn

Ruby: Dir.pwd
来源：http://mj.asd995.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vr.gzmigu.cn

[M05] 设置退出码
来源：http://ct.bookmarksfly.cn

Py:   sys.exit(1)
来源：http://cx.panjiajie.cn

PHP:  exit(1);
来源：http://ho.nszjky.cn

JS:   process.exit(1)
来源：http://hh.chemitech.net.cn

TS:   process.exit(1)
来源：http://pp.shxzskj.cn

Java: System.exit(1)
来源：http://zn.szxytkj.cn

Go:   os.Exit(1)
来源：http://fw.haigaiapp.cn

Ruby: exit 1
来源：http://md.521024.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ae.asd995.cn

[M06] 向标准错误输出
来源：http://ht.gzmigu.cn

Py:   print("err", file=sys.stderr)
来源：http://zg.shtwfgs.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://zr.hahajie.cn

JS:   console.error("err")
来源：http://ta.nicolike.cn

TS:   console.error("err")
来源：http://gl.bjjhwx.cn

Java: System.err.println("err")
来源：http://py.jianghongdianzi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zu.521024.cn

Ruby: warn "err"
来源：http://ty.huanxung.cn

C#:   Console.Error.WriteLine("err")
来源：http://be.yuexingan06.cn

[M07] 判断是否为主入口
来源：http://gs.bjjhwx.cn

Py:   if __name__ == "__main__":
来源：http://uv.hahajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qs.panjiajie.cn

JS:   require.main === module
来源：http://oe.huanxung.cn

TS:   require.main === module
来源：http://wy.shxzskj.cn


<!-- 参考信息 -->