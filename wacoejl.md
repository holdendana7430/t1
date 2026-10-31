代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zj.newstarts.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://il.jctech888.com.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ci.szsharing.cn

TS:   d.toISOString()
来源：http://qd.panjiajie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pz.nicolike.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ry.szxytkj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ax.huixinmuqiang.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yp.nszjky.cn

[J03] 字符串解析为日期
来源：http://al.huanxung.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://es.huixiangedu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fb.gzmigu.cn

JS:   new Date("2024-01-02")
来源：http://nd.yuexingan06.cn

TS:   new Date("2024-01-02")
来源：http://vk.haigaiapp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://tz.jianghongdianzi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mr.gzmigu.cn

Ruby: Date.parse("2024-01-02")
来源：http://nj.panjiajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://on.panjiajie.cn

[J04] 时间戳与日期互转
来源：http://el.haigaiapp.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nd.hahajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.nicolike.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://me.wgjwhj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gt.huixinmuqiang.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://af.asd995.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ub.haigaiapp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ir.szsharing.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tm.hnjuh.cn

[J05] 时间加减（加 7 天）
来源：http://af.huixinmuqiang.cn

Py:   now + timedelta(days=7)
来源：http://hd.shxzskj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://tv.shxzskj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tf.gzmigu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kk.gzmigu.cn

Java: LocalDate.now().plusDays(7)
来源：http://uy.szsharing.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://er.nszjky.cn

Ruby: Time.now + 7 * 86400
来源：http://fb.nszjky.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ms.shxzukj.cn

[J06] 计算两时间之差
来源：http://tn.hnjuh.cn

Py:   (end - start).total_seconds()
来源：http://dy.huixinmuqiang.cn

PHP:  $end->diff($start)->days;
来源：http://ig.jctech888.com.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yl.szsharing.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wy.jianghongdianzi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://tj.hnjuh.cn

Go:   end.Sub(start).Hours()
来源：http://kv.nicolike.cn

Ruby: end - start                 # 返回秒数
来源：http://eh.9csxet.cn

C#:   (end - start).TotalSeconds
来源：http://at.newstarts.cn

[J07] 比较两个日期
来源：http://zk.panjiajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://ya.shxzskj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qm.hnjuh.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hm.521024.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yy.newstarts.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ez.panjiajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uj.szxytkj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xa.szsharing.cn

C#:   d1 < d2;  d1 == d2
来源：http://ao.yuexingan06.cn

[J08] 提取年月日与星期
来源：http://uc.jctech888.com.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kb.haigaiapp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wi.9csxet.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://he.panjiajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nn.huixiangedu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://na.colortex.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hu.haigaiapp.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wp.hahajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://in.hnjuh.cn

[J09] 时区处理
来源：http://mn.jctech888.com.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nl.asd995.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qz.nicolike.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qb.hahajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vp.colortex.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cs.szsharing.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://je.nszjky.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://je.jctech888.com.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hg.hnjuh.cn

[J10] 取今天 / 本月第一天
来源：http://bx.colortex.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://yu.bookmarksfly.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pc.hahajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://no.huanxung.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vn.nszjky.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mw.gzmigu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hg.gzmigu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pz.521024.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xi.521024.cn

================================================================================
来源：http://pi.jctech888.com.cn

K. JSON 与序列化
来源：http://ww.huanxung.cn

================================================================================
来源：http://fz.panjiajie.cn

[K01] 对象转 JSON 字符串
来源：http://cj.jctech888.com.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kd.muxihuayi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lv.huixiangedu.cn

JS:   JSON.stringify(obj)
来源：http://xv.haigaiapp.cn

TS:   JSON.stringify(obj)
来源：http://vs.huanxung.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gk.shtwfgs.cn

Go:   json.Marshal(obj)
来源：http://wc.haigaiapp.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xn.newstarts.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jv.yuntaijiaju.cn

[K02] JSON 字符串转对象
来源：http://kx.hnjuh.cn

Py:   json.loads(s)
来源：http://xm.huixinmuqiang.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kv.yuntaijiaju.cn

JS:   JSON.parse(s)
来源：http://br.jianghongdianzi.cn

TS:   JSON.parse(s)
来源：http://pj.haigaiapp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ya.521024.cn

Go:   json.Unmarshal(data, &v)
来源：http://yy.newstarts.cn

Ruby: JSON.parse(s)
来源：http://gb.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uw.nszjky.cn

[K03] JSON 美化输出（带缩进）
来源：http://au.521024.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tk.shtwfgs.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yk.shtwfgs.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jn.shxzukj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ob.lnxyls.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vf.huixiangedu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jp.gzmigu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rb.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://og.hahajie.cn

