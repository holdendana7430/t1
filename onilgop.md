代发 wailian999

TS:   new Date("2024-01-02")
来源：http://fy.lnxyls.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ek.bookmarksfly.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sj.jctech888.com.cn

Ruby: Date.parse("2024-01-02")
来源：http://yj.newstarts.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kc.yuexingan06.cn

[J04] 时间戳与日期互转
来源：http://yv.yuntaijiaju.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yi.shtwfgs.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jc.jianghongdianzi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ql.chemitech.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vc.nszjky.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gt.hnjuh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sn.huanxung.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cb.jctech888.com.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mt.jctech888.com.cn

[J05] 时间加减（加 7 天）
来源：http://xu.huixinmuqiang.cn

Py:   now + timedelta(days=7)
来源：http://fi.9csxet.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://uc.bookmarksfly.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://oz.hnjuh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nz.nicolike.cn

Java: LocalDate.now().plusDays(7)
来源：http://nz.hahajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ox.bjjhwx.cn

Ruby: Time.now + 7 * 86400
来源：http://ac.gzmigu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://dp.huixiangedu.cn

[J06] 计算两时间之差
来源：http://rs.gzmigu.cn

Py:   (end - start).total_seconds()
来源：http://ee.newstarts.cn

PHP:  $end->diff($start)->days;
来源：http://ka.hahajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pl.shxzukj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xx.hnjuh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://wt.jianghongdianzi.cn

Go:   end.Sub(start).Hours()
来源：http://hc.haigaiapp.cn

Ruby: end - start                 # 返回秒数
来源：http://uu.colortex.cn

C#:   (end - start).TotalSeconds
来源：http://ma.nicolike.cn

[J07] 比较两个日期
来源：http://uc.newstarts.cn

Py:   d1 < d2;  d1 == d2
来源：http://nz.yuexingan06.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uq.9csxet.cn

JS:   d1.getTime() < d2.getTime()
来源：http://oo.szxytkj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ph.szsharing.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yp.muxihuayi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jy.hnjuh.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pn.nszjky.cn

C#:   d1 < d2;  d1 == d2
来源：http://ls.chemitech.net.cn

[J08] 提取年月日与星期
来源：http://xo.9csxet.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://df.panjiajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dd.colortex.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xy.colortex.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yt.bookmarksfly.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yl.9csxet.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dx.asd995.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nr.panjiajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zo.muxihuayi.cn

[J09] 时区处理
来源：http://lf.9csxet.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fn.colortex.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gf.shxzskj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ru.shxzskj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qk.newstarts.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://uy.huanxung.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ff.haigaiapp.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ix.lnxyls.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ow.shxzskj.cn

[J10] 取今天 / 本月第一天
来源：http://ym.lnxyls.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://nv.hnjuh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wl.shxzukj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://eg.colortex.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cb.szxytkj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ue.panjiajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kl.9csxet.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xs.colortex.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wd.yuntaijiaju.cn

================================================================================
来源：http://xr.jianghongdianzi.cn

K. JSON 与序列化
来源：http://tk.521024.cn

================================================================================
来源：http://tp.muxihuayi.cn

[K01] 对象转 JSON 字符串
来源：http://io.huixiangedu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lf.haigaiapp.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://my.shxzukj.cn

JS:   JSON.stringify(obj)
来源：http://wq.nszjky.cn

TS:   JSON.stringify(obj)
来源：http://sn.hnjuh.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wf.jctech888.com.cn

Go:   json.Marshal(obj)
来源：http://mx.wgjwhj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://lm.colortex.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://do.521024.cn

[K02] JSON 字符串转对象
来源：http://xv.gzmigu.cn

Py:   json.loads(s)
来源：http://tr.chemitech.net.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jd.bjjhwx.cn

JS:   JSON.parse(s)
来源：http://lp.colortex.cn

TS:   JSON.parse(s)
来源：http://oo.bjjhwx.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dp.shtwfgs.cn

Go:   json.Unmarshal(data, &v)
来源：http://uk.hahajie.cn

Ruby: JSON.parse(s)
来源：http://ko.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xl.asd995.cn

[K03] JSON 美化输出（带缩进）
来源：http://we.panjiajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rx.szxytkj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yj.nicolike.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gg.chemitech.net.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://po.newstarts.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mp.panjiajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kr.chemitech.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ct.lnxyls.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hx.bookmarksfly.cn

[K04] 读取 JSON 文件
来源：http://mb.yuntaijiaju.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vc.newstarts.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hb.jctech888.com.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oe.szxytkj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ql.lnxyls.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xh.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mc.wgjwhj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ns.colortex.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ca.nicolike.cn

[K05] 深拷贝对象
来源：http://rl.lnxyls.cn

Py:   copy.deepcopy(obj)
来源：http://ic.haigaiapp.cn

