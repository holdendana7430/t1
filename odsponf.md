代发 wailian999

Go:   time.Now()
来源：http://uv.shtwfgs.cn

Ruby: Time.now
来源：http://sn.panjiajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ka.chemitech.net.cn

[J02] 格式化输出
来源：http://mp.hnjuh.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hp.9csxet.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sg.jctech888.com.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gd.panjiajie.cn

TS:   d.toISOString()
来源：http://rg.bjjhwx.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ci.9csxet.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hv.lnxyls.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bg.panjiajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lr.hahajie.cn

[J03] 字符串解析为日期
来源：http://jm.jianghongdianzi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qa.nszjky.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ur.wgjwhj.cn

JS:   new Date("2024-01-02")
来源：http://pc.wgjwhj.cn

TS:   new Date("2024-01-02")
来源：http://af.haigaiapp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rk.hnjuh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ne.huixiangedu.cn

Ruby: Date.parse("2024-01-02")
来源：http://hb.9csxet.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pb.hnjuh.cn

[J04] 时间戳与日期互转
来源：http://br.newstarts.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vp.huixiangedu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yb.huanxung.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fk.nszjky.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hw.shtwfgs.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ga.newstarts.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sk.nszjky.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cd.lnxyls.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jz.asd995.cn

[J05] 时间加减（加 7 天）
来源：http://ky.colortex.cn

Py:   now + timedelta(days=7)
来源：http://gk.szxytkj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lw.szxytkj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ek.haigaiapp.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xu.huixinmuqiang.cn

Java: LocalDate.now().plusDays(7)
来源：http://iv.huanxung.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zp.chemitech.net.cn

Ruby: Time.now + 7 * 86400
来源：http://qi.huixinmuqiang.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ov.jctech888.com.cn

[J06] 计算两时间之差
来源：http://ov.bjjhwx.cn

Py:   (end - start).total_seconds()
来源：http://vx.shtwfgs.cn

PHP:  $end->diff($start)->days;
来源：http://rh.9csxet.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qy.newstarts.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sb.lnxyls.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ur.bjjhwx.cn

Go:   end.Sub(start).Hours()
来源：http://qs.shtwfgs.cn

Ruby: end - start                 # 返回秒数
来源：http://bu.lnxyls.cn

C#:   (end - start).TotalSeconds
来源：http://ts.nicolike.cn

[J07] 比较两个日期
来源：http://qp.lnxyls.cn

Py:   d1 < d2;  d1 == d2
来源：http://sv.chemitech.net.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sb.hahajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kt.shxzskj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://wl.jianghongdianzi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uw.chemitech.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ok.jianghongdianzi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hj.huanxung.cn

C#:   d1 < d2;  d1 == d2
来源：http://ha.panjiajie.cn

[J08] 提取年月日与星期
来源：http://ax.521024.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pq.newstarts.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gv.szsharing.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://px.huixiangedu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oa.jctech888.com.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jh.nszjky.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xn.muxihuayi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fc.hnjuh.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kl.yuntaijiaju.cn

[J09] 时区处理
来源：http://rp.huixiangedu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ui.muxihuayi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pm.521024.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ox.gzmigu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mi.huixiangedu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bm.shxzukj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pv.yuexingan06.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://da.shxzukj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kq.szxytkj.cn

[J10] 取今天 / 本月第一天
来源：http://np.yuntaijiaju.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://mp.shxzukj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xb.huixinmuqiang.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ne.huixiangedu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qp.yuntaijiaju.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qr.shtwfgs.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wc.huixiangedu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dm.nicolike.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bx.lnxyls.cn

================================================================================
来源：http://or.shtwfgs.cn

K. JSON 与序列化
来源：http://pv.hnjuh.cn

================================================================================
来源：http://ti.shxzukj.cn

[K01] 对象转 JSON 字符串
来源：http://tz.colortex.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lb.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hv.chemitech.net.cn

JS:   JSON.stringify(obj)
来源：http://xv.huanxung.cn

TS:   JSON.stringify(obj)
来源：http://ei.jianghongdianzi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kx.9csxet.cn

Go:   json.Marshal(obj)
来源：http://vj.yuexingan06.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mg.nszjky.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qk.panjiajie.cn

[K02] JSON 字符串转对象
来源：http://mt.szsharing.cn

Py:   json.loads(s)
来源：http://wd.yuexingan06.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uf.nszjky.cn

JS:   JSON.parse(s)
来源：http://uz.newstarts.cn

TS:   JSON.parse(s)
来源：http://vw.yuntaijiaju.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ph.yuexingan06.cn

Go:   json.Unmarshal(data, &v)
来源：http://mh.huixiangedu.cn

Ruby: JSON.parse(s)
来源：http://ny.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ef.nszjky.cn

