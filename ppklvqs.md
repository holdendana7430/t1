代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ir.shxzukj.cn

JS:   new Date();  Date.now()
来源：http://uk.bookmarksfly.cn

TS:   new Date();  Date.now()
来源：http://sd.haigaiapp.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ys.colortex.cn

Go:   time.Now()
来源：http://bf.muxihuayi.cn

Ruby: Time.now
来源：http://th.nszjky.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lj.haigaiapp.cn

[J02] 格式化输出
来源：http://da.huixinmuqiang.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ay.hahajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wx.huixiangedu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yn.hahajie.cn

TS:   d.toISOString()
来源：http://sv.gzmigu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://op.hnjuh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ym.newstarts.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ud.panjiajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://az.hahajie.cn

[J03] 字符串解析为日期
来源：http://yo.yuntaijiaju.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tv.jctech888.com.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ao.jctech888.com.cn

JS:   new Date("2024-01-02")
来源：http://nl.newstarts.cn

TS:   new Date("2024-01-02")
来源：http://bm.yuntaijiaju.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xr.chemitech.net.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://io.haigaiapp.cn

Ruby: Date.parse("2024-01-02")
来源：http://ah.hahajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://to.muxihuayi.cn

[J04] 时间戳与日期互转
来源：http://eo.hnjuh.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tf.huixiangedu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nf.bookmarksfly.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kn.shxzskj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://mn.newstarts.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tn.asd995.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wr.nicolike.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ym.asd995.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jk.jctech888.com.cn

[J05] 时间加减（加 7 天）
来源：http://gp.yuntaijiaju.cn

Py:   now + timedelta(days=7)
来源：http://zj.lnxyls.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://je.hnjuh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kq.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ae.asd995.cn

Java: LocalDate.now().plusDays(7)
来源：http://du.bjjhwx.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wu.wgjwhj.cn

Ruby: Time.now + 7 * 86400
来源：http://dc.shxzukj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ln.szxytkj.cn

[J06] 计算两时间之差
来源：http://zt.shtwfgs.cn

Py:   (end - start).total_seconds()
来源：http://dn.jctech888.com.cn

PHP:  $end->diff($start)->days;
来源：http://dm.haigaiapp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fc.muxihuayi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ay.muxihuayi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fh.nicolike.cn

Go:   end.Sub(start).Hours()
来源：http://vk.newstarts.cn

Ruby: end - start                 # 返回秒数
来源：http://vr.yuexingan06.cn

C#:   (end - start).TotalSeconds
来源：http://za.shtwfgs.cn

[J07] 比较两个日期
来源：http://aq.huixiangedu.cn

Py:   d1 < d2;  d1 == d2
来源：http://wq.9csxet.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vi.shxzskj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jv.jctech888.com.cn

TS:   d1.getTime() < d2.getTime()
来源：http://id.muxihuayi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tr.gzmigu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ft.hahajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://is.9csxet.cn

C#:   d1 < d2;  d1 == d2
来源：http://lh.newstarts.cn

[J08] 提取年月日与星期
来源：http://cn.yuexingan06.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ns.haigaiapp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xq.bookmarksfly.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nq.bjjhwx.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hs.huanxung.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qe.colortex.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ff.nicolike.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://oe.muxihuayi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vj.szsharing.cn

[J09] 时区处理
来源：http://cf.szsharing.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vu.jctech888.com.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pj.panjiajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oh.hahajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rh.shxzukj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ub.9csxet.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://oc.yuntaijiaju.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yd.huixiangedu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rr.hnjuh.cn

[J10] 取今天 / 本月第一天
来源：http://od.nicolike.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xr.newstarts.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lv.hahajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ji.nicolike.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fo.shtwfgs.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rj.gzmigu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xu.szxytkj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ys.muxihuayi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://su.wgjwhj.cn

================================================================================
来源：http://lp.panjiajie.cn

K. JSON 与序列化
来源：http://hi.yuexingan06.cn

================================================================================
来源：http://fi.newstarts.cn

[K01] 对象转 JSON 字符串
来源：http://ly.shxzukj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fs.lnxyls.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wz.szxytkj.cn

JS:   JSON.stringify(obj)
来源：http://pm.shxzskj.cn

TS:   JSON.stringify(obj)
来源：http://fr.yuexingan06.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ls.haigaiapp.cn

Go:   json.Marshal(obj)
来源：http://hy.shxzskj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rc.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ht.newstarts.cn

[K02] JSON 字符串转对象
来源：http://ca.hahajie.cn

Py:   json.loads(s)
来源：http://of.colortex.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nv.huixiangedu.cn

JS:   JSON.parse(s)
来源：http://ab.chemitech.net.cn

TS:   JSON.parse(s)
来源：http://bm.shxzskj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kg.newstarts.cn

