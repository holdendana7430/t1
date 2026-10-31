代发 wailian999

TS:   new Date("2024-01-02")
来源：http://kb.huanxung.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ue.szsharing.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cx.shtwfgs.cn

Ruby: Date.parse("2024-01-02")
来源：http://df.lnxyls.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rk.bjjhwx.cn

[J04] 时间戳与日期互转
来源：http://bj.hnjuh.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ls.jianghongdianzi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pz.nszjky.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://io.wgjwhj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://by.shxzskj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ju.shxzukj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qh.nszjky.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uq.shxzskj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rz.wgjwhj.cn

[J05] 时间加减（加 7 天）
来源：http://ls.muxihuayi.cn

Py:   now + timedelta(days=7)
来源：http://ke.lnxyls.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xx.yuntaijiaju.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ti.shxzskj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pw.newstarts.cn

Java: LocalDate.now().plusDays(7)
来源：http://bb.nszjky.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fe.szsharing.cn

Ruby: Time.now + 7 * 86400
来源：http://qy.huixinmuqiang.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xv.chemitech.net.cn

[J06] 计算两时间之差
来源：http://pq.huanxung.cn

Py:   (end - start).total_seconds()
来源：http://oi.521024.cn

PHP:  $end->diff($start)->days;
来源：http://oj.nicolike.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ky.szsharing.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ov.szsharing.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ee.szsharing.cn

Go:   end.Sub(start).Hours()
来源：http://ox.huixiangedu.cn

Ruby: end - start                 # 返回秒数
来源：http://oz.muxihuayi.cn

C#:   (end - start).TotalSeconds
来源：http://ck.newstarts.cn

[J07] 比较两个日期
来源：http://kn.yuexingan06.cn

Py:   d1 < d2;  d1 == d2
来源：http://fz.huanxung.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wg.nszjky.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rz.jctech888.com.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ud.huixiangedu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hd.asd995.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jk.shxzskj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jp.521024.cn

C#:   d1 < d2;  d1 == d2
来源：http://ip.wgjwhj.cn

[J08] 提取年月日与星期
来源：http://aa.9csxet.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fe.nicolike.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://aq.nszjky.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cj.shxzukj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zm.huixiangedu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uw.gzmigu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vq.jianghongdianzi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lr.9csxet.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gg.9csxet.cn

[J09] 时区处理
来源：http://ts.shxzukj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xs.hnjuh.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rs.nszjky.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ik.newstarts.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xn.yuexingan06.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ug.haigaiapp.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zx.wgjwhj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://rp.szxytkj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qy.wgjwhj.cn

[J10] 取今天 / 本月第一天
来源：http://sx.yuexingan06.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ga.bjjhwx.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zx.jianghongdianzi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yj.hnjuh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nk.huixinmuqiang.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zb.521024.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xg.bookmarksfly.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://co.panjiajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bs.shtwfgs.cn

================================================================================
来源：http://uk.jctech888.com.cn

K. JSON 与序列化
来源：http://pt.hnjuh.cn

================================================================================
来源：http://fb.panjiajie.cn

[K01] 对象转 JSON 字符串
来源：http://au.gzmigu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ag.asd995.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yf.521024.cn

JS:   JSON.stringify(obj)
来源：http://by.haigaiapp.cn

TS:   JSON.stringify(obj)
来源：http://ba.hnjuh.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qo.nszjky.cn

Go:   json.Marshal(obj)
来源：http://sy.panjiajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zk.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pz.haigaiapp.cn

[K02] JSON 字符串转对象
来源：http://zd.haigaiapp.cn

Py:   json.loads(s)
来源：http://ew.9csxet.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://as.panjiajie.cn

JS:   JSON.parse(s)
来源：http://ij.huixiangedu.cn

TS:   JSON.parse(s)
来源：http://fz.huanxung.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sj.muxihuayi.cn

Go:   json.Unmarshal(data, &v)
来源：http://ic.huixinmuqiang.cn

Ruby: JSON.parse(s)
来源：http://wq.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cd.jianghongdianzi.cn

[K03] JSON 美化输出（带缩进）
来源：http://ix.nicolike.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ay.muxihuayi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://am.bookmarksfly.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xb.yuexingan06.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fk.shxzskj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nx.hahajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yt.haigaiapp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jr.asd995.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ts.muxihuayi.cn

[K04] 读取 JSON 文件
来源：http://ze.chemitech.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pf.hahajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gq.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dg.shxzukj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ru.panjiajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ld.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pa.521024.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://pu.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bu.shxzukj.cn

[K05] 深拷贝对象
来源：http://gn.wgjwhj.cn

Py:   copy.deepcopy(obj)
来源：http://cr.shtwfgs.cn

PHP:  unserialize(serialize($obj));
来源：http://my.nszjky.cn