PHP:  unserialize(serialize($obj));
来源：http://pr.jianghongdianzi.cn

JS:   structuredClone(obj)
来源：http://eg.lnxyls.cn

TS:   structuredClone(obj)
来源：http://dd.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bq.bookmarksfly.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pw.hahajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pj.asd995.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ue.shtwfgs.cn

[K06] 解析 URL 查询串
来源：http://ve.szsharing.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xp.huanxung.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ha.nicolike.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lm.asd995.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://by.huixinmuqiang.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nm.yuexingan06.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mc.lnxyls.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uj.nszjky.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pj.9csxet.cn

[K07] 进制转换
来源：http://yi.shtwfgs.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uh.asd995.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fz.jianghongdianzi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qh.nicolike.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jq.huanxung.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tk.nicolike.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vj.huanxung.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ym.gzmigu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hk.lnxyls.cn

[K08] 二进制序列化（非 JSON）
来源：http://da.yuexingan06.cn

Py:   pickle.dumps(obj)
来源：http://cb.shxzukj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://oj.shxzukj.cn

JS:   v8.serialize(obj)        // Node
来源：http://nr.521024.cn

TS:   v8.serialize(obj)        // Node
来源：http://lt.szxytkj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kw.muxihuayi.cn

Go:   encoding/gob
来源：http://cs.nicolike.cn

Ruby: Marshal.dump(obj)
来源：http://ar.jianghongdianzi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nr.hahajie.cn

================================================================================
来源：http://ak.colortex.cn

L. 网络请求
来源：http://nj.panjiajie.cn

================================================================================
来源：http://ta.nszjky.cn

[L01] 发送 GET 请求
来源：http://ky.lnxyls.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fn.panjiajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rq.hnjuh.cn

JS:   await fetch(url)
来源：http://vp.nszjky.cn

TS:   await fetch(url)
来源：http://wp.chemitech.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://is.521024.cn

Go:   resp, err := http.Get(url)
来源：http://fu.szsharing.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://px.panjiajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ak.bjjhwx.cn

[L02] 发送 POST JSON
来源：http://hk.newstarts.cn

Py:   requests.post(url, json={"a": 1})
来源：http://yn.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://oc.wgjwhj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gn.hahajie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bf.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jm.szsharing.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dd.huixinmuqiang.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://he.hahajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hc.colortex.cn

[L03] 设置自定义请求头
来源：http://rl.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cq.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ug.asd995.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uh.newstarts.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lu.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ka.szsharing.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mv.9csxet.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lm.bjjhwx.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zv.shxzskj.cn

[L04] 设置超时
来源：http://xm.panjiajie.cn

Py:   requests.get(url, timeout=5)
来源：http://xg.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ib.hnjuh.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ql.huixinmuqiang.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://em.nszjky.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ur.huanxung.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qv.nicolike.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hv.colortex.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://id.asd995.cn

[L05] 上传文件（multipart）
来源：http://qe.jctech888.com.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ao.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ge.9csxet.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kb.9csxet.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fq.colortex.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://np.panjiajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fj.muxihuayi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gy.shtwfgs.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pw.gzmigu.cn

[L06] 解析响应为 JSON
来源：http://gy.chemitech.net.cn

Py:   resp.json()
来源：http://pz.asd995.cn

PHP:  json_decode($body, true);
来源：http://gf.hahajie.cn

JS:   await resp.json()
来源：http://qo.wgjwhj.cn

TS:   await resp.json()
来源：http://ef.hnjuh.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dn.shxzskj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lq.newstarts.cn

Ruby: JSON.parse(resp.body)
来源：http://tm.asd995.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cv.chemitech.net.cn

[L07] 处理 HTTP 状态码
来源：http://sn.muxihuayi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dk.gzmigu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ga.gzmigu.cn

JS:   resp.ok;  resp.status
来源：http://np.bookmarksfly.cn

TS:   resp.ok;  resp.status
来源：http://hq.haigaiapp.cn

Java: resp.statusCode()
来源：http://li.9csxet.cn

Go:   resp.StatusCode
来源：http://ox.chemitech.net.cn

Ruby: resp.code.to_i
来源：http://jf.bookmarksfly.cn

C#:   (int)resp.StatusCode
来源：http://dz.shtwfgs.cn

[L08] 并发请求多个地址
来源：http://gf.huixiangedu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yf.shxzskj.cn

PHP:  curl_multi_init() 系列
来源：http://dz.chemitech.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jf.shxzskj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zj.yuexingan06.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kt.521024.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qn.hahajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wb.asd995.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ih.lnxyls.cn

================================================================================
来源：http://xm.lnxyls.cn

M. 命令行 / 进程 / 环境
来源：http://xn.521024.cn

================================================================================
来源：http://dl.hahajie.cn

[M01] 读取命令行参数
来源：http://td.shxzukj.cn