[K04] 读取 JSON 文件
来源：http://il.shxzskj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dw.colortex.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gr.muxihuayi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jn.nszjky.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ys.muxihuayi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jg.shxzukj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ro.haigaiapp.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hc.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uj.colortex.cn

[K05] 深拷贝对象
来源：http://ch.shxzskj.cn

Py:   copy.deepcopy(obj)
来源：http://yk.521024.cn

PHP:  unserialize(serialize($obj));
来源：http://jk.szsharing.cn

JS:   structuredClone(obj)
来源：http://wo.wgjwhj.cn

TS:   structuredClone(obj)
来源：http://ne.jianghongdianzi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://by.9csxet.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dy.hahajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cd.shtwfgs.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xn.shxzukj.cn

[K06] 解析 URL 查询串
来源：http://ne.shtwfgs.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://td.wgjwhj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ar.huixiangedu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ve.wgjwhj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://me.nicolike.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zk.jctech888.com.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://to.muxihuayi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mn.panjiajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wq.huixinmuqiang.cn

[K07] 进制转换
来源：http://hl.asd995.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xg.wgjwhj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qr.hahajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tl.hahajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xl.muxihuayi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cd.haigaiapp.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tb.colortex.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yuexingan06.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ly.hnjuh.cn

[K08] 二进制序列化（非 JSON）
来源：http://ka.chemitech.net.cn

Py:   pickle.dumps(obj)
来源：http://ra.chemitech.net.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ms.jianghongdianzi.cn

JS:   v8.serialize(obj)        // Node
来源：http://bq.hnjuh.cn

TS:   v8.serialize(obj)        // Node
来源：http://ec.newstarts.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vt.colortex.cn

Go:   encoding/gob
来源：http://re.colortex.cn

Ruby: Marshal.dump(obj)
来源：http://jm.shxzskj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jb.9csxet.cn

================================================================================
来源：http://il.shtwfgs.cn

L. 网络请求
来源：http://zr.yuexingan06.cn

================================================================================
来源：http://by.hnjuh.cn

[L01] 发送 GET 请求
来源：http://uo.yuexingan06.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kr.szsharing.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://td.hahajie.cn

JS:   await fetch(url)
来源：http://pv.huixinmuqiang.cn

TS:   await fetch(url)
来源：http://xl.shxzskj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yf.yuntaijiaju.cn

Go:   resp, err := http.Get(url)
来源：http://pi.gzmigu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xg.chemitech.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lg.huanxung.cn

[L02] 发送 POST JSON
来源：http://fi.yuntaijiaju.cn

Py:   requests.post(url, json={"a": 1})
来源：http://od.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bh.newstarts.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ro.yuexingan06.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zc.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jr.yuntaijiaju.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bj.bjjhwx.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nl.shxzukj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vh.asd995.cn

[L03] 设置自定义请求头
来源：http://rq.huanxung.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ec.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tm.gzmigu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sq.shxzukj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wv.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kj.haigaiapp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://eo.asd995.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mc.chemitech.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ji.bjjhwx.cn

[L04] 设置超时
来源：http://zd.huanxung.cn

Py:   requests.get(url, timeout=5)
来源：http://av.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yl.lnxyls.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ak.colortex.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dy.haigaiapp.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://as.jctech888.com.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kb.nicolike.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hq.asd995.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yi.shtwfgs.cn

[L05] 上传文件（multipart）
来源：http://al.yuexingan06.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fg.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jb.muxihuayi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sg.yuexingan06.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lb.shtwfgs.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pp.yuntaijiaju.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kn.huixiangedu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wq.lnxyls.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://og.jctech888.com.cn

[L06] 解析响应为 JSON
来源：http://cf.bjjhwx.cn

Py:   resp.json()
来源：http://qq.521024.cn

PHP:  json_decode($body, true);
来源：http://nt.gzmigu.cn

JS:   await resp.json()
来源：http://tn.jianghongdianzi.cn

TS:   await resp.json()
来源：http://bv.newstarts.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uk.521024.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://em.9csxet.cn

Ruby: JSON.parse(resp.body)
来源：http://vi.9csxet.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mt.hahajie.cn

[L07] 处理 HTTP 状态码
来源：http://ic.panjiajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ay.huanxung.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jv.panjiajie.cn

JS:   resp.ok;  resp.status
来源：http://ev.colortex.cn

TS:   resp.ok;  resp.status
来源：http://gl.521024.cn

Java: resp.statusCode()
来源：http://zt.newstarts.cn

Go:   resp.StatusCode
来源：http://kg.szsharing.cn

Ruby: resp.code.to_i
来源：http://po.shxzskj.cn

C#:   (int)resp.StatusCode
来源：http://hi.bjjhwx.cn

