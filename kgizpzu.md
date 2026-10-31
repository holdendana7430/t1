代发 wailian999

[J03] 字符串解析为日期
来源：http://xz.9csxet.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vf.bjjhwx.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pz.shxzskj.cn

JS:   new Date("2024-01-02")
来源：http://eq.hahajie.cn

TS:   new Date("2024-01-02")
来源：http://pd.huanxung.cn

Java: LocalDate.parse("2024-01-02")
来源：http://kz.wgjwhj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gt.hahajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://xn.chemitech.net.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gn.jctech888.com.cn

[J04] 时间戳与日期互转
来源：http://ia.yuexingan06.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bm.muxihuayi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hg.wgjwhj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ci.asd995.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gf.jctech888.com.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xh.jianghongdianzi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ip.szsharing.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hb.asd995.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pn.colortex.cn

[J05] 时间加减（加 7 天）
来源：http://ak.shtwfgs.cn

Py:   now + timedelta(days=7)
来源：http://ct.521024.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vc.asd995.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qu.jianghongdianzi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vz.newstarts.cn

Java: LocalDate.now().plusDays(7)
来源：http://gs.huanxung.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sb.jctech888.com.cn

Ruby: Time.now + 7 * 86400
来源：http://bt.shxzskj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zy.jctech888.com.cn

[J06] 计算两时间之差
来源：http://vz.jianghongdianzi.cn

Py:   (end - start).total_seconds()
来源：http://gu.bookmarksfly.cn

PHP:  $end->diff($start)->days;
来源：http://de.jianghongdianzi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pr.haigaiapp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ho.chemitech.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://kx.newstarts.cn

Go:   end.Sub(start).Hours()
来源：http://pn.gzmigu.cn

Ruby: end - start                 # 返回秒数
来源：http://vt.9csxet.cn

C#:   (end - start).TotalSeconds
来源：http://le.jianghongdianzi.cn

[J07] 比较两个日期
来源：http://em.huixiangedu.cn

Py:   d1 < d2;  d1 == d2
来源：http://mk.huixinmuqiang.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vw.huixinmuqiang.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ya.haigaiapp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ah.jianghongdianzi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dn.yuexingan06.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fi.jctech888.com.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cs.hnjuh.cn

C#:   d1 < d2;  d1 == d2
来源：http://qy.panjiajie.cn

[J08] 提取年月日与星期
来源：http://pf.nszjky.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ur.shtwfgs.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ks.nszjky.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vw.muxihuayi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ub.colortex.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xm.asd995.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pj.chemitech.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ng.huanxung.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qs.9csxet.cn

[J09] 时区处理
来源：http://df.nicolike.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dz.colortex.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://oo.newstarts.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ym.shxzukj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://or.chemitech.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fq.colortex.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dw.newstarts.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tp.9csxet.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kr.9csxet.cn

[J10] 取今天 / 本月第一天
来源：http://pa.hahajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://iu.jianghongdianzi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ao.asd995.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xp.muxihuayi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vm.yuntaijiaju.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yz.9csxet.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jf.gzmigu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gr.szsharing.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://te.muxihuayi.cn

================================================================================
来源：http://ua.lnxyls.cn

K. JSON 与序列化
来源：http://fa.yuexingan06.cn

================================================================================
来源：http://lv.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://jf.szsharing.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dv.521024.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://sg.yuexingan06.cn

JS:   JSON.stringify(obj)
来源：http://sq.szxytkj.cn

TS:   JSON.stringify(obj)
来源：http://iz.lnxyls.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://am.chemitech.net.cn

Go:   json.Marshal(obj)
来源：http://wo.gzmigu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ll.huanxung.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fs.szsharing.cn

[K02] JSON 字符串转对象
来源：http://ip.newstarts.cn

Py:   json.loads(s)
来源：http://sr.bjjhwx.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zg.panjiajie.cn

JS:   JSON.parse(s)
来源：http://ps.colortex.cn

TS:   JSON.parse(s)
来源：http://lu.huixinmuqiang.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yt.shtwfgs.cn

Go:   json.Unmarshal(data, &v)
来源：http://de.gzmigu.cn

Ruby: JSON.parse(s)
来源：http://xh.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://er.hahajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://ic.shxzskj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://je.shtwfgs.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qo.yuexingan06.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://oy.panjiajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://pp.bjjhwx.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lm.huixiangedu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://eu.jianghongdianzi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zf.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mc.panjiajie.cn

[K04] 读取 JSON 文件
来源：http://ld.hahajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ej.newstarts.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zy.huanxung.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sm.wgjwhj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pr.yuntaijiaju.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yq.newstarts.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bb.chemitech.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://iu.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ns.shxzukj.cn

[K05] 深拷贝对象
来源：http://li.nszjky.cn

