代发 wailian999

Go:   time.Now()
来源：http://hx.huanxung.cn

Ruby: Time.now
来源：http://kg.asd995.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xk.szxytkj.cn

[J02] 格式化输出
来源：http://nh.bjjhwx.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ow.shxzskj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://aj.yuntaijiaju.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://aw.chemitech.net.cn

TS:   d.toISOString()
来源：http://je.panjiajie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xo.panjiajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ut.huanxung.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rg.muxihuayi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fr.bjjhwx.cn

[J03] 字符串解析为日期
来源：http://my.panjiajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ks.9csxet.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://oe.521024.cn

JS:   new Date("2024-01-02")
来源：http://aw.huanxung.cn

TS:   new Date("2024-01-02")
来源：http://hh.chemitech.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ey.hnjuh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dh.wgjwhj.cn

Ruby: Date.parse("2024-01-02")
来源：http://dk.huanxung.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xt.huixiangedu.cn

[J04] 时间戳与日期互转
来源：http://at.yuexingan06.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rj.asd995.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wu.szxytkj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sk.chemitech.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qm.colortex.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vg.9csxet.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hr.jctech888.com.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ab.lnxyls.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gg.lnxyls.cn

[J05] 时间加减（加 7 天）
来源：http://so.yuntaijiaju.cn

Py:   now + timedelta(days=7)
来源：http://im.lnxyls.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bj.hnjuh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bo.shxzskj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rl.chemitech.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://ho.jctech888.com.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tz.bjjhwx.cn

Ruby: Time.now + 7 * 86400
来源：http://em.9csxet.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gf.gzmigu.cn

[J06] 计算两时间之差
来源：http://re.nicolike.cn

Py:   (end - start).total_seconds()
来源：http://yf.szxytkj.cn

PHP:  $end->diff($start)->days;
来源：http://eb.yuntaijiaju.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ju.9csxet.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lb.huixinmuqiang.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gi.lnxyls.cn

Go:   end.Sub(start).Hours()
来源：http://lh.asd995.cn

Ruby: end - start                 # 返回秒数
来源：http://gy.yuntaijiaju.cn

C#:   (end - start).TotalSeconds
来源：http://lx.huanxung.cn

[J07] 比较两个日期
来源：http://wc.shxzskj.cn

Py:   d1 < d2;  d1 == d2
来源：http://gg.shtwfgs.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ci.wgjwhj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ii.panjiajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ca.9csxet.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://md.szxytkj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://iz.lnxyls.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mq.521024.cn

C#:   d1 < d2;  d1 == d2
来源：http://cg.hnjuh.cn

[J08] 提取年月日与星期
来源：http://az.jctech888.com.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yw.huixiangedu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vy.yuntaijiaju.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://en.bjjhwx.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pw.huanxung.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mt.haigaiapp.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rw.jctech888.com.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mb.gzmigu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bs.9csxet.cn

[J09] 时区处理
来源：http://xr.wgjwhj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lk.huixinmuqiang.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hw.asd995.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vu.panjiajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mf.shtwfgs.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dk.colortex.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ll.shtwfgs.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vq.jctech888.com.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rt.yuexingan06.cn

[J10] 取今天 / 本月第一天
来源：http://zf.gzmigu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://yl.szxytkj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://np.huixinmuqiang.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dm.jctech888.com.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sk.hahajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://we.wgjwhj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tt.yuntaijiaju.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zi.huanxung.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hs.huixiangedu.cn

================================================================================
来源：http://kx.shtwfgs.cn

K. JSON 与序列化
来源：http://hu.lnxyls.cn

================================================================================
来源：http://mw.gzmigu.cn

[K01] 对象转 JSON 字符串
来源：http://rf.newstarts.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sl.muxihuayi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mb.shtwfgs.cn

JS:   JSON.stringify(obj)
来源：http://xv.yuexingan06.cn

TS:   JSON.stringify(obj)
来源：http://qp.bjjhwx.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sn.jctech888.com.cn

Go:   json.Marshal(obj)
来源：http://sp.nszjky.cn

Ruby: obj.to_json                                     // require "json"
来源：http://tz.asd995.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jt.newstarts.cn

[K02] JSON 字符串转对象
来源：http://gz.szxytkj.cn

Py:   json.loads(s)
来源：http://zd.newstarts.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bd.huixiangedu.cn

JS:   JSON.parse(s)
来源：http://hn.jctech888.com.cn

TS:   JSON.parse(s)
来源：http://ud.bookmarksfly.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xf.wgjwhj.cn

Go:   json.Unmarshal(data, &v)
来源：http://lo.yuexingan06.cn

Ruby: JSON.parse(s)
来源：http://nx.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wi.gzmigu.cn

