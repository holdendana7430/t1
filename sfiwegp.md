代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ay.shxzskj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mg.szsharing.cn

[J05] 时间加减（加 7 天）
来源：http://kf.colortex.cn

Py:   now + timedelta(days=7)
来源：http://mm.gzmigu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jt.hahajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://iz.haigaiapp.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fq.yuntaijiaju.cn

Java: LocalDate.now().plusDays(7)
来源：http://ik.hahajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cp.jctech888.com.cn

Ruby: Time.now + 7 * 86400
来源：http://kb.shtwfgs.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bt.asd995.cn

[J06] 计算两时间之差
来源：http://pz.gzmigu.cn

Py:   (end - start).total_seconds()
来源：http://we.hnjuh.cn

PHP:  $end->diff($start)->days;
来源：http://cj.lnxyls.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gb.nicolike.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mf.colortex.cn

Java: Duration.between(start, end).toSeconds()
来源：http://iw.bjjhwx.cn

Go:   end.Sub(start).Hours()
来源：http://wv.jianghongdianzi.cn

Ruby: end - start                 # 返回秒数
来源：http://qo.jctech888.com.cn

C#:   (end - start).TotalSeconds
来源：http://uu.shtwfgs.cn

[J07] 比较两个日期
来源：http://km.huixinmuqiang.cn

Py:   d1 < d2;  d1 == d2
来源：http://gu.shxzukj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mi.huanxung.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lp.panjiajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ae.haigaiapp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nw.bjjhwx.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bx.shxzukj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xo.jianghongdianzi.cn

C#:   d1 < d2;  d1 == d2
来源：http://ib.lnxyls.cn

[J08] 提取年月日与星期
来源：http://lr.jctech888.com.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://eg.shxzukj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sk.wgjwhj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fz.nszjky.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hs.bjjhwx.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mj.huixiangedu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hl.haigaiapp.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kq.lnxyls.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yp.hahajie.cn

[J09] 时区处理
来源：http://sv.huixinmuqiang.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vw.newstarts.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wl.hahajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rh.chemitech.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tk.shxzukj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xf.bookmarksfly.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mk.asd995.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://iq.9csxet.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fd.panjiajie.cn

[J10] 取今天 / 本月第一天
来源：http://gt.521024.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tq.521024.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ca.yuntaijiaju.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sh.newstarts.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hc.huanxung.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qr.huanxung.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jw.gzmigu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rm.newstarts.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://br.hnjuh.cn

================================================================================
来源：http://ho.hnjuh.cn

K. JSON 与序列化
来源：http://ad.bookmarksfly.cn

================================================================================
来源：http://iz.muxihuayi.cn

[K01] 对象转 JSON 字符串
来源：http://kh.nszjky.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gt.9csxet.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lt.muxihuayi.cn

JS:   JSON.stringify(obj)
来源：http://ks.lnxyls.cn

TS:   JSON.stringify(obj)
来源：http://wa.yuntaijiaju.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xp.nszjky.cn

Go:   json.Marshal(obj)
来源：http://em.bookmarksfly.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ll.hahajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://to.gzmigu.cn

[K02] JSON 字符串转对象
来源：http://fj.colortex.cn

Py:   json.loads(s)
来源：http://ym.muxihuayi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ma.newstarts.cn

JS:   JSON.parse(s)
来源：http://oq.haigaiapp.cn

TS:   JSON.parse(s)
来源：http://ic.yuexingan06.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ul.szsharing.cn

Go:   json.Unmarshal(data, &v)
来源：http://gh.hnjuh.cn

Ruby: JSON.parse(s)
来源：http://cs.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ju.huanxung.cn

[K03] JSON 美化输出（带缩进）
来源：http://ze.muxihuayi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ac.521024.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xm.huanxung.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://mt.asd995.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mq.hnjuh.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zv.huixinmuqiang.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hw.szxytkj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://tm.lnxyls.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kp.bookmarksfly.cn

[K04] 读取 JSON 文件
来源：http://mq.shxzukj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ev.huixinmuqiang.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fi.jianghongdianzi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iq.521024.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wx.gzmigu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://br.colortex.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dm.muxihuayi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rq.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hq.szsharing.cn

[K05] 深拷贝对象
来源：http://hw.colortex.cn

Py:   copy.deepcopy(obj)
来源：http://ua.nszjky.cn

PHP:  unserialize(serialize($obj));
来源：http://lm.huanxung.cn

JS:   structuredClone(obj)
来源：http://wf.huixinmuqiang.cn

TS:   structuredClone(obj)
来源：http://xd.lnxyls.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qg.bjjhwx.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ho.shxzukj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hl.yuntaijiaju.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tm.muxihuayi.cn

[K06] 解析 URL 查询串
来源：http://yf.wgjwhj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qq.jctech888.com.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://er.jctech888.com.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qq.muxihuayi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nl.gzmigu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://la.shxzskj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pk.jianghongdianzi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qf.haigaiapp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xn.jctech888.com.cn