[L08] 并发请求多个地址
来源：http://hi.gzmigu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ng.9csxet.cn

PHP:  curl_multi_init() 系列
来源：http://yn.jianghongdianzi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ev.asd995.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gr.lnxyls.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://za.nszjky.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ai.asd995.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ud.hnjuh.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gu.huixinmuqiang.cn

================================================================================
来源：http://gx.asd995.cn

M. 命令行 / 进程 / 环境
来源：http://sd.bookmarksfly.cn

================================================================================
来源：http://pm.gzmigu.cn

[M01] 读取命令行参数
来源：http://hf.wgjwhj.cn

Py:   sys.argv[1:]
来源：http://hr.asd995.cn

PHP:  $argv;  $argc;
来源：http://rq.wgjwhj.cn

JS:   process.argv.slice(2)
来源：http://af.hnjuh.cn

TS:   process.argv.slice(2)
来源：http://os.szsharing.cn

Java: args 数组（main 方法参数）
来源：http://hn.nicolike.cn

Go:   os.Args[1:]
来源：http://ks.shtwfgs.cn

Ruby: ARGV
来源：http://xh.nicolike.cn

C#:   args 数组（Main 方法参数）
来源：http://zz.yuntaijiaju.cn

[M02] 读取环境变量
来源：http://qh.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://bz.9csxet.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sr.lnxyls.cn

JS:   process.env.HOME
来源：http://wi.521024.cn

TS:   process.env.HOME
来源：http://pr.wgjwhj.cn

Java: System.getenv("HOME")
来源：http://lo.muxihuayi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ri.wgjwhj.cn

Ruby: ENV["HOME"]
来源：http://ac.szsharing.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rg.lnxyls.cn

[M03] 执行外部命令
来源：http://lm.yuntaijiaju.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://si.muxihuayi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://oa.newstarts.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://sy.huixinmuqiang.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ug.jctech888.com.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gf.hnjuh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fu.shxzukj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://mr.wgjwhj.cn

C#:   Process.Start("ls", "-l");
来源：http://wl.szxytkj.cn

[M04] 获取当前工作目录
来源：http://pj.9csxet.cn

Py:   os.getcwd()
来源：http://gd.szsharing.cn

PHP:  getcwd();
来源：http://xk.huanxung.cn

JS:   process.cwd()
来源：http://ry.yuexingan06.cn

TS:   process.cwd()
来源：http://co.chemitech.net.cn

Java: Path.of("").toAbsolutePath()
来源：http://rf.panjiajie.cn

Go:   os.Getwd()
来源：http://hd.yuntaijiaju.cn

Ruby: Dir.pwd
来源：http://js.jctech888.com.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ho.9csxet.cn

[M05] 设置退出码
来源：http://ib.nicolike.cn

Py:   sys.exit(1)
来源：http://kr.bjjhwx.cn

PHP:  exit(1);
来源：http://zr.panjiajie.cn

JS:   process.exit(1)
来源：http://ck.yuntaijiaju.cn

TS:   process.exit(1)
来源：http://vk.gzmigu.cn

Java: System.exit(1)
来源：http://gp.shxzskj.cn

Go:   os.Exit(1)
来源：http://vw.nszjky.cn

Ruby: exit 1
来源：http://ob.jianghongdianzi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pj.hahajie.cn

[M06] 向标准错误输出
来源：http://tf.yuexingan06.cn

Py:   print("err", file=sys.stderr)
来源：http://xy.nicolike.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ch.shxzukj.cn

JS:   console.error("err")
来源：http://lv.9csxet.cn

TS:   console.error("err")
来源：http://ro.shtwfgs.cn

Java: System.err.println("err")
来源：http://pp.hnjuh.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hx.szsharing.cn

Ruby: warn "err"
来源：http://hc.bookmarksfly.cn

C#:   Console.Error.WriteLine("err")
来源：http://sc.bjjhwx.cn

[M07] 判断是否为主入口
来源：http://pl.muxihuayi.cn

Py:   if __name__ == "__main__":
来源：http://sz.muxihuayi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zg.huixinmuqiang.cn

JS:   require.main === module
来源：http://dc.huanxung.cn

TS:   require.main === module
来源：http://an.wgjwhj.cn

Java: public static void main(String[] args)
来源：http://un.shxzskj.cn

Go:   func main()
来源：http://dz.hnjuh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sy.muxihuayi.cn

C#:   static void Main(string[] args)
来源：http://yb.gzmigu.cn

[M08] 获取系统与运行时信息
来源：http://uc.9csxet.cn

Py:   platform.system();  platform.python_version()
来源：http://uy.hahajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://eq.haigaiapp.cn

JS:   process.platform;  process.version
来源：http://qb.nszjky.cn


<!-- 参考信息 -->