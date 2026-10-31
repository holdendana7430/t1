代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wh.huixinmuqiang.cn

[J04] 时间戳与日期互转
来源：http://cq.colortex.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dt.panjiajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uc.lnxyls.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mk.jctech888.com.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xv.szxytkj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vg.hnjuh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qo.haigaiapp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tu.huixinmuqiang.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pb.haigaiapp.cn

[J05] 时间加减（加 7 天）
来源：http://gy.szsharing.cn

Py:   now + timedelta(days=7)
来源：http://si.panjiajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sn.bjjhwx.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zg.jctech888.com.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ns.gzmigu.cn

Java: LocalDate.now().plusDays(7)
来源：http://ba.wgjwhj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nn.newstarts.cn

Ruby: Time.now + 7 * 86400
来源：http://tu.nszjky.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ze.hnjuh.cn

[J06] 计算两时间之差
来源：http://vp.yuexingan06.cn

Py:   (end - start).total_seconds()
来源：http://hg.wgjwhj.cn

PHP:  $end->diff($start)->days;
来源：http://yc.521024.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ae.lnxyls.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ll.wgjwhj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zo.chemitech.net.cn

Go:   end.Sub(start).Hours()
来源：http://no.bjjhwx.cn

Ruby: end - start                 # 返回秒数
来源：http://wn.yuexingan06.cn

C#:   (end - start).TotalSeconds
来源：http://ft.huixiangedu.cn

[J07] 比较两个日期
来源：http://uv.muxihuayi.cn

Py:   d1 < d2;  d1 == d2
来源：http://sq.chemitech.net.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bb.huanxung.cn

JS:   d1.getTime() < d2.getTime()
来源：http://me.yuntaijiaju.cn

TS:   d1.getTime() < d2.getTime()
来源：http://tm.521024.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qn.muxihuayi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fo.jianghongdianzi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://nu.huanxung.cn

C#:   d1 < d2;  d1 == d2
来源：http://uq.nszjky.cn

[J08] 提取年月日与星期
来源：http://iq.gzmigu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hf.hnjuh.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fw.bjjhwx.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://to.jianghongdianzi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://sl.yuexingan06.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zj.huanxung.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xr.yuexingan06.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xm.bookmarksfly.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mb.colortex.cn

[J09] 时区处理
来源：http://xt.gzmigu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vb.yuexingan06.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ko.muxihuayi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kl.nszjky.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ko.colortex.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bx.huixiangedu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ys.szsharing.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gw.colortex.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://eg.yuntaijiaju.cn

[J10] 取今天 / 本月第一天
来源：http://ts.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://js.hnjuh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://up.bookmarksfly.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cy.gzmigu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qo.muxihuayi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jp.jctech888.com.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://oh.newstarts.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ch.shtwfgs.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bn.bjjhwx.cn

================================================================================
来源：http://wv.gzmigu.cn

K. JSON 与序列化
来源：http://qv.asd995.cn

================================================================================
来源：http://lg.huixiangedu.cn

[K01] 对象转 JSON 字符串
来源：http://gc.huixinmuqiang.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gw.shxzskj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yi.bjjhwx.cn

JS:   JSON.stringify(obj)
来源：http://sv.colortex.cn

TS:   JSON.stringify(obj)
来源：http://nw.huanxung.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lx.jianghongdianzi.cn

Go:   json.Marshal(obj)
来源：http://cz.bookmarksfly.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xr.asd995.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ie.huanxung.cn

[K02] JSON 字符串转对象
来源：http://ko.huixiangedu.cn

Py:   json.loads(s)
来源：http://eq.bookmarksfly.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gm.szxytkj.cn

JS:   JSON.parse(s)
来源：http://tn.hnjuh.cn

TS:   JSON.parse(s)
来源：http://tm.521024.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nr.9csxet.cn

Go:   json.Unmarshal(data, &v)
来源：http://zj.huanxung.cn

Ruby: JSON.parse(s)
来源：http://af.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yu.huixiangedu.cn

[K03] JSON 美化输出（带缩进）
来源：http://sj.muxihuayi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ne.lnxyls.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ii.hnjuh.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wy.gzmigu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://jr.bjjhwx.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wi.szxytkj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bn.wgjwhj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ii.colortex.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ba.chemitech.net.cn

[K04] 读取 JSON 文件
来源：http://rm.huixinmuqiang.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wv.asd995.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gj.bookmarksfly.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xe.huixinmuqiang.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xq.huanxung.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://eh.9csxet.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ew.9csxet.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mg.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://el.gzmigu.cn

[K05] 深拷贝对象
来源：http://ll.wgjwhj.cn

Py:   copy.deepcopy(obj)
来源：http://ch.shxzukj.cn

PHP:  unserialize(serialize($obj));
来源：http://st.panjiajie.cn

JS:   structuredClone(obj)
来源：http://ue.newstarts.cn

