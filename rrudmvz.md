代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hy.huixinmuqiang.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sc.yuntaijiaju.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qo.huixiangedu.cn

TS:   d.toISOString()
来源：http://xg.shxzskj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://av.bjjhwx.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://be.yuexingan06.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wh.huanxung.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vq.yuexingan06.cn

[J03] 字符串解析为日期
来源：http://mi.panjiajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://op.szxytkj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://le.shxzskj.cn

JS:   new Date("2024-01-02")
来源：http://ox.yuntaijiaju.cn

TS:   new Date("2024-01-02")
来源：http://gv.huixinmuqiang.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dc.szsharing.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cz.muxihuayi.cn

Ruby: Date.parse("2024-01-02")
来源：http://ep.shtwfgs.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tu.nicolike.cn

[J04] 时间戳与日期互转
来源：http://mg.yuntaijiaju.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tv.shxzskj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jp.shxzskj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cb.bjjhwx.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://nz.bookmarksfly.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ta.panjiajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wq.asd995.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rk.gzmigu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rg.huanxung.cn

[J05] 时间加减（加 7 天）
来源：http://iy.panjiajie.cn

Py:   now + timedelta(days=7)
来源：http://tx.lnxyls.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sw.wgjwhj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yb.colortex.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xn.panjiajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://nc.huanxung.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://eo.szxytkj.cn

Ruby: Time.now + 7 * 86400
来源：http://yk.9csxet.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ot.521024.cn

[J06] 计算两时间之差
来源：http://kl.chemitech.net.cn

Py:   (end - start).total_seconds()
来源：http://nn.panjiajie.cn

PHP:  $end->diff($start)->days;
来源：http://bi.jctech888.com.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kd.shtwfgs.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nr.shxzukj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jw.muxihuayi.cn

Go:   end.Sub(start).Hours()
来源：http://qa.jctech888.com.cn

Ruby: end - start                 # 返回秒数
来源：http://tw.yuntaijiaju.cn

C#:   (end - start).TotalSeconds
来源：http://nz.hahajie.cn

[J07] 比较两个日期
来源：http://xb.newstarts.cn

Py:   d1 < d2;  d1 == d2
来源：http://ek.wgjwhj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ty.hahajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://il.asd995.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zc.huixiangedu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yh.asd995.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mx.nszjky.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pl.huixinmuqiang.cn

C#:   d1 < d2;  d1 == d2
来源：http://fk.asd995.cn

[J08] 提取年月日与星期
来源：http://su.chemitech.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ch.muxihuayi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ci.wgjwhj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rn.shxzukj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gv.colortex.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fj.jctech888.com.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bi.wgjwhj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dl.panjiajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ty.huixinmuqiang.cn

[J09] 时区处理
来源：http://kg.jianghongdianzi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bu.nszjky.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pv.haigaiapp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ku.shxzskj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ur.asd995.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cw.chemitech.net.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://un.wgjwhj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://at.newstarts.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sj.huixinmuqiang.cn

[J10] 取今天 / 本月第一天
来源：http://ur.jianghongdianzi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://py.bookmarksfly.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jj.szxytkj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bf.shxzukj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pl.panjiajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jk.bjjhwx.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uu.9csxet.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fc.bookmarksfly.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xo.asd995.cn

================================================================================
来源：http://fz.9csxet.cn

K. JSON 与序列化
来源：http://ea.huixinmuqiang.cn

================================================================================
来源：http://ib.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://jy.szxytkj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xv.szsharing.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vg.haigaiapp.cn

JS:   JSON.stringify(obj)
来源：http://ry.wgjwhj.cn

TS:   JSON.stringify(obj)
来源：http://sl.lnxyls.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://in.asd995.cn

Go:   json.Marshal(obj)
来源：http://tw.huixinmuqiang.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ls.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ox.muxihuayi.cn

[K02] JSON 字符串转对象
来源：http://zl.nszjky.cn

Py:   json.loads(s)
来源：http://md.hnjuh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dg.lnxyls.cn

JS:   JSON.parse(s)
来源：http://be.colortex.cn

TS:   JSON.parse(s)
来源：http://sn.colortex.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ow.bookmarksfly.cn

Go:   json.Unmarshal(data, &v)
来源：http://fu.huixiangedu.cn

Ruby: JSON.parse(s)
来源：http://rg.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://iw.huixiangedu.cn

[K03] JSON 美化输出（带缩进）
来源：http://th.colortex.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yv.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jl.gzmigu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dr.asd995.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vh.gzmigu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ad.shtwfgs.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jf.9csxet.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dm.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://og.chemitech.net.cn