[K03] JSON 美化输出（带缩进）
来源：http://tg.jianghongdianzi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kv.chemitech.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lc.szxytkj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://cr.asd995.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zq.bookmarksfly.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ir.shtwfgs.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zn.jctech888.com.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ql.lnxyls.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xh.chemitech.net.cn

[K04] 读取 JSON 文件
来源：http://xm.yuexingan06.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zo.szxytkj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hy.szsharing.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hm.jctech888.com.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zn.yuexingan06.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tl.shxzskj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ni.gzmigu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fh.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cl.shtwfgs.cn

[K05] 深拷贝对象
来源：http://ww.wgjwhj.cn

Py:   copy.deepcopy(obj)
来源：http://gc.nicolike.cn

PHP:  unserialize(serialize($obj));
来源：http://mt.jianghongdianzi.cn

JS:   structuredClone(obj)
来源：http://ze.asd995.cn

TS:   structuredClone(obj)
来源：http://sk.shxzskj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ri.haigaiapp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nb.bookmarksfly.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://os.colortex.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fg.panjiajie.cn

[K06] 解析 URL 查询串
来源：http://cn.shtwfgs.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kl.bookmarksfly.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wf.nszjky.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ot.hnjuh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hm.lnxyls.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uh.huanxung.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wt.newstarts.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jl.hahajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xn.szsharing.cn

[K07] 进制转换
来源：http://pn.lnxyls.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xu.jianghongdianzi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lu.colortex.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ul.colortex.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ov.521024.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xh.szsharing.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wr.9csxet.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hi.nicolike.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kp.panjiajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://oo.jianghongdianzi.cn

Py:   pickle.dumps(obj)
来源：http://vs.huixiangedu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yx.bookmarksfly.cn

JS:   v8.serialize(obj)        // Node
来源：http://vq.yuexingan06.cn

TS:   v8.serialize(obj)        // Node
来源：http://um.haigaiapp.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pd.panjiajie.cn

Go:   encoding/gob
来源：http://xx.hnjuh.cn

Ruby: Marshal.dump(obj)
来源：http://mz.gzmigu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gl.521024.cn

================================================================================
来源：http://ya.asd995.cn

L. 网络请求
来源：http://ql.bjjhwx.cn

================================================================================
来源：http://tz.hahajie.cn

[L01] 发送 GET 请求
来源：http://do.asd995.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://su.shxzukj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://os.haigaiapp.cn

JS:   await fetch(url)
来源：http://vi.colortex.cn

TS:   await fetch(url)
来源：http://vz.haigaiapp.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pm.jianghongdianzi.cn

Go:   resp, err := http.Get(url)
来源：http://fg.jianghongdianzi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://oa.shxzukj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nx.hnjuh.cn

[L02] 发送 POST JSON
来源：http://mg.newstarts.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gk.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://we.shxzskj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fn.lnxyls.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sd.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://og.chemitech.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lf.huixiangedu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://re.bjjhwx.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bg.shxzskj.cn

[L03] 设置自定义请求头
来源：http://qj.huixiangedu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sv.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ns.yuntaijiaju.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dt.shxzskj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://db.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://se.nszjky.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://he.shxzskj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qd.gzmigu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cs.huanxung.cn

[L04] 设置超时
来源：http://hb.muxihuayi.cn

Py:   requests.get(url, timeout=5)
来源：http://fx.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ds.hnjuh.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rw.shtwfgs.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ep.chemitech.net.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://op.jctech888.com.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pb.panjiajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pg.asd995.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ds.asd995.cn

[L05] 上传文件（multipart）
来源：http://uj.lnxyls.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ke.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lm.newstarts.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kl.muxihuayi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pl.nicolike.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yz.shxzukj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://la.521024.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zk.yuexingan06.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zk.jctech888.com.cn

[L06] 解析响应为 JSON
来源：http://zr.lnxyls.cn

Py:   resp.json()
来源：http://bi.szxytkj.cn

PHP:  json_decode($body, true);
来源：http://kk.asd995.cn

JS:   await resp.json()
来源：http://tl.panjiajie.cn

TS:   await resp.json()
来源：http://tx.yuntaijiaju.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ea.panjiajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://an.huanxung.cn

Ruby: JSON.parse(resp.body)
来源：http://ku.haigaiapp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://an.jctech888.com.cn

[L07] 处理 HTTP 状态码
来源：http://eb.huixinmuqiang.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tw.asd995.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qk.shxzskj.cn

JS:   resp.ok;  resp.status
来源：http://xv.chemitech.net.cn

TS:   resp.ok;  resp.status
来源：http://ht.shtwfgs.cn

Java: resp.statusCode()
来源：http://eo.haigaiapp.cn