Py:   sys.argv[1:]
来源：http://cq.lnxyls.cn

PHP:  $argv;  $argc;
来源：http://yi.shxzukj.cn

JS:   process.argv.slice(2)
来源：http://ob.newstarts.cn

TS:   process.argv.slice(2)
来源：http://hz.huixiangedu.cn

Java: args 数组（main 方法参数）
来源：http://qn.newstarts.cn

Go:   os.Args[1:]
来源：http://sw.hahajie.cn

Ruby: ARGV
来源：http://su.jctech888.com.cn

C#:   args 数组（Main 方法参数）
来源：http://ax.newstarts.cn

[M02] 读取环境变量
来源：http://yr.haigaiapp.cn

Py:   os.environ.get("HOME")
来源：http://vf.szsharing.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ar.newstarts.cn

JS:   process.env.HOME
来源：http://qg.bjjhwx.cn

TS:   process.env.HOME
来源：http://gk.chemitech.net.cn

Java: System.getenv("HOME")
来源：http://cz.jctech888.com.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://by.shxzskj.cn

Ruby: ENV["HOME"]
来源：http://qh.9csxet.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pd.9csxet.cn

[M03] 执行外部命令
来源：http://dy.szxytkj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kb.wgjwhj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gu.shtwfgs.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://sv.haigaiapp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zs.wgjwhj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hg.shxzukj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wn.haigaiapp.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hk.nszjky.cn

C#:   Process.Start("ls", "-l");
来源：http://yk.huixiangedu.cn

[M04] 获取当前工作目录
来源：http://np.yuntaijiaju.cn

Py:   os.getcwd()
来源：http://ov.panjiajie.cn

PHP:  getcwd();
来源：http://cp.yuntaijiaju.cn

JS:   process.cwd()
来源：http://va.haigaiapp.cn

TS:   process.cwd()
来源：http://kx.lnxyls.cn

Java: Path.of("").toAbsolutePath()
来源：http://oz.bjjhwx.cn

Go:   os.Getwd()
来源：http://dh.hahajie.cn

Ruby: Dir.pwd
来源：http://fn.nszjky.cn

C#:   Directory.GetCurrentDirectory()
来源：http://bj.shxzskj.cn

[M05] 设置退出码
来源：http://fh.bookmarksfly.cn

Py:   sys.exit(1)
来源：http://xe.newstarts.cn

PHP:  exit(1);
来源：http://eb.newstarts.cn

JS:   process.exit(1)
来源：http://xp.shtwfgs.cn

TS:   process.exit(1)
来源：http://rj.colortex.cn

Java: System.exit(1)
来源：http://wu.shxzukj.cn

Go:   os.Exit(1)
来源：http://uk.panjiajie.cn

Ruby: exit 1
来源：http://lw.bjjhwx.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://au.shtwfgs.cn

[M06] 向标准错误输出
来源：http://mv.hahajie.cn

Py:   print("err", file=sys.stderr)
来源：http://zx.lnxyls.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://co.shtwfgs.cn

JS:   console.error("err")
来源：http://vn.yuntaijiaju.cn

TS:   console.error("err")
来源：http://ka.yuntaijiaju.cn

Java: System.err.println("err")
来源：http://ha.shxzskj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vx.yuexingan06.cn

Ruby: warn "err"
来源：http://rw.9csxet.cn

C#:   Console.Error.WriteLine("err")
来源：http://ka.huixiangedu.cn

[M07] 判断是否为主入口
来源：http://xm.521024.cn

Py:   if __name__ == "__main__":
来源：http://uw.hahajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jz.521024.cn

JS:   require.main === module
来源：http://ea.huixinmuqiang.cn

TS:   require.main === module
来源：http://xe.szxytkj.cn

Java: public static void main(String[] args)
来源：http://fb.yuntaijiaju.cn

Go:   func main()
来源：http://ha.wgjwhj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vq.lnxyls.cn

C#:   static void Main(string[] args)
来源：http://qg.bjjhwx.cn

[M08] 获取系统与运行时信息
来源：http://cx.szxytkj.cn

Py:   platform.system();  platform.python_version()
来源：http://rt.521024.cn

PHP:  PHP_OS;  phpversion();
来源：http://qw.yuexingan06.cn

JS:   process.platform;  process.version
来源：http://ik.shxzukj.cn

TS:   process.platform;  process.version
来源：http://yl.521024.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yq.huixiangedu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://pr.huixiangedu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cn.yuntaijiaju.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ij.newstarts.cn

================================================================================
来源：http://xo.shtwfgs.cn

N. 数据结构与算法
来源：http://ma.huanxung.cn

================================================================================
来源：http://kj.haigaiapp.cn

[N01] 二分查找（有序数组）
来源：http://zb.jctech888.com.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qu.9csxet.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rn.szsharing.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yd.nszjky.cn


<!-- 参考信息 -->