代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://im.newstarts.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bt.nszjky.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kq.bookmarksfly.cn

TS:   d.toISOString()
来源：http://yj.huixiangedu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pl.szsharing.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hd.9csxet.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qo.huanxung.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://en.lnxyls.cn

[J03] 字符串解析为日期
来源：http://uf.colortex.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://us.gzmigu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lm.shxzukj.cn

JS:   new Date("2024-01-02")
来源：http://yj.jianghongdianzi.cn

TS:   new Date("2024-01-02")
来源：http://xx.szxytkj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://on.shxzukj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uy.panjiajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://pu.nszjky.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gr.jctech888.com.cn

[J04] 时间戳与日期互转
来源：http://li.huixinmuqiang.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qz.jctech888.com.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ha.bjjhwx.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qb.nicolike.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zg.bjjhwx.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nd.hnjuh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fs.asd995.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.gzmigu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://al.colortex.cn

[J05] 时间加减（加 7 天）
来源：http://bm.newstarts.cn

Py:   now + timedelta(days=7)
来源：http://tj.9csxet.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vu.shxzukj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uy.haigaiapp.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://av.jianghongdianzi.cn

Java: LocalDate.now().plusDays(7)
来源：http://fg.haigaiapp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uf.huixiangedu.cn

Ruby: Time.now + 7 * 86400
来源：http://zl.szxytkj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gu.muxihuayi.cn

[J06] 计算两时间之差
来源：http://zx.colortex.cn

Py:   (end - start).total_seconds()
来源：http://wb.huixiangedu.cn

PHP:  $end->diff($start)->days;
来源：http://vc.yuexingan06.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yq.yuexingan06.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mn.lnxyls.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ay.jianghongdianzi.cn

Go:   end.Sub(start).Hours()
来源：http://cj.hahajie.cn

Ruby: end - start                 # 返回秒数
来源：http://dt.yuntaijiaju.cn

C#:   (end - start).TotalSeconds
来源：http://ei.shxzukj.cn

[J07] 比较两个日期
来源：http://xw.shxzukj.cn

Py:   d1 < d2;  d1 == d2
来源：http://xr.nicolike.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wg.bjjhwx.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kg.yuexingan06.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yx.nicolike.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zq.nicolike.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xc.gzmigu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qh.shxzskj.cn

C#:   d1 < d2;  d1 == d2
来源：http://yb.521024.cn

[J08] 提取年月日与星期
来源：http://bf.chemitech.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ae.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pp.panjiajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://th.chemitech.net.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vw.asd995.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pc.szsharing.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://se.gzmigu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qc.yuntaijiaju.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yp.shtwfgs.cn

[J09] 时区处理
来源：http://eo.muxihuayi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uo.shxzukj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ak.haigaiapp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ub.panjiajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cq.panjiajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xq.bjjhwx.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hj.yuexingan06.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fp.shxzskj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ig.yuexingan06.cn

[J10] 取今天 / 本月第一天
来源：http://me.nicolike.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jp.asd995.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rc.shtwfgs.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jy.gzmigu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dn.panjiajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lo.yuntaijiaju.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ox.hnjuh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wc.gzmigu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kd.hahajie.cn

================================================================================
来源：http://vd.jctech888.com.cn

K. JSON 与序列化
来源：http://wf.haigaiapp.cn

================================================================================
来源：http://cl.jianghongdianzi.cn

[K01] 对象转 JSON 字符串
来源：http://hg.colortex.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pr.panjiajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ed.newstarts.cn

JS:   JSON.stringify(obj)
来源：http://oc.hnjuh.cn

TS:   JSON.stringify(obj)
来源：http://pj.jctech888.com.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hn.lnxyls.cn

Go:   json.Marshal(obj)
来源：http://im.szsharing.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wc.9csxet.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dd.521024.cn

[K02] JSON 字符串转对象
来源：http://ho.huixinmuqiang.cn

Py:   json.loads(s)
来源：http://jt.yuexingan06.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wa.521024.cn

JS:   JSON.parse(s)
来源：http://yw.colortex.cn

TS:   JSON.parse(s)
来源：http://kd.shtwfgs.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://oy.szsharing.cn

Go:   json.Unmarshal(data, &v)
来源：http://zx.szsharing.cn

Ruby: JSON.parse(s)
来源：http://qo.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cp.szsharing.cn

[K03] JSON 美化输出（带缩进）
来源：http://vt.muxihuayi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ch.huixiangedu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ih.jianghongdianzi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://oj.asd995.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yk.yuexingan06.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ex.nicolike.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pd.hahajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ah.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rk.asd995.cn

[K04] 读取 JSON 文件
来源：http://fx.nszjky.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ox.shxzskj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ow.colortex.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mr.bookmarksfly.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wu.shxzukj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gu.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lt.huanxung.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ce.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nl.bjjhwx.cn