[K07] 进制转换
来源：http://py.yuntaijiaju.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xj.bookmarksfly.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uw.shtwfgs.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vg.shxzskj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nm.asd995.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://oe.jianghongdianzi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mq.521024.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ee.9csxet.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nb.gzmigu.cn

[K08] 二进制序列化（非 JSON）
来源：http://gy.szxytkj.cn

Py:   pickle.dumps(obj)
来源：http://qi.521024.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sm.huixiangedu.cn

JS:   v8.serialize(obj)        // Node
来源：http://rb.nicolike.cn

TS:   v8.serialize(obj)        // Node
来源：http://au.szxytkj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gh.huanxung.cn

Go:   encoding/gob
来源：http://ob.bjjhwx.cn

Ruby: Marshal.dump(obj)
来源：http://ol.szxytkj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://au.9csxet.cn

================================================================================
来源：http://hd.szxytkj.cn

L. 网络请求
来源：http://fv.jianghongdianzi.cn

================================================================================
来源：http://qp.shtwfgs.cn

[L01] 发送 GET 请求
来源：http://ja.wgjwhj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zz.bjjhwx.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ik.szxytkj.cn

JS:   await fetch(url)
来源：http://ta.gzmigu.cn

TS:   await fetch(url)
来源：http://us.bookmarksfly.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://og.asd995.cn

Go:   resp, err := http.Get(url)
来源：http://ax.huanxung.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ny.huixinmuqiang.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hx.chemitech.net.cn

[L02] 发送 POST JSON
来源：http://re.bjjhwx.cn

Py:   requests.post(url, json={"a": 1})
来源：http://we.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://la.szsharing.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://be.huixinmuqiang.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qg.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mx.9csxet.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lz.huixinmuqiang.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lq.huixiangedu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dt.hahajie.cn

[L03] 设置自定义请求头
来源：http://gg.yuntaijiaju.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cx.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lv.hnjuh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fx.huixiangedu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ui.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gj.hnjuh.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ck.newstarts.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://eh.colortex.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gx.bookmarksfly.cn

[L04] 设置超时
来源：http://rz.bookmarksfly.cn

Py:   requests.get(url, timeout=5)
来源：http://hd.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ky.wgjwhj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zg.gzmigu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xj.gzmigu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tm.asd995.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ha.lnxyls.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ov.chemitech.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dl.hnjuh.cn

[L05] 上传文件（multipart）
来源：http://yg.panjiajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xd.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jx.bjjhwx.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tx.shxzskj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mm.nicolike.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mq.szsharing.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fz.szsharing.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sl.huixinmuqiang.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://de.lnxyls.cn

[L06] 解析响应为 JSON
来源：http://iz.9csxet.cn

Py:   resp.json()
来源：http://wl.panjiajie.cn

PHP:  json_decode($body, true);
来源：http://ks.huixiangedu.cn

JS:   await resp.json()
来源：http://iw.9csxet.cn

TS:   await resp.json()
来源：http://kq.521024.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hc.wgjwhj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ju.haigaiapp.cn

Ruby: JSON.parse(resp.body)
来源：http://tt.nicolike.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yn.yuntaijiaju.cn

[L07] 处理 HTTP 状态码
来源：http://fy.jianghongdianzi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zl.newstarts.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mu.jianghongdianzi.cn

JS:   resp.ok;  resp.status
来源：http://mz.huanxung.cn

TS:   resp.ok;  resp.status
来源：http://xg.lnxyls.cn

Java: resp.statusCode()
来源：http://mj.chemitech.net.cn

Go:   resp.StatusCode
来源：http://jm.hahajie.cn

Ruby: resp.code.to_i
来源：http://ic.newstarts.cn

C#:   (int)resp.StatusCode
来源：http://ha.nicolike.cn

[L08] 并发请求多个地址
来源：http://te.colortex.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yv.bookmarksfly.cn

PHP:  curl_multi_init() 系列
来源：http://zd.bjjhwx.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jb.bjjhwx.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qz.chemitech.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bs.bjjhwx.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yx.hahajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ga.haigaiapp.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rs.shtwfgs.cn

================================================================================
来源：http://yb.lnxyls.cn

M. 命令行 / 进程 / 环境
来源：http://zi.huixinmuqiang.cn

================================================================================
来源：http://pl.panjiajie.cn

[M01] 读取命令行参数
来源：http://vl.shxzskj.cn

Py:   sys.argv[1:]
来源：http://mf.nszjky.cn

PHP:  $argv;  $argc;
来源：http://ig.lnxyls.cn

JS:   process.argv.slice(2)
来源：http://hi.muxihuayi.cn

TS:   process.argv.slice(2)
来源：http://qx.bookmarksfly.cn

Java: args 数组（main 方法参数）
来源：http://zf.huixinmuqiang.cn