[K04] 读取 JSON 文件
来源：http://qv.hnjuh.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gd.jctech888.com.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://eu.huixiangedu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jy.bjjhwx.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rk.9csxet.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uo.nszjky.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pz.shxzukj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://sr.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vm.szsharing.cn

[K05] 深拷贝对象
来源：http://zs.nicolike.cn

Py:   copy.deepcopy(obj)
来源：http://jf.shxzukj.cn

PHP:  unserialize(serialize($obj));
来源：http://nd.wgjwhj.cn

JS:   structuredClone(obj)
来源：http://cu.bookmarksfly.cn

TS:   structuredClone(obj)
来源：http://gi.colortex.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fn.jianghongdianzi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nr.newstarts.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pj.bjjhwx.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yz.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://dh.nszjky.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mo.szxytkj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cq.panjiajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pm.muxihuayi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mh.gzmigu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fr.shtwfgs.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pi.yuexingan06.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rz.huixiangedu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yf.newstarts.cn

[K07] 进制转换
来源：http://hu.szsharing.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ci.huixiangedu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ym.hahajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qg.shxzskj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nd.9csxet.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xe.chemitech.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jw.jctech888.com.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oc.gzmigu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kr.shtwfgs.cn

[K08] 二进制序列化（非 JSON）
来源：http://di.haigaiapp.cn

Py:   pickle.dumps(obj)
来源：http://ea.huixiangedu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ke.szxytkj.cn

JS:   v8.serialize(obj)        // Node
来源：http://nh.bookmarksfly.cn

TS:   v8.serialize(obj)        // Node
来源：http://ft.wgjwhj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hx.wgjwhj.cn

Go:   encoding/gob
来源：http://sz.lnxyls.cn

Ruby: Marshal.dump(obj)
来源：http://go.huixiangedu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dx.wgjwhj.cn

================================================================================
来源：http://la.yuexingan06.cn

L. 网络请求
来源：http://mi.hahajie.cn

================================================================================
来源：http://pz.bjjhwx.cn

[L01] 发送 GET 请求
来源：http://kb.bookmarksfly.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vu.shtwfgs.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ax.newstarts.cn

JS:   await fetch(url)
来源：http://vn.muxihuayi.cn

TS:   await fetch(url)
来源：http://hg.newstarts.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bn.nicolike.cn

Go:   resp, err := http.Get(url)
来源：http://yf.newstarts.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://lm.nszjky.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hi.nszjky.cn

[L02] 发送 POST JSON
来源：http://ka.wgjwhj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://iy.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jz.szxytkj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ky.yuntaijiaju.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cn.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://br.yuexingan06.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lm.jianghongdianzi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://im.wgjwhj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wq.yuexingan06.cn

[L03] 设置自定义请求头
来源：http://zu.colortex.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pq.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ma.gzmigu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rl.chemitech.net.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zn.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ve.yuexingan06.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://si.shtwfgs.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rm.shtwfgs.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ue.shtwfgs.cn

[L04] 设置超时
来源：http://cc.shtwfgs.cn

Py:   requests.get(url, timeout=5)
来源：http://zr.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://by.jctech888.com.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hn.haigaiapp.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cb.huixiangedu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xm.jianghongdianzi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ou.chemitech.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sp.szsharing.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gj.gzmigu.cn

[L05] 上传文件（multipart）
来源：http://jw.shxzskj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://el.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sn.hahajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ew.wgjwhj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://na.wgjwhj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wd.shxzukj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jo.yuexingan06.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yb.yuexingan06.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ms.521024.cn

[L06] 解析响应为 JSON
来源：http://hy.szxytkj.cn

Py:   resp.json()
来源：http://cf.panjiajie.cn

PHP:  json_decode($body, true);
来源：http://ua.bookmarksfly.cn

JS:   await resp.json()
来源：http://qq.nszjky.cn

TS:   await resp.json()
来源：http://jf.colortex.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gh.hahajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fu.asd995.cn

Ruby: JSON.parse(resp.body)
来源：http://vq.chemitech.net.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gl.chemitech.net.cn

[L07] 处理 HTTP 状态码
来源：http://ul.newstarts.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zl.hnjuh.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vi.shxzukj.cn

JS:   resp.ok;  resp.status
来源：http://dk.hnjuh.cn

TS:   resp.ok;  resp.status
来源：http://fz.nicolike.cn

Java: resp.statusCode()
来源：http://zy.newstarts.cn

Go:   resp.StatusCode
来源：http://qp.shxzskj.cn

Ruby: resp.code.to_i
来源：http://ja.newstarts.cn

C#:   (int)resp.StatusCode
来源：http://er.shtwfgs.cn

[L08] 并发请求多个地址
来源：http://bf.hahajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zk.lnxyls.cn

