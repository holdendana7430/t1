代发 wailian999

TS:   new Date("2024-01-02")
来源：http://vw.hahajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qh.chemitech.net.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://eh.shxzskj.cn

Ruby: Date.parse("2024-01-02")
来源：http://vs.asd995.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ih.shxzukj.cn

[J04] 时间戳与日期互转
来源：http://hv.szsharing.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vr.jctech888.com.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yv.wgjwhj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rs.hahajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cr.lnxyls.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cw.huixiangedu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xy.9csxet.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://na.shtwfgs.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://at.panjiajie.cn

[J05] 时间加减（加 7 天）
来源：http://fx.nicolike.cn

Py:   now + timedelta(days=7)
来源：http://vj.huixinmuqiang.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yt.shxzukj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xj.panjiajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jd.521024.cn

Java: LocalDate.now().plusDays(7)
来源：http://xq.chemitech.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://er.panjiajie.cn

Ruby: Time.now + 7 * 86400
来源：http://zy.chemitech.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://tt.gzmigu.cn

[J06] 计算两时间之差
来源：http://xv.hahajie.cn

Py:   (end - start).total_seconds()
来源：http://zb.nicolike.cn

PHP:  $end->diff($start)->days;
来源：http://nw.shxzukj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cz.bookmarksfly.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ue.newstarts.cn

Java: Duration.between(start, end).toSeconds()
来源：http://tu.haigaiapp.cn

Go:   end.Sub(start).Hours()
来源：http://rq.bjjhwx.cn

Ruby: end - start                 # 返回秒数
来源：http://cv.bookmarksfly.cn

C#:   (end - start).TotalSeconds
来源：http://ml.lnxyls.cn

[J07] 比较两个日期
来源：http://wd.jianghongdianzi.cn

Py:   d1 < d2;  d1 == d2
来源：http://hv.shxzskj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://om.huixinmuqiang.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wa.bjjhwx.cn

TS:   d1.getTime() < d2.getTime()
来源：http://nd.wgjwhj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gn.yuexingan06.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fu.huixinmuqiang.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jk.szsharing.cn

C#:   d1 < d2;  d1 == d2
来源：http://ik.muxihuayi.cn

[J08] 提取年月日与星期
来源：http://be.yuexingan06.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rs.hnjuh.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sp.hnjuh.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mi.jianghongdianzi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ru.hahajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wv.panjiajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jo.hnjuh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mw.521024.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://aj.bookmarksfly.cn

[J09] 时区处理
来源：http://aa.lnxyls.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qc.nszjky.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nl.nszjky.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zi.lnxyls.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oa.huanxung.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dj.bjjhwx.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wb.haigaiapp.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wb.nszjky.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xb.nicolike.cn

[J10] 取今天 / 本月第一天
来源：http://jq.huixiangedu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://eu.yuntaijiaju.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qk.asd995.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ii.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tv.huixinmuqiang.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mu.asd995.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xb.szxytkj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wf.muxihuayi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ey.9csxet.cn

================================================================================
来源：http://be.9csxet.cn

K. JSON 与序列化
来源：http://gl.nicolike.cn

================================================================================
来源：http://ua.9csxet.cn

[K01] 对象转 JSON 字符串
来源：http://zt.nszjky.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kf.huixiangedu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hd.szsharing.cn

JS:   JSON.stringify(obj)
来源：http://cy.bjjhwx.cn

TS:   JSON.stringify(obj)
来源：http://jz.huanxung.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dm.521024.cn

Go:   json.Marshal(obj)
来源：http://yo.colortex.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xx.nicolike.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ri.521024.cn

[K02] JSON 字符串转对象
来源：http://xx.9csxet.cn

Py:   json.loads(s)
来源：http://if.hnjuh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ro.shxzskj.cn

JS:   JSON.parse(s)
来源：http://ox.haigaiapp.cn

TS:   JSON.parse(s)
来源：http://jg.chemitech.net.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tc.nszjky.cn

Go:   json.Unmarshal(data, &v)
来源：http://ij.newstarts.cn

Ruby: JSON.parse(s)
来源：http://un.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ld.yuntaijiaju.cn

[K03] JSON 美化输出（带缩进）
来源：http://sp.521024.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jc.yuexingan06.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://us.chemitech.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://op.muxihuayi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://by.jctech888.com.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zm.szsharing.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nz.huixiangedu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://yq.colortex.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://iw.panjiajie.cn

[K04] 读取 JSON 文件
来源：http://hr.huanxung.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zg.huixiangedu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pt.jianghongdianzi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kb.szxytkj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yx.haigaiapp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vb.asd995.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jh.colortex.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://pa.hnjuh.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xd.nicolike.cn

[K05] 深拷贝对象
来源：http://nq.colortex.cn

Py:   copy.deepcopy(obj)
来源：http://ks.shxzukj.cn

PHP:  unserialize(serialize($obj));
来源：http://ar.shtwfgs.cn