Go:   json.Unmarshal(data, &v)
来源：http://ub.hahajie.cn

Ruby: JSON.parse(s)
来源：http://sz.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fp.szxytkj.cn

[K03] JSON 美化输出（带缩进）
来源：http://uu.asd995.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fl.hahajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ih.bookmarksfly.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gt.muxihuayi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ha.haigaiapp.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mo.jctech888.com.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yp.shxzukj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://us.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vc.521024.cn

[K04] 读取 JSON 文件
来源：http://ho.nicolike.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qy.shxzukj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wi.9csxet.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gb.haigaiapp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xe.panjiajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sf.521024.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ch.muxihuayi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wc.hnjuh.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rw.huixinmuqiang.cn

[K05] 深拷贝对象
来源：http://ij.huixinmuqiang.cn

Py:   copy.deepcopy(obj)
来源：http://iv.colortex.cn

PHP:  unserialize(serialize($obj));
来源：http://lk.shxzukj.cn

JS:   structuredClone(obj)
来源：http://vu.huanxung.cn

TS:   structuredClone(obj)
来源：http://al.jctech888.com.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ox.newstarts.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jh.huanxung.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pj.gzmigu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://is.asd995.cn

[K06] 解析 URL 查询串
来源：http://bw.szxytkj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dp.huanxung.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://my.9csxet.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pv.szxytkj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vf.shxzukj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mv.hnjuh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gc.newstarts.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ju.haigaiapp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ow.szsharing.cn

[K07] 进制转换
来源：http://wv.colortex.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://eq.nszjky.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ed.haigaiapp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wy.lnxyls.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pb.jianghongdianzi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ke.huanxung.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kd.colortex.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ub.yuexingan06.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fn.9csxet.cn

[K08] 二进制序列化（非 JSON）
来源：http://ag.shxzskj.cn

Py:   pickle.dumps(obj)
来源：http://tq.shxzskj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tm.colortex.cn

JS:   v8.serialize(obj)        // Node
来源：http://gw.szxytkj.cn

TS:   v8.serialize(obj)        // Node
来源：http://op.huanxung.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dl.nszjky.cn

Go:   encoding/gob
来源：http://ny.yuntaijiaju.cn

Ruby: Marshal.dump(obj)
来源：http://az.hnjuh.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://to.shxzskj.cn

================================================================================
来源：http://nk.9csxet.cn

L. 网络请求
来源：http://wp.jctech888.com.cn

================================================================================
来源：http://uo.shxzskj.cn

[L01] 发送 GET 请求
来源：http://ef.colortex.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://iw.nszjky.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fe.9csxet.cn

JS:   await fetch(url)
来源：http://zv.yuntaijiaju.cn

TS:   await fetch(url)
来源：http://va.nszjky.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://iv.yuexingan06.cn

Go:   resp, err := http.Get(url)
来源：http://mb.bjjhwx.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ym.gzmigu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mj.yuexingan06.cn

[L02] 发送 POST JSON
来源：http://pm.shxzskj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://kh.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yz.jctech888.com.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mk.colortex.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zr.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vz.yuexingan06.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zx.gzmigu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xd.nicolike.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vz.colortex.cn

[L03] 设置自定义请求头
来源：http://id.bookmarksfly.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gd.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ct.shxzukj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rf.521024.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nw.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ce.jianghongdianzi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nj.colortex.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qg.wgjwhj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qo.colortex.cn

[L04] 设置超时
来源：http://sh.szxytkj.cn

Py:   requests.get(url, timeout=5)
来源：http://uh.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zf.bookmarksfly.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jh.bjjhwx.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sh.nicolike.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yp.521024.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vx.asd995.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ff.szxytkj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fa.gzmigu.cn

[L05] 上传文件（multipart）
来源：http://ar.521024.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ex.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bu.szsharing.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://be.yuntaijiaju.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hj.chemitech.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://in.huixinmuqiang.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://es.szxytkj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vx.muxihuayi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yt.huanxung.cn

[L06] 解析响应为 JSON
来源：http://rl.newstarts.cn

Py:   resp.json()
来源：http://wj.hahajie.cn

PHP:  json_decode($body, true);
来源：http://mt.huixinmuqiang.cn

JS:   await resp.json()
来源：http://rh.jctech888.com.cn

TS:   await resp.json()
来源：http://mv.jianghongdianzi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://do.yuexingan06.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zm.hahajie.cn

Ruby: JSON.parse(resp.body)
来源：http://ov.huixinmuqiang.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fl.colortex.cn

[L07] 处理 HTTP 状态码
来源：http://ae.bjjhwx.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nr.nicolike.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ti.lnxyls.cn

JS:   resp.ok;  resp.status
来源：http://kt.muxihuayi.cn