[K03] JSON 美化输出（带缩进）
来源：http://sc.nszjky.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ze.bookmarksfly.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://oq.bookmarksfly.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ld.bjjhwx.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ww.yuexingan06.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nt.nicolike.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://de.haigaiapp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wc.lnxyls.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ve.szsharing.cn

[K04] 读取 JSON 文件
来源：http://wv.lnxyls.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sf.shxzukj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sm.haigaiapp.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qa.colortex.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vx.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://iw.nicolike.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hu.jianghongdianzi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mx.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kt.szxytkj.cn

[K05] 深拷贝对象
来源：http://tc.asd995.cn

Py:   copy.deepcopy(obj)
来源：http://fn.huixinmuqiang.cn

PHP:  unserialize(serialize($obj));
来源：http://qn.lnxyls.cn

JS:   structuredClone(obj)
来源：http://re.hahajie.cn

TS:   structuredClone(obj)
来源：http://kr.521024.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://to.gzmigu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qh.haigaiapp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uh.huanxung.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gm.muxihuayi.cn

[K06] 解析 URL 查询串
来源：http://rx.shxzukj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jm.hnjuh.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://my.yuntaijiaju.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tk.jctech888.com.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vq.haigaiapp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mk.shxzukj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fg.colortex.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nm.haigaiapp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ai.lnxyls.cn

[K07] 进制转换
来源：http://ld.shxzukj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://by.huixinmuqiang.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nv.jctech888.com.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hh.nicolike.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hg.wgjwhj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pm.bookmarksfly.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vz.521024.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ci.nszjky.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://la.asd995.cn

[K08] 二进制序列化（非 JSON）
来源：http://ou.muxihuayi.cn

Py:   pickle.dumps(obj)
来源：http://kb.huixiangedu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ti.haigaiapp.cn

JS:   v8.serialize(obj)        // Node
来源：http://hn.jctech888.com.cn

TS:   v8.serialize(obj)        // Node
来源：http://ts.huixinmuqiang.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ir.lnxyls.cn

Go:   encoding/gob
来源：http://vw.szsharing.cn

Ruby: Marshal.dump(obj)
来源：http://xz.yuntaijiaju.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yo.hnjuh.cn

================================================================================
来源：http://op.jctech888.com.cn

L. 网络请求
来源：http://ri.asd995.cn

================================================================================
来源：http://of.nszjky.cn

[L01] 发送 GET 请求
来源：http://ut.wgjwhj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://co.asd995.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cc.gzmigu.cn

JS:   await fetch(url)
来源：http://qu.muxihuayi.cn

TS:   await fetch(url)
来源：http://nx.huanxung.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rz.wgjwhj.cn

Go:   resp, err := http.Get(url)
来源：http://rj.muxihuayi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ml.haigaiapp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sq.huixiangedu.cn

[L02] 发送 POST JSON
来源：http://ln.hahajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hn.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://oh.shxzukj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xk.shxzskj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://no.asd995.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yu.hahajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zi.huixinmuqiang.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dw.gzmigu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zg.huixinmuqiang.cn

[L03] 设置自定义请求头
来源：http://ej.shtwfgs.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sa.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wx.newstarts.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dw.9csxet.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jb.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mj.szsharing.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lt.panjiajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zo.lnxyls.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gp.nicolike.cn

[L04] 设置超时
来源：http://ev.chemitech.net.cn

Py:   requests.get(url, timeout=5)
来源：http://xn.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hv.yuntaijiaju.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qs.521024.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rt.asd995.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qo.nicolike.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nx.colortex.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wc.muxihuayi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zl.szxytkj.cn

[L05] 上传文件（multipart）
来源：http://gw.9csxet.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dq.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ea.asd995.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://aa.jianghongdianzi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://go.huixinmuqiang.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gg.asd995.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ho.yuntaijiaju.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ow.nicolike.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uv.huixinmuqiang.cn

[L06] 解析响应为 JSON
来源：http://ua.asd995.cn

Py:   resp.json()
来源：http://zp.bookmarksfly.cn

PHP:  json_decode($body, true);
来源：http://gh.nicolike.cn

JS:   await resp.json()
来源：http://mo.wgjwhj.cn

TS:   await resp.json()
来源：http://sm.yuntaijiaju.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ci.hahajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gl.nszjky.cn

Ruby: JSON.parse(resp.body)
来源：http://ht.szxytkj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://az.muxihuayi.cn

[L07] 处理 HTTP 状态码
来源：http://gp.szsharing.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fe.huanxung.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ex.jctech888.com.cn

JS:   resp.ok;  resp.status
来源：http://uv.shxzukj.cn

TS:   resp.ok;  resp.status
来源：http://qt.szsharing.cn

Java: resp.statusCode()
来源：http://ba.muxihuayi.cn

Go:   resp.StatusCode
来源：http://zp.jianghongdianzi.cn

Ruby: resp.code.to_i
来源：http://zl.nicolike.cn