JS:   structuredClone(obj)
来源：http://jy.huixinmuqiang.cn

TS:   structuredClone(obj)
来源：http://jz.hnjuh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kn.yuntaijiaju.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hs.nszjky.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vf.nicolike.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ji.newstarts.cn

[K06] 解析 URL 查询串
来源：http://ry.haigaiapp.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xb.szxytkj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xm.shxzukj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yr.yuntaijiaju.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ea.521024.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bn.chemitech.net.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://yl.shxzskj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sd.gzmigu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tg.9csxet.cn

[K07] 进制转换
来源：http://fv.nszjky.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pi.jianghongdianzi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fk.muxihuayi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://el.szxytkj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sd.panjiajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wv.haigaiapp.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ej.nszjky.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qk.yuexingan06.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ld.yuntaijiaju.cn

[K08] 二进制序列化（非 JSON）
来源：http://tl.bookmarksfly.cn

Py:   pickle.dumps(obj)
来源：http://hj.yuexingan06.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://jp.asd995.cn

JS:   v8.serialize(obj)        // Node
来源：http://az.newstarts.cn

TS:   v8.serialize(obj)        // Node
来源：http://mg.lnxyls.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://da.huixinmuqiang.cn

Go:   encoding/gob
来源：http://ly.newstarts.cn

Ruby: Marshal.dump(obj)
来源：http://zk.huanxung.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://up.yuexingan06.cn

================================================================================
来源：http://sx.wgjwhj.cn

L. 网络请求
来源：http://ts.huixiangedu.cn

================================================================================
来源：http://uo.newstarts.cn

[L01] 发送 GET 请求
来源：http://kb.hahajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ai.bjjhwx.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jx.szxytkj.cn

JS:   await fetch(url)
来源：http://rl.hahajie.cn

TS:   await fetch(url)
来源：http://hp.szxytkj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://me.huixinmuqiang.cn

Go:   resp, err := http.Get(url)
来源：http://wk.lnxyls.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ax.jctech888.com.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://iq.bookmarksfly.cn

[L02] 发送 POST JSON
来源：http://ia.yuexingan06.cn

Py:   requests.post(url, json={"a": 1})
来源：http://if.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xc.shxzukj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ze.yuexingan06.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vl.asd995.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gn.shxzukj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ce.521024.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ea.yuntaijiaju.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jx.muxihuayi.cn

[L03] 设置自定义请求头
来源：http://zp.newstarts.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gf.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fb.szsharing.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cu.lnxyls.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ba.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://if.lnxyls.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lw.shxzukj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jq.nszjky.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bq.chemitech.net.cn

[L04] 设置超时
来源：http://ju.nszjky.cn

Py:   requests.get(url, timeout=5)
来源：http://sk.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rv.hahajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ne.haigaiapp.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yc.haigaiapp.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://do.haigaiapp.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://iw.jctech888.com.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bj.shtwfgs.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tj.hahajie.cn

[L05] 上传文件（multipart）
来源：http://to.jianghongdianzi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://on.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rz.panjiajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ss.521024.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://di.shxzukj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://by.nszjky.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ly.shtwfgs.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fg.shtwfgs.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://er.chemitech.net.cn

[L06] 解析响应为 JSON
来源：http://pr.szsharing.cn

Py:   resp.json()
来源：http://ji.huixiangedu.cn

PHP:  json_decode($body, true);
来源：http://zl.newstarts.cn

JS:   await resp.json()
来源：http://zh.shxzukj.cn

TS:   await resp.json()
来源：http://fy.huixiangedu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qd.szsharing.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dw.szsharing.cn

Ruby: JSON.parse(resp.body)
来源：http://to.nicolike.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tn.asd995.cn

[L07] 处理 HTTP 状态码
来源：http://qz.szsharing.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hs.9csxet.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kk.huixinmuqiang.cn

JS:   resp.ok;  resp.status
来源：http://vh.asd995.cn

TS:   resp.ok;  resp.status
来源：http://ys.jianghongdianzi.cn

Java: resp.statusCode()
来源：http://nc.nicolike.cn

Go:   resp.StatusCode
来源：http://gw.jianghongdianzi.cn

Ruby: resp.code.to_i
来源：http://lh.huanxung.cn

C#:   (int)resp.StatusCode
来源：http://ka.hnjuh.cn

[L08] 并发请求多个地址
来源：http://zp.szsharing.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ou.gzmigu.cn

PHP:  curl_multi_init() 系列
来源：http://ei.nicolike.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xh.haigaiapp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ic.bjjhwx.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mt.bjjhwx.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hj.szsharing.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ck.nszjky.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dp.hnjuh.cn

================================================================================
来源：http://ul.bookmarksfly.cn

M. 命令行 / 进程 / 环境
来源：http://nu.haigaiapp.cn

================================================================================
来源：http://jn.shtwfgs.cn