TS:   resp.ok;  resp.status
来源：http://zu.huixiangedu.cn

Java: resp.statusCode()
来源：http://ob.hnjuh.cn

Go:   resp.StatusCode
来源：http://yq.shtwfgs.cn

Ruby: resp.code.to_i
来源：http://vi.lnxyls.cn

C#:   (int)resp.StatusCode
来源：http://kd.hahajie.cn

[L08] 并发请求多个地址
来源：http://su.haigaiapp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://em.bjjhwx.cn

PHP:  curl_multi_init() 系列
来源：http://nj.huixinmuqiang.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lx.panjiajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oe.yuexingan06.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kk.jctech888.com.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lo.bookmarksfly.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tn.szsharing.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kb.wgjwhj.cn

================================================================================
来源：http://pl.shxzukj.cn

M. 命令行 / 进程 / 环境
来源：http://uz.gzmigu.cn

================================================================================
来源：http://ja.huanxung.cn

[M01] 读取命令行参数
来源：http://oq.jctech888.com.cn

Py:   sys.argv[1:]
来源：http://fk.jctech888.com.cn

PHP:  $argv;  $argc;
来源：http://wu.panjiajie.cn

JS:   process.argv.slice(2)
来源：http://qs.haigaiapp.cn

TS:   process.argv.slice(2)
来源：http://qk.huixinmuqiang.cn

Java: args 数组（main 方法参数）
来源：http://hy.newstarts.cn

Go:   os.Args[1:]
来源：http://wu.521024.cn

Ruby: ARGV
来源：http://wp.bjjhwx.cn

C#:   args 数组（Main 方法参数）
来源：http://nw.bookmarksfly.cn

[M02] 读取环境变量
来源：http://od.521024.cn

Py:   os.environ.get("HOME")
来源：http://hf.521024.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xp.colortex.cn

JS:   process.env.HOME
来源：http://xi.521024.cn

TS:   process.env.HOME
来源：http://yt.newstarts.cn

Java: System.getenv("HOME")
来源：http://dl.gzmigu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ok.hahajie.cn

Ruby: ENV["HOME"]
来源：http://ea.panjiajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tl.shxzukj.cn

[M03] 执行外部命令
来源：http://pv.muxihuayi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://iz.jctech888.com.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lb.hnjuh.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://be.szxytkj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xw.shxzukj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://la.chemitech.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hs.yuntaijiaju.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gp.shtwfgs.cn

C#:   Process.Start("ls", "-l");
来源：http://sa.hahajie.cn

[M04] 获取当前工作目录
来源：http://qf.huixiangedu.cn

Py:   os.getcwd()
来源：http://gu.panjiajie.cn

PHP:  getcwd();
来源：http://yg.jianghongdianzi.cn

JS:   process.cwd()
来源：http://qe.huixinmuqiang.cn

TS:   process.cwd()
来源：http://zq.huixinmuqiang.cn

Java: Path.of("").toAbsolutePath()
来源：http://ud.huixiangedu.cn

Go:   os.Getwd()
来源：http://pc.hahajie.cn

Ruby: Dir.pwd
来源：http://sc.bjjhwx.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zx.hnjuh.cn

[M05] 设置退出码
来源：http://js.huixinmuqiang.cn

Py:   sys.exit(1)
来源：http://ol.9csxet.cn

PHP:  exit(1);
来源：http://qk.shxzukj.cn

JS:   process.exit(1)
来源：http://ko.szxytkj.cn

TS:   process.exit(1)
来源：http://kp.nszjky.cn

Java: System.exit(1)
来源：http://pf.muxihuayi.cn

Go:   os.Exit(1)
来源：http://mc.shxzukj.cn

Ruby: exit 1
来源：http://ir.521024.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sb.huanxung.cn

[M06] 向标准错误输出
来源：http://ev.yuntaijiaju.cn

Py:   print("err", file=sys.stderr)
来源：http://sc.521024.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ij.bookmarksfly.cn

JS:   console.error("err")
来源：http://hy.panjiajie.cn

TS:   console.error("err")
来源：http://ad.chemitech.net.cn

Java: System.err.println("err")
来源：http://ny.huixiangedu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rr.jctech888.com.cn

Ruby: warn "err"
来源：http://jw.huixiangedu.cn

C#:   Console.Error.WriteLine("err")
来源：http://mf.colortex.cn

[M07] 判断是否为主入口
来源：http://sy.jianghongdianzi.cn

Py:   if __name__ == "__main__":
来源：http://gp.muxihuayi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vg.jctech888.com.cn

JS:   require.main === module
来源：http://kf.gzmigu.cn

TS:   require.main === module
来源：http://tu.wgjwhj.cn


<!-- 参考信息 -->