TS:   structuredClone(obj)
来源：http://ks.gzmigu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gw.jianghongdianzi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bj.9csxet.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lm.szsharing.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mm.chemitech.net.cn

[K06] 解析 URL 查询串
来源：http://is.shtwfgs.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tr.panjiajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rq.9csxet.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dw.chemitech.net.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tv.521024.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hu.yuexingan06.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zs.jctech888.com.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yh.chemitech.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lx.jctech888.com.cn

[K07] 进制转换
来源：http://cx.bjjhwx.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yh.newstarts.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tw.shxzukj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cp.wgjwhj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yu.bjjhwx.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gw.gzmigu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fd.chemitech.net.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hi.huanxung.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pj.nszjky.cn

[K08] 二进制序列化（非 JSON）
来源：http://hk.wgjwhj.cn

Py:   pickle.dumps(obj)
来源：http://yt.bjjhwx.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ny.wgjwhj.cn

JS:   v8.serialize(obj)        // Node
来源：http://qm.huixinmuqiang.cn

TS:   v8.serialize(obj)        // Node
来源：http://sd.bjjhwx.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jq.shxzskj.cn

Go:   encoding/gob
来源：http://sz.hahajie.cn

Ruby: Marshal.dump(obj)
来源：http://aq.shtwfgs.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nk.nszjky.cn

================================================================================
来源：http://qm.gzmigu.cn

L. 网络请求
来源：http://tk.shtwfgs.cn

================================================================================
来源：http://bg.huanxung.cn

[L01] 发送 GET 请求
来源：http://de.asd995.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sg.lnxyls.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uz.jianghongdianzi.cn

JS:   await fetch(url)
来源：http://dr.yuntaijiaju.cn

TS:   await fetch(url)
来源：http://nm.9csxet.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yi.hnjuh.cn

Go:   resp, err := http.Get(url)
来源：http://tj.jctech888.com.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://iu.bjjhwx.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://td.9csxet.cn

[L02] 发送 POST JSON
来源：http://mx.hnjuh.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nv.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://by.shxzskj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://le.yuntaijiaju.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pd.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ro.szxytkj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kf.panjiajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://it.jianghongdianzi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xm.lnxyls.cn

[L03] 设置自定义请求头
来源：http://fj.jianghongdianzi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ue.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rp.szsharing.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kj.bookmarksfly.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vm.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mp.shxzskj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://oo.wgjwhj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cj.gzmigu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bt.wgjwhj.cn

[L04] 设置超时
来源：http://nj.haigaiapp.cn

Py:   requests.get(url, timeout=5)
来源：http://pi.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rt.bjjhwx.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qg.szxytkj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oi.huanxung.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mk.hnjuh.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kg.shxzukj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mt.jianghongdianzi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xu.jctech888.com.cn

[L05] 上传文件（multipart）
来源：http://vm.521024.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ba.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://et.jianghongdianzi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xx.lnxyls.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sc.hnjuh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jj.jianghongdianzi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ht.521024.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nd.panjiajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wy.huixiangedu.cn

[L06] 解析响应为 JSON
来源：http://zz.wgjwhj.cn

Py:   resp.json()
来源：http://ja.hahajie.cn

PHP:  json_decode($body, true);
来源：http://bi.newstarts.cn

JS:   await resp.json()
来源：http://bl.muxihuayi.cn

TS:   await resp.json()
来源：http://nk.asd995.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xw.nicolike.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kl.bjjhwx.cn

Ruby: JSON.parse(resp.body)
来源：http://nl.wgjwhj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://en.asd995.cn

[L07] 处理 HTTP 状态码
来源：http://gj.huixiangedu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tn.asd995.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qg.bjjhwx.cn

JS:   resp.ok;  resp.status
来源：http://kp.szsharing.cn

TS:   resp.ok;  resp.status
来源：http://wh.haigaiapp.cn

Java: resp.statusCode()
来源：http://xa.hahajie.cn

Go:   resp.StatusCode
来源：http://vv.jctech888.com.cn

Ruby: resp.code.to_i
来源：http://ap.9csxet.cn

C#:   (int)resp.StatusCode
来源：http://wd.huixinmuqiang.cn

[L08] 并发请求多个地址
来源：http://ys.szsharing.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qa.muxihuayi.cn

PHP:  curl_multi_init() 系列
来源：http://nt.colortex.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ia.szsharing.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qw.panjiajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fo.muxihuayi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lm.wgjwhj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tc.colortex.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ix.yuexingan06.cn

================================================================================
来源：http://ya.nicolike.cn

M. 命令行 / 进程 / 环境
来源：http://vp.nszjky.cn

================================================================================
来源：http://yn.huanxung.cn

[M01] 读取命令行参数
来源：http://pd.hnjuh.cn

Py:   sys.argv[1:]
来源：http://ao.lnxyls.cn