[K05] 深拷贝对象
来源：http://gk.huixinmuqiang.cn

Py:   copy.deepcopy(obj)
来源：http://dw.panjiajie.cn

PHP:  unserialize(serialize($obj));
来源：http://hi.panjiajie.cn

JS:   structuredClone(obj)
来源：http://vs.hahajie.cn

TS:   structuredClone(obj)
来源：http://js.haigaiapp.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kh.newstarts.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rn.nicolike.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sn.asd995.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hj.jctech888.com.cn

[K06] 解析 URL 查询串
来源：http://qa.jctech888.com.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ta.gzmigu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jz.jianghongdianzi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oj.shtwfgs.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ql.nszjky.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sa.shxzukj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ku.yuntaijiaju.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bd.yuntaijiaju.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://na.szxytkj.cn

[K07] 进制转换
来源：http://tf.hahajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vj.colortex.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wu.shxzukj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qp.muxihuayi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bj.hnjuh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qd.yuexingan06.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zu.gzmigu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rg.shtwfgs.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lw.9csxet.cn

[K08] 二进制序列化（非 JSON）
来源：http://ha.521024.cn

Py:   pickle.dumps(obj)
来源：http://xk.huanxung.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hh.shtwfgs.cn

JS:   v8.serialize(obj)        // Node
来源：http://or.gzmigu.cn

TS:   v8.serialize(obj)        // Node
来源：http://nc.yuexingan06.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uc.wgjwhj.cn

Go:   encoding/gob
来源：http://au.521024.cn

Ruby: Marshal.dump(obj)
来源：http://qf.muxihuayi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vx.yuntaijiaju.cn

================================================================================
来源：http://zc.jctech888.com.cn

L. 网络请求
来源：http://gi.szsharing.cn

================================================================================
来源：http://xw.panjiajie.cn

[L01] 发送 GET 请求
来源：http://nu.521024.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ak.yuntaijiaju.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ii.huixiangedu.cn

JS:   await fetch(url)
来源：http://bw.jctech888.com.cn

TS:   await fetch(url)
来源：http://ej.yuntaijiaju.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://je.bjjhwx.cn

Go:   resp, err := http.Get(url)
来源：http://zg.jctech888.com.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bp.shtwfgs.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nc.chemitech.net.cn

[L02] 发送 POST JSON
来源：http://hp.huanxung.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hx.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qi.huanxung.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wb.bookmarksfly.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iw.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mg.hnjuh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fe.panjiajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ht.panjiajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ff.yuexingan06.cn

[L03] 设置自定义请求头
来源：http://zi.asd995.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ew.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qs.huixinmuqiang.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gm.jianghongdianzi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cw.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://if.huixiangedu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cc.szxytkj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ez.jctech888.com.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ga.wgjwhj.cn

[L04] 设置超时
来源：http://ae.huixiangedu.cn

Py:   requests.get(url, timeout=5)
来源：http://fz.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bf.huanxung.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ty.chemitech.net.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fz.9csxet.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gx.nszjky.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hl.colortex.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jz.haigaiapp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yk.newstarts.cn

[L05] 上传文件（multipart）
来源：http://jd.szsharing.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://iw.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ha.muxihuayi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vs.chemitech.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wp.lnxyls.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nb.521024.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jt.szxytkj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ru.colortex.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kz.szsharing.cn

[L06] 解析响应为 JSON
来源：http://ng.huixiangedu.cn

Py:   resp.json()
来源：http://ex.szsharing.cn

PHP:  json_decode($body, true);
来源：http://lo.yuntaijiaju.cn

JS:   await resp.json()
来源：http://us.newstarts.cn

TS:   await resp.json()
来源：http://xi.yuntaijiaju.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jo.shxzskj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dm.jianghongdianzi.cn

Ruby: JSON.parse(resp.body)
来源：http://ul.huixiangedu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hl.huixiangedu.cn

[L07] 处理 HTTP 状态码
来源：http://gm.huixinmuqiang.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rb.asd995.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fc.nicolike.cn

JS:   resp.ok;  resp.status
来源：http://mn.hahajie.cn

TS:   resp.ok;  resp.status
来源：http://pt.szxytkj.cn

Java: resp.statusCode()
来源：http://bk.szxytkj.cn

Go:   resp.StatusCode
来源：http://ri.wgjwhj.cn

Ruby: resp.code.to_i
来源：http://hb.colortex.cn

C#:   (int)resp.StatusCode
来源：http://cq.jctech888.com.cn

[L08] 并发请求多个地址
来源：http://np.huixinmuqiang.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lg.shtwfgs.cn