[M01] 读取命令行参数
来源：http://kn.wgjwhj.cn

Py:   sys.argv[1:]
来源：http://ns.szxytkj.cn

PHP:  $argv;  $argc;
来源：http://wn.jctech888.com.cn

JS:   process.argv.slice(2)
来源：http://oc.jctech888.com.cn

TS:   process.argv.slice(2)
来源：http://kz.newstarts.cn

Java: args 数组（main 方法参数）
来源：http://nz.newstarts.cn

Go:   os.Args[1:]
来源：http://sf.haigaiapp.cn

Ruby: ARGV
来源：http://uq.9csxet.cn

C#:   args 数组（Main 方法参数）
来源：http://hr.szsharing.cn

[M02] 读取环境变量
来源：http://gk.newstarts.cn

Py:   os.environ.get("HOME")
来源：http://fs.shtwfgs.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zv.hnjuh.cn

JS:   process.env.HOME
来源：http://mo.szxytkj.cn

TS:   process.env.HOME
来源：http://xh.newstarts.cn

Java: System.getenv("HOME")
来源：http://lj.bjjhwx.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dt.bookmarksfly.cn

Ruby: ENV["HOME"]
来源：http://cb.szxytkj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oq.yuexingan06.cn

[M03] 执行外部命令
来源：http://rr.yuntaijiaju.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ct.hahajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ux.huixiangedu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://yq.nicolike.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://st.nicolike.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kz.shxzukj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hr.muxihuayi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ov.colortex.cn

C#:   Process.Start("ls", "-l");
来源：http://bt.shxzskj.cn

[M04] 获取当前工作目录
来源：http://ph.nicolike.cn

Py:   os.getcwd()
来源：http://sc.wgjwhj.cn

PHP:  getcwd();
来源：http://rq.chemitech.net.cn

JS:   process.cwd()
来源：http://wa.szsharing.cn

TS:   process.cwd()
来源：http://nr.huixinmuqiang.cn

Java: Path.of("").toAbsolutePath()
来源：http://pm.shtwfgs.cn

Go:   os.Getwd()
来源：http://cw.colortex.cn

Ruby: Dir.pwd
来源：http://by.szsharing.cn

C#:   Directory.GetCurrentDirectory()
来源：http://lh.bjjhwx.cn

[M05] 设置退出码
来源：http://gk.bjjhwx.cn

Py:   sys.exit(1)
来源：http://fz.lnxyls.cn

PHP:  exit(1);
来源：http://bh.colortex.cn

JS:   process.exit(1)
来源：http://zp.colortex.cn

TS:   process.exit(1)
来源：http://xg.9csxet.cn

Java: System.exit(1)
来源：http://cz.bjjhwx.cn

Go:   os.Exit(1)
来源：http://qk.muxihuayi.cn

Ruby: exit 1
来源：http://ez.yuexingan06.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sm.yuexingan06.cn

[M06] 向标准错误输出
来源：http://vp.shxzskj.cn

Py:   print("err", file=sys.stderr)
来源：http://io.newstarts.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://uo.asd995.cn

JS:   console.error("err")
来源：http://jr.shtwfgs.cn

TS:   console.error("err")
来源：http://yt.shxzskj.cn

Java: System.err.println("err")
来源：http://km.shtwfgs.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ij.asd995.cn

Ruby: warn "err"
来源：http://ha.nszjky.cn

C#:   Console.Error.WriteLine("err")
来源：http://el.muxihuayi.cn

[M07] 判断是否为主入口
来源：http://ei.chemitech.net.cn

Py:   if __name__ == "__main__":
来源：http://hw.521024.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://no.bookmarksfly.cn

JS:   require.main === module
来源：http://sx.jctech888.com.cn

TS:   require.main === module
来源：http://iw.9csxet.cn

Java: public static void main(String[] args)
来源：http://kq.panjiajie.cn

Go:   func main()
来源：http://in.nicolike.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xu.bookmarksfly.cn

C#:   static void Main(string[] args)
来源：http://gk.jctech888.com.cn

[M08] 获取系统与运行时信息
来源：http://px.hnjuh.cn

Py:   platform.system();  platform.python_version()
来源：http://ma.9csxet.cn

PHP:  PHP_OS;  phpversion();
来源：http://wd.muxihuayi.cn

JS:   process.platform;  process.version
来源：http://hk.haigaiapp.cn

TS:   process.platform;  process.version
来源：http://pu.yuntaijiaju.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yw.521024.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://el.szxytkj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wy.hahajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bf.shxzskj.cn

================================================================================
来源：http://mn.wgjwhj.cn

N. 数据结构与算法
来源：http://rc.lnxyls.cn

================================================================================
来源：http://wn.colortex.cn

[N01] 二分查找（有序数组）
来源：http://vd.szxytkj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fi.asd995.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ft.szxytkj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kn.wgjwhj.cn


<!-- 参考信息 -->