PHP:  $argv;  $argc;
来源：http://uu.jianghongdianzi.cn

JS:   process.argv.slice(2)
来源：http://id.newstarts.cn

TS:   process.argv.slice(2)
来源：http://eb.shtwfgs.cn

Java: args 数组（main 方法参数）
来源：http://ka.newstarts.cn

Go:   os.Args[1:]
来源：http://ow.haigaiapp.cn

Ruby: ARGV
来源：http://rn.huixiangedu.cn

C#:   args 数组（Main 方法参数）
来源：http://pv.bookmarksfly.cn

[M02] 读取环境变量
来源：http://ha.panjiajie.cn

Py:   os.environ.get("HOME")
来源：http://ij.newstarts.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jt.colortex.cn

JS:   process.env.HOME
来源：http://rk.panjiajie.cn

TS:   process.env.HOME
来源：http://bn.shxzskj.cn

Java: System.getenv("HOME")
来源：http://ni.huixinmuqiang.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dw.gzmigu.cn

Ruby: ENV["HOME"]
来源：http://ev.chemitech.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nq.yuexingan06.cn

[M03] 执行外部命令
来源：http://st.panjiajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nt.bookmarksfly.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fv.shxzskj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ta.panjiajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://my.asd995.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wq.panjiajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://sk.jctech888.com.cn

Ruby: system("ls -l");  `ls -l`
来源：http://dy.bjjhwx.cn

C#:   Process.Start("ls", "-l");
来源：http://oq.shxzukj.cn

[M04] 获取当前工作目录
来源：http://ef.szsharing.cn

Py:   os.getcwd()
来源：http://uf.9csxet.cn

PHP:  getcwd();
来源：http://mf.asd995.cn

JS:   process.cwd()
来源：http://ni.szxytkj.cn

TS:   process.cwd()
来源：http://vo.panjiajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://hs.shxzskj.cn

Go:   os.Getwd()
来源：http://hv.szxytkj.cn

Ruby: Dir.pwd
来源：http://lv.bjjhwx.cn

C#:   Directory.GetCurrentDirectory()
来源：http://en.colortex.cn

[M05] 设置退出码
来源：http://vc.nszjky.cn

Py:   sys.exit(1)
来源：http://ze.bookmarksfly.cn

PHP:  exit(1);
来源：http://gv.szsharing.cn

JS:   process.exit(1)
来源：http://yx.jctech888.com.cn

TS:   process.exit(1)
来源：http://or.huixiangedu.cn

Java: System.exit(1)
来源：http://tz.panjiajie.cn

Go:   os.Exit(1)
来源：http://cc.szxytkj.cn

Ruby: exit 1
来源：http://ma.szxytkj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gd.shtwfgs.cn

[M06] 向标准错误输出
来源：http://xr.hahajie.cn

Py:   print("err", file=sys.stderr)
来源：http://lj.wgjwhj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bu.szsharing.cn

JS:   console.error("err")
来源：http://qs.haigaiapp.cn

TS:   console.error("err")
来源：http://tz.chemitech.net.cn

Java: System.err.println("err")
来源：http://mr.muxihuayi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://st.jctech888.com.cn

Ruby: warn "err"
来源：http://hb.muxihuayi.cn

C#:   Console.Error.WriteLine("err")
来源：http://cx.newstarts.cn

[M07] 判断是否为主入口
来源：http://kp.hahajie.cn

Py:   if __name__ == "__main__":
来源：http://zk.hnjuh.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://va.huixiangedu.cn

JS:   require.main === module
来源：http://yh.hahajie.cn

TS:   require.main === module
来源：http://va.bjjhwx.cn

Java: public static void main(String[] args)
来源：http://fy.chemitech.net.cn

Go:   func main()
来源：http://mg.huixinmuqiang.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ay.muxihuayi.cn

C#:   static void Main(string[] args)
来源：http://zs.colortex.cn

[M08] 获取系统与运行时信息
来源：http://on.newstarts.cn

Py:   platform.system();  platform.python_version()
来源：http://yd.asd995.cn

PHP:  PHP_OS;  phpversion();
来源：http://rn.szsharing.cn

JS:   process.platform;  process.version
来源：http://fy.shxzskj.cn

TS:   process.platform;  process.version
来源：http://ox.521024.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qy.nicolike.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mv.asd995.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zh.yuexingan06.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://im.yuntaijiaju.cn

================================================================================
来源：http://lr.muxihuayi.cn

N. 数据结构与算法
来源：http://tz.521024.cn

================================================================================
来源：http://po.yuexingan06.cn

[N01] 二分查找（有序数组）
来源：http://xq.jianghongdianzi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://pf.panjiajie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tz.huanxung.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bl.yuntaijiaju.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yi.jctech888.com.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wo.asd995.cn

Go:   sort.SearchInts(arr, x)
来源：http://gh.gzmigu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://di.gzmigu.cn


<!-- 参考信息 -->