JS:   structuredClone(obj)
来源：http://ip.nicolike.cn

TS:   structuredClone(obj)
来源：http://kt.newstarts.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://he.hahajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://st.lnxyls.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ev.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://sd.panjiajie.cn

[K06] 解析 URL 查询串
来源：http://cv.gzmigu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://il.muxihuayi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lb.bjjhwx.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nv.wgjwhj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cx.521024.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nr.panjiajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rl.huixinmuqiang.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jh.hnjuh.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hm.yuntaijiaju.cn

[K07] 进制转换
来源：http://vf.shtwfgs.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cs.colortex.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ja.muxihuayi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ab.colortex.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sc.nszjky.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gq.hahajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gp.yuexingan06.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ja.yuntaijiaju.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mg.wgjwhj.cn

[K08] 二进制序列化（非 JSON）
来源：http://ao.muxihuayi.cn

Py:   pickle.dumps(obj)
来源：http://xp.haigaiapp.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bq.panjiajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://un.wgjwhj.cn

TS:   v8.serialize(obj)        // Node
来源：http://nj.panjiajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jc.gzmigu.cn

Go:   encoding/gob
来源：http://ei.gzmigu.cn

Ruby: Marshal.dump(obj)
来源：http://eq.huanxung.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://et.wgjwhj.cn

================================================================================
来源：http://iq.shtwfgs.cn

L. 网络请求
来源：http://dd.wgjwhj.cn

================================================================================
来源：http://ks.yuexingan06.cn

[L01] 发送 GET 请求
来源：http://ij.bookmarksfly.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gc.shxzukj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nt.huixinmuqiang.cn

JS:   await fetch(url)
来源：http://xh.shtwfgs.cn

TS:   await fetch(url)
来源：http://dt.jctech888.com.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ah.szsharing.cn

Go:   resp, err := http.Get(url)
来源：http://rr.hahajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://yf.nszjky.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://au.9csxet.cn

[L02] 发送 POST JSON
来源：http://ma.gzmigu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mb.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dh.newstarts.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rp.bjjhwx.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://py.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yb.yuexingan06.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gj.jianghongdianzi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tw.chemitech.net.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gy.shxzukj.cn

[L03] 设置自定义请求头
来源：http://hg.haigaiapp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dq.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ur.9csxet.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fr.bookmarksfly.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ym.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wb.wgjwhj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ty.shtwfgs.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hn.9csxet.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qf.9csxet.cn

[L04] 设置超时
来源：http://qu.yuntaijiaju.cn

Py:   requests.get(url, timeout=5)
来源：http://hu.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hr.huanxung.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hs.nszjky.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fm.chemitech.net.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ur.521024.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kx.shxzskj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gp.nszjky.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pi.jianghongdianzi.cn

[L05] 上传文件（multipart）
来源：http://le.yuexingan06.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fs.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jj.shxzukj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cy.bookmarksfly.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sz.bjjhwx.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ne.muxihuayi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xx.wgjwhj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ai.muxihuayi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rp.yuexingan06.cn

[L06] 解析响应为 JSON
来源：http://lg.huixiangedu.cn

Py:   resp.json()
来源：http://rv.chemitech.net.cn

PHP:  json_decode($body, true);
来源：http://bd.szxytkj.cn

JS:   await resp.json()
来源：http://nv.yuexingan06.cn

TS:   await resp.json()
来源：http://tz.wgjwhj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lh.hnjuh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wj.jctech888.com.cn

Ruby: JSON.parse(resp.body)
来源：http://xo.nicolike.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qe.muxihuayi.cn

[L07] 处理 HTTP 状态码
来源：http://ld.colortex.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dy.jctech888.com.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cr.nszjky.cn

JS:   resp.ok;  resp.status
来源：http://xi.bookmarksfly.cn

TS:   resp.ok;  resp.status
来源：http://ja.nszjky.cn

Java: resp.statusCode()
来源：http://us.9csxet.cn

Go:   resp.StatusCode
来源：http://jl.yuntaijiaju.cn

Ruby: resp.code.to_i
来源：http://tv.szsharing.cn

C#:   (int)resp.StatusCode
来源：http://oz.bjjhwx.cn

[L08] 并发请求多个地址
来源：http://se.wgjwhj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ld.9csxet.cn

PHP:  curl_multi_init() 系列
来源：http://fi.huixiangedu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lr.bjjhwx.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ui.yuexingan06.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fm.shtwfgs.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ub.szxytkj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dv.newstarts.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bj.521024.cn

================================================================================
来源：http://bz.yuexingan06.cn

M. 命令行 / 进程 / 环境
来源：http://ur.shtwfgs.cn

================================================================================
来源：http://qe.521024.cn

[M01] 读取命令行参数
来源：http://kr.bjjhwx.cn