Go:   os.Args[1:]
来源：http://ng.asd995.cn

Ruby: ARGV
来源：http://gx.shtwfgs.cn

C#:   args 数组（Main 方法参数）
来源：http://ox.huixinmuqiang.cn

[M02] 读取环境变量
来源：http://fg.wgjwhj.cn

Py:   os.environ.get("HOME")
来源：http://rh.shtwfgs.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://au.9csxet.cn

JS:   process.env.HOME
来源：http://kl.bookmarksfly.cn

TS:   process.env.HOME
来源：http://xv.jianghongdianzi.cn

Java: System.getenv("HOME")
来源：http://fs.lnxyls.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qa.shtwfgs.cn

Ruby: ENV["HOME"]
来源：http://tx.yuntaijiaju.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ug.gzmigu.cn

[M03] 执行外部命令
来源：http://nw.asd995.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://oo.yuexingan06.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ns.yuntaijiaju.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://yw.lnxyls.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qw.nszjky.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fn.asd995.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://eb.nszjky.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jk.bjjhwx.cn

C#:   Process.Start("ls", "-l");
来源：http://im.jianghongdianzi.cn

[M04] 获取当前工作目录
来源：http://ri.shtwfgs.cn

Py:   os.getcwd()
来源：http://jh.yuexingan06.cn

PHP:  getcwd();
来源：http://fj.gzmigu.cn

JS:   process.cwd()
来源：http://xy.asd995.cn

TS:   process.cwd()
来源：http://ab.521024.cn

Java: Path.of("").toAbsolutePath()
来源：http://ki.asd995.cn

Go:   os.Getwd()
来源：http://ky.lnxyls.cn

Ruby: Dir.pwd
来源：http://pv.lnxyls.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qy.521024.cn

[M05] 设置退出码
来源：http://ji.huixiangedu.cn

Py:   sys.exit(1)
来源：http://cn.wgjwhj.cn

PHP:  exit(1);
来源：http://nx.shxzukj.cn

JS:   process.exit(1)
来源：http://qv.nszjky.cn

TS:   process.exit(1)
来源：http://ln.shxzskj.cn

Java: System.exit(1)
来源：http://ey.bjjhwx.cn

Go:   os.Exit(1)
来源：http://ui.nszjky.cn

Ruby: exit 1
来源：http://la.muxihuayi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gy.muxihuayi.cn

[M06] 向标准错误输出
来源：http://tg.haigaiapp.cn

Py:   print("err", file=sys.stderr)
来源：http://aa.shxzukj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lx.muxihuayi.cn

JS:   console.error("err")
来源：http://kr.colortex.cn

TS:   console.error("err")
来源：http://dr.shxzskj.cn

Java: System.err.println("err")
来源：http://fw.szsharing.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nq.newstarts.cn

Ruby: warn "err"
来源：http://id.chemitech.net.cn

C#:   Console.Error.WriteLine("err")
来源：http://nz.chemitech.net.cn

[M07] 判断是否为主入口
来源：http://ue.shxzukj.cn

Py:   if __name__ == "__main__":
来源：http://ke.bookmarksfly.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ur.wgjwhj.cn

JS:   require.main === module
来源：http://rw.colortex.cn

TS:   require.main === module
来源：http://ck.shxzukj.cn

Java: public static void main(String[] args)
来源：http://zz.yuexingan06.cn

Go:   func main()
来源：http://du.hahajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nf.yuntaijiaju.cn

C#:   static void Main(string[] args)
来源：http://wi.haigaiapp.cn

[M08] 获取系统与运行时信息
来源：http://ys.lnxyls.cn

Py:   platform.system();  platform.python_version()
来源：http://vo.szsharing.cn

PHP:  PHP_OS;  phpversion();
来源：http://zi.nszjky.cn

JS:   process.platform;  process.version
来源：http://vv.huixiangedu.cn

TS:   process.platform;  process.version
来源：http://ef.bookmarksfly.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zs.shxzskj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xr.colortex.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ir.jianghongdianzi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zr.wgjwhj.cn

================================================================================
来源：http://qw.haigaiapp.cn

N. 数据结构与算法
来源：http://tt.bjjhwx.cn

================================================================================
来源：http://tq.colortex.cn

[N01] 二分查找（有序数组）
来源：http://dl.shxzskj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qj.chemitech.net.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sj.9csxet.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gi.colortex.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pf.wgjwhj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://vg.panjiajie.cn

Go:   sort.SearchInts(arr, x)
来源：http://lc.gzmigu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://sq.shtwfgs.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wg.panjiajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://zy.shtwfgs.cn

Py:   sorted(arr);  arr.sort()
来源：http://mb.colortex.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ok.haigaiapp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gc.szxytkj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ag.lnxyls.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://oh.haigaiapp.cn

Go:   slices.Sort(arr)
来源：http://ec.bjjhwx.cn


<!-- 参考信息 -->