PHP:  curl_multi_init() 系列
来源：http://xv.hnjuh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wd.wgjwhj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://by.shxzskj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://di.shxzskj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vp.szsharing.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lc.yuntaijiaju.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qi.huixiangedu.cn

================================================================================
来源：http://fr.newstarts.cn

M. 命令行 / 进程 / 环境
来源：http://us.jctech888.com.cn

================================================================================
来源：http://ba.hnjuh.cn

[M01] 读取命令行参数
来源：http://fb.wgjwhj.cn

Py:   sys.argv[1:]
来源：http://zo.bjjhwx.cn

PHP:  $argv;  $argc;
来源：http://hn.colortex.cn

JS:   process.argv.slice(2)
来源：http://hq.yuexingan06.cn

TS:   process.argv.slice(2)
来源：http://ui.szxytkj.cn

Java: args 数组（main 方法参数）
来源：http://kz.shtwfgs.cn

Go:   os.Args[1:]
来源：http://xe.9csxet.cn

Ruby: ARGV
来源：http://gw.hnjuh.cn

C#:   args 数组（Main 方法参数）
来源：http://cn.wgjwhj.cn

[M02] 读取环境变量
来源：http://cp.jctech888.com.cn

Py:   os.environ.get("HOME")
来源：http://gg.haigaiapp.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cy.shtwfgs.cn

JS:   process.env.HOME
来源：http://ah.521024.cn

TS:   process.env.HOME
来源：http://ci.szsharing.cn

Java: System.getenv("HOME")
来源：http://gl.nszjky.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jv.hahajie.cn

Ruby: ENV["HOME"]
来源：http://vk.wgjwhj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gd.shxzukj.cn

[M03] 执行外部命令
来源：http://mb.chemitech.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ix.huixiangedu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://se.lnxyls.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://yp.hnjuh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nu.newstarts.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mb.jctech888.com.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://je.colortex.cn

Ruby: system("ls -l");  `ls -l`
来源：http://di.hnjuh.cn

C#:   Process.Start("ls", "-l");
来源：http://mp.bjjhwx.cn

[M04] 获取当前工作目录
来源：http://yb.hnjuh.cn

Py:   os.getcwd()
来源：http://ef.bookmarksfly.cn

PHP:  getcwd();
来源：http://mg.chemitech.net.cn

JS:   process.cwd()
来源：http://sb.hahajie.cn

TS:   process.cwd()
来源：http://os.shtwfgs.cn

Java: Path.of("").toAbsolutePath()
来源：http://ff.jianghongdianzi.cn

Go:   os.Getwd()
来源：http://ow.haigaiapp.cn

Ruby: Dir.pwd
来源：http://vw.jctech888.com.cn

C#:   Directory.GetCurrentDirectory()
来源：http://fk.lnxyls.cn

[M05] 设置退出码
来源：http://gt.chemitech.net.cn

Py:   sys.exit(1)
来源：http://cc.wgjwhj.cn

PHP:  exit(1);
来源：http://qz.lnxyls.cn

JS:   process.exit(1)
来源：http://oe.lnxyls.cn

TS:   process.exit(1)
来源：http://ua.panjiajie.cn

Java: System.exit(1)
来源：http://nd.huixinmuqiang.cn

Go:   os.Exit(1)
来源：http://qh.haigaiapp.cn

Ruby: exit 1
来源：http://jg.haigaiapp.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dq.lnxyls.cn

[M06] 向标准错误输出
来源：http://mx.521024.cn

Py:   print("err", file=sys.stderr)
来源：http://ph.bjjhwx.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pw.panjiajie.cn

JS:   console.error("err")
来源：http://zv.521024.cn

TS:   console.error("err")
来源：http://kt.huixinmuqiang.cn

Java: System.err.println("err")
来源：http://ni.huixiangedu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rk.szxytkj.cn

Ruby: warn "err"
来源：http://fa.hahajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://mr.haigaiapp.cn

[M07] 判断是否为主入口
来源：http://iz.huixinmuqiang.cn

Py:   if __name__ == "__main__":
来源：http://kj.panjiajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.chemitech.net.cn

JS:   require.main === module
来源：http://va.yuexingan06.cn

TS:   require.main === module
来源：http://lc.bjjhwx.cn

Java: public static void main(String[] args)
来源：http://fb.panjiajie.cn

Go:   func main()
来源：http://ku.yuntaijiaju.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pg.shxzukj.cn

C#:   static void Main(string[] args)
来源：http://sl.asd995.cn

[M08] 获取系统与运行时信息
来源：http://iu.shxzukj.cn

Py:   platform.system();  platform.python_version()
来源：http://qh.haigaiapp.cn

PHP:  PHP_OS;  phpversion();
来源：http://tf.9csxet.cn

JS:   process.platform;  process.version
来源：http://pu.huixinmuqiang.cn


<!-- 参考信息 -->