Py:   copy.deepcopy(obj)
来源：http://jy.chemitech.net.cn

PHP:  unserialize(serialize($obj));
来源：http://so.jctech888.com.cn

JS:   structuredClone(obj)
来源：http://sf.shxzukj.cn

TS:   structuredClone(obj)
来源：http://oj.lnxyls.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bf.newstarts.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xa.nicolike.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tn.jctech888.com.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dx.chemitech.net.cn

[K06] 解析 URL 查询串
来源：http://un.hahajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kh.shxzukj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rq.shtwfgs.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ya.9csxet.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fi.shtwfgs.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nd.lnxyls.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://yx.szxytkj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://st.jianghongdianzi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kn.haigaiapp.cn

[K07] 进制转换
来源：http://zs.9csxet.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kq.9csxet.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tt.haigaiapp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bx.bookmarksfly.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ju.hnjuh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lu.haigaiapp.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ei.jctech888.com.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yg.shxzskj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bw.bjjhwx.cn

[K08] 二进制序列化（非 JSON）
来源：http://iq.colortex.cn

Py:   pickle.dumps(obj)
来源：http://zz.shtwfgs.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hy.muxihuayi.cn

JS:   v8.serialize(obj)        // Node
来源：http://yb.colortex.cn

TS:   v8.serialize(obj)        // Node
来源：http://tl.lnxyls.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://en.521024.cn

Go:   encoding/gob
来源：http://ls.haigaiapp.cn

Ruby: Marshal.dump(obj)
来源：http://zm.521024.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ki.shxzukj.cn

================================================================================
来源：http://qu.haigaiapp.cn

L. 网络请求
来源：http://mw.haigaiapp.cn

================================================================================
来源：http://xt.shxzukj.cn

[L01] 发送 GET 请求
来源：http://dp.wgjwhj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gg.jctech888.com.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://eg.jctech888.com.cn

JS:   await fetch(url)
来源：http://dx.gzmigu.cn

TS:   await fetch(url)
来源：http://fb.haigaiapp.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sq.bookmarksfly.cn

Go:   resp, err := http.Get(url)
来源：http://wm.wgjwhj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dy.nszjky.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nu.huanxung.cn

[L02] 发送 POST JSON
来源：http://nb.shxzukj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xk.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gk.haigaiapp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sp.huixiangedu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ba.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sa.9csxet.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jy.bjjhwx.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lg.szsharing.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qa.haigaiapp.cn

[L03] 设置自定义请求头
来源：http://al.szxytkj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tx.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ay.jctech888.com.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vn.521024.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pe.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vl.muxihuayi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vr.huixinmuqiang.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ga.colortex.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qw.jianghongdianzi.cn

[L04] 设置超时
来源：http://up.yuntaijiaju.cn

Py:   requests.get(url, timeout=5)
来源：http://wb.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vb.szsharing.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cf.9csxet.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://an.huixinmuqiang.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qh.asd995.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gi.huanxung.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qp.yuntaijiaju.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://js.asd995.cn

[L05] 上传文件（multipart）
来源：http://kh.nicolike.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pa.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ii.huixiangedu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://py.bookmarksfly.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mz.haigaiapp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lr.shxzskj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mo.szxytkj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cs.yuexingan06.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vp.colortex.cn

[L06] 解析响应为 JSON
来源：http://gh.yuntaijiaju.cn

Py:   resp.json()
来源：http://yb.lnxyls.cn

PHP:  json_decode($body, true);
来源：http://sa.jianghongdianzi.cn

JS:   await resp.json()
来源：http://qa.jianghongdianzi.cn

TS:   await resp.json()
来源：http://ko.chemitech.net.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fx.huixiangedu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dx.newstarts.cn

Ruby: JSON.parse(resp.body)
来源：http://nh.shtwfgs.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://he.shxzukj.cn

[L07] 处理 HTTP 状态码
来源：http://fw.asd995.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yk.9csxet.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gx.yuntaijiaju.cn

JS:   resp.ok;  resp.status
来源：http://qb.nicolike.cn

TS:   resp.ok;  resp.status
来源：http://fh.huanxung.cn

Java: resp.statusCode()
来源：http://wb.asd995.cn

Go:   resp.StatusCode
来源：http://yn.9csxet.cn

Ruby: resp.code.to_i
来源：http://gi.gzmigu.cn

C#:   (int)resp.StatusCode
来源：http://lt.jctech888.com.cn

[L08] 并发请求多个地址
来源：http://ci.jctech888.com.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://re.9csxet.cn

PHP:  curl_multi_init() 系列
来源：http://vj.muxihuayi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://av.huixinmuqiang.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://po.shxzskj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://os.asd995.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wp.asd995.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lu.hnjuh.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qh.yuexingan06.cn