PHP:  curl_multi_init() 系列
来源：http://xt.yuntaijiaju.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lp.bookmarksfly.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nz.9csxet.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://my.shtwfgs.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pr.szsharing.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://el.colortex.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qa.lnxyls.cn

================================================================================
来源：http://bd.shxzskj.cn

M. 命令行 / 进程 / 环境
来源：http://ya.yuntaijiaju.cn

================================================================================
来源：http://dj.haigaiapp.cn

[M01] 读取命令行参数
来源：http://sh.nicolike.cn

Py:   sys.argv[1:]
来源：http://zk.shxzskj.cn

PHP:  $argv;  $argc;
来源：http://gb.newstarts.cn

JS:   process.argv.slice(2)
来源：http://sb.colortex.cn

TS:   process.argv.slice(2)
来源：http://mg.hnjuh.cn

Java: args 数组（main 方法参数）
来源：http://sy.huixinmuqiang.cn

Go:   os.Args[1:]
来源：http://um.gzmigu.cn

Ruby: ARGV
来源：http://wg.huixinmuqiang.cn

C#:   args 数组（Main 方法参数）
来源：http://mf.asd995.cn

[M02] 读取环境变量
来源：http://xm.yuntaijiaju.cn

Py:   os.environ.get("HOME")
来源：http://bl.lnxyls.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yw.muxihuayi.cn

JS:   process.env.HOME
来源：http://bx.szsharing.cn

TS:   process.env.HOME
来源：http://dp.gzmigu.cn

Java: System.getenv("HOME")
来源：http://fl.jianghongdianzi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://me.nszjky.cn

Ruby: ENV["HOME"]
来源：http://vs.gzmigu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nu.shxzskj.cn

[M03] 执行外部命令
来源：http://aq.chemitech.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lr.yuntaijiaju.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hl.lnxyls.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nj.hnjuh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://et.newstarts.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mm.chemitech.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://tb.jianghongdianzi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wg.shtwfgs.cn

C#:   Process.Start("ls", "-l");
来源：http://bp.szxytkj.cn

[M04] 获取当前工作目录
来源：http://pz.panjiajie.cn

Py:   os.getcwd()
来源：http://za.bookmarksfly.cn

PHP:  getcwd();
来源：http://zf.asd995.cn

JS:   process.cwd()
来源：http://sx.huixinmuqiang.cn

TS:   process.cwd()
来源：http://ce.haigaiapp.cn

Java: Path.of("").toAbsolutePath()
来源：http://kr.wgjwhj.cn

Go:   os.Getwd()
来源：http://ke.521024.cn

Ruby: Dir.pwd
来源：http://fb.bjjhwx.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yu.colortex.cn

[M05] 设置退出码
来源：http://mz.shxzukj.cn

Py:   sys.exit(1)
来源：http://oj.yuntaijiaju.cn

PHP:  exit(1);
来源：http://wa.gzmigu.cn

JS:   process.exit(1)
来源：http://yb.muxihuayi.cn

TS:   process.exit(1)
来源：http://ah.panjiajie.cn

Java: System.exit(1)
来源：http://wr.hnjuh.cn

Go:   os.Exit(1)
来源：http://sd.hahajie.cn

Ruby: exit 1
来源：http://ti.lnxyls.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lk.muxihuayi.cn

[M06] 向标准错误输出
来源：http://eg.jctech888.com.cn

Py:   print("err", file=sys.stderr)
来源：http://hi.nicolike.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cv.9csxet.cn

JS:   console.error("err")
来源：http://gd.521024.cn

TS:   console.error("err")
来源：http://mo.521024.cn

Java: System.err.println("err")
来源：http://vf.hnjuh.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xf.nszjky.cn

Ruby: warn "err"
来源：http://ds.9csxet.cn

C#:   Console.Error.WriteLine("err")
来源：http://hi.huixiangedu.cn

[M07] 判断是否为主入口
来源：http://kp.wgjwhj.cn

Py:   if __name__ == "__main__":
来源：http://px.bjjhwx.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://it.shxzskj.cn

JS:   require.main === module
来源：http://gt.huixinmuqiang.cn

TS:   require.main === module
来源：http://qo.shxzskj.cn

Java: public static void main(String[] args)
来源：http://ry.panjiajie.cn

Go:   func main()
来源：http://fl.shxzukj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qn.shxzukj.cn

C#:   static void Main(string[] args)
来源：http://bv.jianghongdianzi.cn

[M08] 获取系统与运行时信息
来源：http://yl.nszjky.cn

Py:   platform.system();  platform.python_version()
来源：http://fx.szxytkj.cn

PHP:  PHP_OS;  phpversion();
来源：http://zf.521024.cn

JS:   process.platform;  process.version
来源：http://le.nszjky.cn


<!-- 参考信息 -->