Py:   sys.argv[1:]
来源：http://ja.nszjky.cn

PHP:  $argv;  $argc;
来源：http://ue.yuexingan06.cn

JS:   process.argv.slice(2)
来源：http://fb.szxytkj.cn

TS:   process.argv.slice(2)
来源：http://dl.panjiajie.cn

Java: args 数组（main 方法参数）
来源：http://ax.lnxyls.cn

Go:   os.Args[1:]
来源：http://cj.wgjwhj.cn

Ruby: ARGV
来源：http://hx.muxihuayi.cn

C#:   args 数组（Main 方法参数）
来源：http://tn.nicolike.cn

[M02] 读取环境变量
来源：http://ks.huixiangedu.cn

Py:   os.environ.get("HOME")
来源：http://dj.huixiangedu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://go.muxihuayi.cn

JS:   process.env.HOME
来源：http://ht.yuexingan06.cn

TS:   process.env.HOME
来源：http://by.shtwfgs.cn

Java: System.getenv("HOME")
来源：http://qr.muxihuayi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yw.shtwfgs.cn

Ruby: ENV["HOME"]
来源：http://lo.szsharing.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uc.haigaiapp.cn

[M03] 执行外部命令
来源：http://qv.yuntaijiaju.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mh.huixiangedu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://na.yuntaijiaju.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nb.huixinmuqiang.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pz.9csxet.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pj.shtwfgs.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://cu.hnjuh.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yh.szsharing.cn

C#:   Process.Start("ls", "-l");
来源：http://ky.huixiangedu.cn

[M04] 获取当前工作目录
来源：http://rr.panjiajie.cn

Py:   os.getcwd()
来源：http://un.bjjhwx.cn

PHP:  getcwd();
来源：http://ke.panjiajie.cn

JS:   process.cwd()
来源：http://ai.shxzukj.cn

TS:   process.cwd()
来源：http://ta.colortex.cn

Java: Path.of("").toAbsolutePath()
来源：http://cr.gzmigu.cn

Go:   os.Getwd()
来源：http://ph.shxzukj.cn

Ruby: Dir.pwd
来源：http://gu.chemitech.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jt.haigaiapp.cn

[M05] 设置退出码
来源：http://am.huanxung.cn

Py:   sys.exit(1)
来源：http://dt.szxytkj.cn

PHP:  exit(1);
来源：http://hi.gzmigu.cn

JS:   process.exit(1)
来源：http://ed.hnjuh.cn

TS:   process.exit(1)
来源：http://sh.haigaiapp.cn

Java: System.exit(1)
来源：http://gy.lnxyls.cn

Go:   os.Exit(1)
来源：http://xz.bjjhwx.cn

Ruby: exit 1
来源：http://qg.shxzukj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vf.huixiangedu.cn

[M06] 向标准错误输出
来源：http://ul.wgjwhj.cn

Py:   print("err", file=sys.stderr)
来源：http://rh.hnjuh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://co.521024.cn

JS:   console.error("err")
来源：http://tg.asd995.cn

TS:   console.error("err")
来源：http://cl.szsharing.cn

Java: System.err.println("err")
来源：http://cy.huixinmuqiang.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xk.huixinmuqiang.cn

Ruby: warn "err"
来源：http://wg.colortex.cn

C#:   Console.Error.WriteLine("err")
来源：http://uf.szsharing.cn

[M07] 判断是否为主入口
来源：http://jt.muxihuayi.cn

Py:   if __name__ == "__main__":
来源：http://yx.newstarts.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://va.yuexingan06.cn

JS:   require.main === module
来源：http://of.jctech888.com.cn

TS:   require.main === module
来源：http://ko.szxytkj.cn

Java: public static void main(String[] args)
来源：http://bq.colortex.cn

Go:   func main()
来源：http://hu.9csxet.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yz.hahajie.cn

C#:   static void Main(string[] args)
来源：http://yl.jctech888.com.cn

[M08] 获取系统与运行时信息
来源：http://fk.shtwfgs.cn

Py:   platform.system();  platform.python_version()
来源：http://bi.jianghongdianzi.cn

PHP:  PHP_OS;  phpversion();
来源：http://zn.haigaiapp.cn

JS:   process.platform;  process.version
来源：http://ml.wgjwhj.cn

TS:   process.platform;  process.version
来源：http://rn.shtwfgs.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kx.nszjky.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://jz.shtwfgs.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xl.shxzukj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zv.jctech888.com.cn

================================================================================
来源：http://zu.shtwfgs.cn

N. 数据结构与算法
来源：http://tm.wgjwhj.cn

================================================================================
来源：http://we.hnjuh.cn

[N01] 二分查找（有序数组）
来源：http://bo.yuntaijiaju.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kq.wgjwhj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yg.yuexingan06.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zb.nszjky.cn


<!-- 参考信息 -->