================================================================================
来源：http://ym.huanxung.cn

M. 命令行 / 进程 / 环境
来源：http://ql.szsharing.cn

================================================================================
来源：http://ld.hahajie.cn

[M01] 读取命令行参数
来源：http://gv.jianghongdianzi.cn

Py:   sys.argv[1:]
来源：http://qo.asd995.cn

PHP:  $argv;  $argc;
来源：http://wl.jianghongdianzi.cn

JS:   process.argv.slice(2)
来源：http://qp.bjjhwx.cn

TS:   process.argv.slice(2)
来源：http://nv.jctech888.com.cn

Java: args 数组（main 方法参数）
来源：http://av.jianghongdianzi.cn

Go:   os.Args[1:]
来源：http://ty.chemitech.net.cn

Ruby: ARGV
来源：http://ai.colortex.cn

C#:   args 数组（Main 方法参数）
来源：http://mi.asd995.cn

[M02] 读取环境变量
来源：http://jn.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://ke.521024.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zj.lnxyls.cn

JS:   process.env.HOME
来源：http://gn.521024.cn

TS:   process.env.HOME
来源：http://ih.hnjuh.cn

Java: System.getenv("HOME")
来源：http://ks.521024.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zn.huixiangedu.cn

Ruby: ENV["HOME"]
来源：http://yy.chemitech.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kz.szxytkj.cn

[M03] 执行外部命令
来源：http://ul.newstarts.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ma.bjjhwx.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zt.lnxyls.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ok.bookmarksfly.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://hu.szsharing.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://he.jianghongdianzi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://iv.szxytkj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tf.muxihuayi.cn

C#:   Process.Start("ls", "-l");
来源：http://ow.asd995.cn

[M04] 获取当前工作目录
来源：http://ta.muxihuayi.cn

Py:   os.getcwd()
来源：http://go.wgjwhj.cn

PHP:  getcwd();
来源：http://gg.asd995.cn

JS:   process.cwd()
来源：http://ss.521024.cn

TS:   process.cwd()
来源：http://ef.bookmarksfly.cn

Java: Path.of("").toAbsolutePath()
来源：http://pb.yuntaijiaju.cn

Go:   os.Getwd()
来源：http://kj.yuexingan06.cn

Ruby: Dir.pwd
来源：http://qe.huixinmuqiang.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jd.haigaiapp.cn

[M05] 设置退出码
来源：http://pw.jctech888.com.cn

Py:   sys.exit(1)
来源：http://tj.nicolike.cn

PHP:  exit(1);
来源：http://zh.521024.cn

JS:   process.exit(1)
来源：http://xw.haigaiapp.cn

TS:   process.exit(1)
来源：http://tf.bjjhwx.cn

Java: System.exit(1)
来源：http://ql.gzmigu.cn

Go:   os.Exit(1)
来源：http://ur.jianghongdianzi.cn

Ruby: exit 1
来源：http://kk.panjiajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qk.shxzskj.cn

[M06] 向标准错误输出
来源：http://cv.gzmigu.cn

Py:   print("err", file=sys.stderr)
来源：http://qh.szsharing.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pk.huixiangedu.cn

JS:   console.error("err")
来源：http://ag.colortex.cn

TS:   console.error("err")
来源：http://op.shxzukj.cn

Java: System.err.println("err")
来源：http://uv.haigaiapp.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ox.panjiajie.cn

Ruby: warn "err"
来源：http://uz.hahajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://ym.gzmigu.cn

[M07] 判断是否为主入口
来源：http://fh.shtwfgs.cn

Py:   if __name__ == "__main__":
来源：http://bd.gzmigu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ma.chemitech.net.cn

JS:   require.main === module
来源：http://mm.jctech888.com.cn

TS:   require.main === module
来源：http://nm.9csxet.cn

Java: public static void main(String[] args)
来源：http://ld.huixinmuqiang.cn

Go:   func main()
来源：http://sm.huixiangedu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rn.521024.cn

C#:   static void Main(string[] args)
来源：http://el.huixinmuqiang.cn

[M08] 获取系统与运行时信息
来源：http://ut.yuexingan06.cn

Py:   platform.system();  platform.python_version()
来源：http://dc.szxytkj.cn

PHP:  PHP_OS;  phpversion();
来源：http://gn.521024.cn

JS:   process.platform;  process.version
来源：http://zb.chemitech.net.cn

TS:   process.platform;  process.version
来源：http://tw.shtwfgs.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ln.bjjhwx.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://cj.colortex.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xi.huixiangedu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dm.hnjuh.cn

================================================================================
来源：http://ne.521024.cn

N. 数据结构与算法
来源：http://jv.hahajie.cn

================================================================================
来源：http://kg.asd995.cn


<!-- 参考信息 -->