C#:   (int)resp.StatusCode
来源：http://yj.szxytkj.cn

[L08] 并发请求多个地址
来源：http://nq.muxihuayi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uy.shxzukj.cn

PHP:  curl_multi_init() 系列
来源：http://ri.newstarts.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bq.shxzukj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gk.colortex.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://oa.shtwfgs.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tm.shtwfgs.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cn.huixinmuqiang.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pp.yuexingan06.cn

================================================================================
来源：http://jw.haigaiapp.cn

M. 命令行 / 进程 / 环境
来源：http://se.jianghongdianzi.cn

================================================================================
来源：http://od.szsharing.cn

[M01] 读取命令行参数
来源：http://kv.yuexingan06.cn

Py:   sys.argv[1:]
来源：http://fh.bjjhwx.cn

PHP:  $argv;  $argc;
来源：http://vr.yuexingan06.cn

JS:   process.argv.slice(2)
来源：http://to.szsharing.cn

TS:   process.argv.slice(2)
来源：http://fi.lnxyls.cn

Java: args 数组（main 方法参数）
来源：http://px.chemitech.net.cn

Go:   os.Args[1:]
来源：http://mu.panjiajie.cn

Ruby: ARGV
来源：http://sv.yuntaijiaju.cn

C#:   args 数组（Main 方法参数）
来源：http://qn.bjjhwx.cn

[M02] 读取环境变量
来源：http://my.szxytkj.cn

Py:   os.environ.get("HOME")
来源：http://gw.hnjuh.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hh.bjjhwx.cn

JS:   process.env.HOME
来源：http://lt.shtwfgs.cn

TS:   process.env.HOME
来源：http://rq.haigaiapp.cn

Java: System.getenv("HOME")
来源：http://di.huanxung.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cp.9csxet.cn

Ruby: ENV["HOME"]
来源：http://vj.shxzukj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qp.bookmarksfly.cn

[M03] 执行外部命令
来源：http://bg.huixinmuqiang.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://go.szsharing.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zk.chemitech.net.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ht.wgjwhj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gk.hahajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jj.wgjwhj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ph.nszjky.cn

Ruby: system("ls -l");  `ls -l`
来源：http://eg.nicolike.cn

C#:   Process.Start("ls", "-l");
来源：http://gu.chemitech.net.cn

[M04] 获取当前工作目录
来源：http://qd.huixinmuqiang.cn

Py:   os.getcwd()
来源：http://pu.asd995.cn

PHP:  getcwd();
来源：http://tn.haigaiapp.cn

JS:   process.cwd()
来源：http://ug.nszjky.cn

TS:   process.cwd()
来源：http://gn.muxihuayi.cn

Java: Path.of("").toAbsolutePath()
来源：http://kh.hnjuh.cn

Go:   os.Getwd()
来源：http://xi.9csxet.cn

Ruby: Dir.pwd
来源：http://lu.nicolike.cn

C#:   Directory.GetCurrentDirectory()
来源：http://aj.gzmigu.cn

[M05] 设置退出码
来源：http://sn.panjiajie.cn

Py:   sys.exit(1)
来源：http://xn.nicolike.cn

PHP:  exit(1);
来源：http://tf.yuntaijiaju.cn

JS:   process.exit(1)
来源：http://ry.huixinmuqiang.cn

TS:   process.exit(1)
来源：http://kr.jctech888.com.cn

Java: System.exit(1)
来源：http://xv.yuntaijiaju.cn

Go:   os.Exit(1)
来源：http://lg.jianghongdianzi.cn

Ruby: exit 1
来源：http://vk.9csxet.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bo.9csxet.cn

[M06] 向标准错误输出
来源：http://yb.lnxyls.cn

Py:   print("err", file=sys.stderr)
来源：http://pq.wgjwhj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pz.jianghongdianzi.cn

JS:   console.error("err")
来源：http://fb.521024.cn

TS:   console.error("err")
来源：http://np.shxzskj.cn

Java: System.err.println("err")
来源：http://vh.shtwfgs.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tw.hnjuh.cn

Ruby: warn "err"
来源：http://fs.szxytkj.cn

C#:   Console.Error.WriteLine("err")
来源：http://ld.jianghongdianzi.cn

[M07] 判断是否为主入口
来源：http://bz.muxihuayi.cn

Py:   if __name__ == "__main__":
来源：http://mx.gzmigu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kt.521024.cn

JS:   require.main === module
来源：http://wp.hnjuh.cn

TS:   require.main === module
来源：http://ew.szxytkj.cn

Java: public static void main(String[] args)
来源：http://lc.haigaiapp.cn

Go:   func main()
来源：http://nm.szsharing.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jw.jctech888.com.cn

C#:   static void Main(string[] args)
来源：http://cu.muxihuayi.cn


<!-- 参考信息 -->