Go:   resp.StatusCode
来源：http://kx.huixinmuqiang.cn

Ruby: resp.code.to_i
来源：http://rt.gzmigu.cn

C#:   (int)resp.StatusCode
来源：http://si.asd995.cn

[L08] 并发请求多个地址
来源：http://pn.9csxet.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bk.yuntaijiaju.cn

PHP:  curl_multi_init() 系列
来源：http://sl.panjiajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gw.chemitech.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dt.9csxet.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yj.szxytkj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pn.nszjky.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ue.yuexingan06.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uy.9csxet.cn

================================================================================
来源：http://ap.yuexingan06.cn

M. 命令行 / 进程 / 环境
来源：http://ve.jctech888.com.cn

================================================================================
来源：http://nj.jianghongdianzi.cn

[M01] 读取命令行参数
来源：http://eh.hnjuh.cn

Py:   sys.argv[1:]
来源：http://ii.haigaiapp.cn

PHP:  $argv;  $argc;
来源：http://ob.9csxet.cn

JS:   process.argv.slice(2)
来源：http://ad.newstarts.cn

TS:   process.argv.slice(2)
来源：http://mf.521024.cn

Java: args 数组（main 方法参数）
来源：http://mz.shxzukj.cn

Go:   os.Args[1:]
来源：http://tv.521024.cn

Ruby: ARGV
来源：http://uj.panjiajie.cn

C#:   args 数组（Main 方法参数）
来源：http://xp.szsharing.cn

[M02] 读取环境变量
来源：http://nu.nicolike.cn

Py:   os.environ.get("HOME")
来源：http://bz.hahajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bd.jianghongdianzi.cn

JS:   process.env.HOME
来源：http://lz.yuntaijiaju.cn

TS:   process.env.HOME
来源：http://gt.szsharing.cn

Java: System.getenv("HOME")
来源：http://go.9csxet.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://az.colortex.cn

Ruby: ENV["HOME"]
来源：http://vo.shtwfgs.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ar.yuntaijiaju.cn

[M03] 执行外部命令
来源：http://ox.yuexingan06.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mv.shxzukj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xh.colortex.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ua.shtwfgs.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rp.huanxung.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://th.gzmigu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vz.nszjky.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ws.szsharing.cn

C#:   Process.Start("ls", "-l");
来源：http://mo.hnjuh.cn

[M04] 获取当前工作目录
来源：http://et.bookmarksfly.cn

Py:   os.getcwd()
来源：http://pe.colortex.cn

PHP:  getcwd();
来源：http://kl.huanxung.cn

JS:   process.cwd()
来源：http://of.muxihuayi.cn

TS:   process.cwd()
来源：http://zb.9csxet.cn

Java: Path.of("").toAbsolutePath()
来源：http://ac.hnjuh.cn

Go:   os.Getwd()
来源：http://ry.yuntaijiaju.cn

Ruby: Dir.pwd
来源：http://xu.nicolike.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vz.newstarts.cn

[M05] 设置退出码
来源：http://xz.huanxung.cn

Py:   sys.exit(1)
来源：http://oh.shtwfgs.cn

PHP:  exit(1);
来源：http://jo.wgjwhj.cn

JS:   process.exit(1)
来源：http://mu.newstarts.cn

TS:   process.exit(1)
来源：http://kc.shxzukj.cn

Java: System.exit(1)
来源：http://bg.huanxung.cn

Go:   os.Exit(1)
来源：http://zx.szsharing.cn

Ruby: exit 1
来源：http://ag.bjjhwx.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://go.nicolike.cn

[M06] 向标准错误输出
来源：http://qb.szxytkj.cn

Py:   print("err", file=sys.stderr)
来源：http://mx.hnjuh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rs.yuntaijiaju.cn

JS:   console.error("err")
来源：http://kd.yuntaijiaju.cn

TS:   console.error("err")
来源：http://di.muxihuayi.cn

Java: System.err.println("err")
来源：http://zf.szsharing.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kk.haigaiapp.cn

Ruby: warn "err"
来源：http://pu.shtwfgs.cn

C#:   Console.Error.WriteLine("err")
来源：http://rz.huixinmuqiang.cn

[M07] 判断是否为主入口
来源：http://oa.chemitech.net.cn

Py:   if __name__ == "__main__":
来源：http://dl.yuntaijiaju.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qh.9csxet.cn

JS:   require.main === module
来源：http://yl.szsharing.cn

TS:   require.main === module
来源：http://no.lnxyls.cn

Java: public static void main(String[] args)
来源：http://mz.muxihuayi.cn

Go:   func main()
来源：http://jm.nszjky.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qy.colortex.cn

C#:   static void Main(string[] args)
来源：http://cb.jianghongdianzi.cn


<!-- 参考信息 -->