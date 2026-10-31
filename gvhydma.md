代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ii.hahajie.cn

[J04] 时间戳与日期互转
来源：http://pv.newstarts.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gl.lnxyls.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hh.lnxyls.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kr.asd995.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ga.wgjwhj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://iu.szxytkj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kv.szxytkj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://we.nicolike.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ka.lnxyls.cn

[J05] 时间加减（加 7 天）
来源：http://lr.huixinmuqiang.cn

Py:   now + timedelta(days=7)
来源：http://jo.colortex.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yn.bookmarksfly.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://oq.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://py.yuntaijiaju.cn

Java: LocalDate.now().plusDays(7)
来源：http://tk.9csxet.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://in.chemitech.net.cn

Ruby: Time.now + 7 * 86400
来源：http://fw.panjiajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://nu.yuexingan06.cn

[J06] 计算两时间之差
来源：http://cl.huanxung.cn

Py:   (end - start).total_seconds()
来源：http://tg.jctech888.com.cn

PHP:  $end->diff($start)->days;
来源：http://rb.nszjky.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tb.haigaiapp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ll.jctech888.com.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fv.yuntaijiaju.cn

Go:   end.Sub(start).Hours()
来源：http://ol.asd995.cn

Ruby: end - start                 # 返回秒数
来源：http://vk.muxihuayi.cn

C#:   (end - start).TotalSeconds
来源：http://ij.gzmigu.cn

[J07] 比较两个日期
来源：http://fj.shxzskj.cn

Py:   d1 < d2;  d1 == d2
来源：http://cp.wgjwhj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://on.gzmigu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ll.chemitech.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zx.huixiangedu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lj.yuexingan06.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ov.huixiangedu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jf.muxihuayi.cn

C#:   d1 < d2;  d1 == d2
来源：http://zt.muxihuayi.cn

[J08] 提取年月日与星期
来源：http://ya.lnxyls.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hm.asd995.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cf.hnjuh.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wv.szsharing.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lj.asd995.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qu.9csxet.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ts.521024.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qe.huixiangedu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rn.hahajie.cn

[J09] 时区处理
来源：http://ds.shtwfgs.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ay.huixinmuqiang.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sr.9csxet.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sk.521024.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://it.521024.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ts.hahajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ep.9csxet.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ex.colortex.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yt.shxzskj.cn

[J10] 取今天 / 本月第一天
来源：http://ut.wgjwhj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://of.nszjky.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vc.shxzskj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://go.huixinmuqiang.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tw.yuntaijiaju.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yd.bookmarksfly.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cj.nicolike.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ce.muxihuayi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sl.szsharing.cn

================================================================================
来源：http://rm.yuexingan06.cn

K. JSON 与序列化
来源：http://wj.panjiajie.cn

================================================================================
来源：http://pp.nszjky.cn

[K01] 对象转 JSON 字符串
来源：http://yb.gzmigu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hp.shtwfgs.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mg.hahajie.cn

JS:   JSON.stringify(obj)
来源：http://dc.colortex.cn

TS:   JSON.stringify(obj)
来源：http://go.newstarts.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ze.haigaiapp.cn

Go:   json.Marshal(obj)
来源：http://up.gzmigu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wz.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://oc.colortex.cn

[K02] JSON 字符串转对象
来源：http://xs.huixiangedu.cn

Py:   json.loads(s)
来源：http://ee.hahajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://za.gzmigu.cn

JS:   JSON.parse(s)
来源：http://pz.haigaiapp.cn

TS:   JSON.parse(s)
来源：http://ab.bjjhwx.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qg.newstarts.cn

Go:   json.Unmarshal(data, &v)
来源：http://su.huanxung.cn

Ruby: JSON.parse(s)
来源：http://sa.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xs.wgjwhj.cn

[K03] JSON 美化输出（带缩进）
来源：http://pi.9csxet.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ac.newstarts.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sf.bookmarksfly.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wi.muxihuayi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://un.szsharing.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ue.szsharing.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wm.nszjky.cn

Ruby: JSON.pretty_generate(obj)
来源：http://is.521024.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://is.yuntaijiaju.cn

[K04] 读取 JSON 文件
来源：http://py.hnjuh.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://av.huixinmuqiang.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wi.jctech888.com.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zg.asd995.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kw.gzmigu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ap.asd995.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pd.lnxyls.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://iy.colortex.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ag.shxzukj.cn

[K05] 深拷贝对象
来源：http://hk.gzmigu.cn

Py:   copy.deepcopy(obj)
来源：http://kv.asd995.cn

PHP:  unserialize(serialize($obj));
来源：http://fa.huixinmuqiang.cn

JS:   structuredClone(obj)
来源：http://pb.hnjuh.cn

TS:   structuredClone(obj)
来源：http://ex.asd995.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xv.jctech888.com.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kl.wgjwhj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ik.hahajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lk.jctech888.com.cn

[K06] 解析 URL 查询串
来源：http://ym.huixiangedu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fb.yuntaijiaju.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fi.muxihuayi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fi.gzmigu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ai.yuexingan06.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mj.jianghongdianzi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://aq.muxihuayi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xp.szxytkj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ks.bookmarksfly.cn

[K07] 进制转换
来源：http://pc.haigaiapp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ig.shtwfgs.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kr.shxzukj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yf.muxihuayi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hp.haigaiapp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fa.chemitech.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://un.huanxung.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mc.huanxung.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://il.bjjhwx.cn

[K08] 二进制序列化（非 JSON）
来源：http://rp.lnxyls.cn

Py:   pickle.dumps(obj)
来源：http://ut.colortex.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mm.shtwfgs.cn

JS:   v8.serialize(obj)        // Node
来源：http://jw.szxytkj.cn

TS:   v8.serialize(obj)        // Node
来源：http://xx.yuntaijiaju.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ow.lnxyls.cn

Go:   encoding/gob
来源：http://om.shxzskj.cn

Ruby: Marshal.dump(obj)
来源：http://xc.yuexingan06.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ml.jianghongdianzi.cn

================================================================================
来源：http://px.jianghongdianzi.cn

L. 网络请求
来源：http://ow.yuntaijiaju.cn

================================================================================
来源：http://be.szsharing.cn

[L01] 发送 GET 请求
来源：http://ri.shtwfgs.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qg.huixinmuqiang.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qp.shxzskj.cn

JS:   await fetch(url)
来源：http://zs.bjjhwx.cn

TS:   await fetch(url)
来源：http://xv.shxzskj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hj.panjiajie.cn

Go:   resp, err := http.Get(url)
来源：http://ma.szxytkj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pk.hahajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ua.jctech888.com.cn

[L02] 发送 POST JSON
来源：http://nu.yuntaijiaju.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fn.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yd.szsharing.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kn.bjjhwx.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bg.colortex.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ze.hnjuh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zb.yuexingan06.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ub.huanxung.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dv.9csxet.cn

[L03] 设置自定义请求头
来源：http://kt.yuntaijiaju.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://my.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dv.panjiajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bp.huixiangedu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wn.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://as.panjiajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ck.lnxyls.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ww.yuntaijiaju.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fm.9csxet.cn

[L04] 设置超时
来源：http://bb.gzmigu.cn

Py:   requests.get(url, timeout=5)
来源：http://cc.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xd.asd995.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oj.shxzskj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kv.jctech888.com.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yn.nszjky.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gb.newstarts.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://oz.haigaiapp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ob.newstarts.cn

[L05] 上传文件（multipart）
来源：http://wc.szsharing.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ut.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tv.9csxet.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ga.jctech888.com.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bn.shxzskj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hb.yuntaijiaju.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gf.hnjuh.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kp.jianghongdianzi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://id.yuexingan06.cn

[L06] 解析响应为 JSON
来源：http://wn.szxytkj.cn

Py:   resp.json()
来源：http://bx.wgjwhj.cn

PHP:  json_decode($body, true);
来源：http://lp.bjjhwx.cn

JS:   await resp.json()
来源：http://xp.shxzukj.cn

TS:   await resp.json()
来源：http://jg.521024.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qq.panjiajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ck.haigaiapp.cn

Ruby: JSON.parse(resp.body)
来源：http://rz.shtwfgs.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ft.szsharing.cn

[L07] 处理 HTTP 状态码
来源：http://xa.bookmarksfly.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gj.hnjuh.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bv.szsharing.cn

JS:   resp.ok;  resp.status
来源：http://kp.huixinmuqiang.cn

TS:   resp.ok;  resp.status
来源：http://il.shtwfgs.cn

Java: resp.statusCode()
来源：http://zm.shtwfgs.cn

Go:   resp.StatusCode
来源：http://xs.bjjhwx.cn

Ruby: resp.code.to_i
来源：http://ek.haigaiapp.cn

C#:   (int)resp.StatusCode
来源：http://uo.shxzukj.cn

[L08] 并发请求多个地址
来源：http://qh.huanxung.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kr.nszjky.cn

PHP:  curl_multi_init() 系列
来源：http://bo.bookmarksfly.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gk.szxytkj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ip.huixinmuqiang.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bx.newstarts.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://av.gzmigu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ih.panjiajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xn.haigaiapp.cn

================================================================================
来源：http://po.lnxyls.cn

M. 命令行 / 进程 / 环境
来源：http://pd.jctech888.com.cn

================================================================================
来源：http://zl.wgjwhj.cn

[M01] 读取命令行参数
来源：http://te.jianghongdianzi.cn

Py:   sys.argv[1:]
来源：http://ax.bookmarksfly.cn

PHP:  $argv;  $argc;
来源：http://ml.colortex.cn

JS:   process.argv.slice(2)
来源：http://ly.nszjky.cn

TS:   process.argv.slice(2)
来源：http://ko.panjiajie.cn

Java: args 数组（main 方法参数）
来源：http://mc.hnjuh.cn

Go:   os.Args[1:]
来源：http://dn.newstarts.cn

Ruby: ARGV
来源：http://vc.shtwfgs.cn

C#:   args 数组（Main 方法参数）
来源：http://ci.nicolike.cn

[M02] 读取环境变量
来源：http://zq.haigaiapp.cn

Py:   os.environ.get("HOME")
来源：http://nd.szxytkj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xa.bjjhwx.cn

JS:   process.env.HOME
来源：http://yv.huixiangedu.cn

TS:   process.env.HOME
来源：http://gs.haigaiapp.cn

Java: System.getenv("HOME")
来源：http://qq.gzmigu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://br.panjiajie.cn

Ruby: ENV["HOME"]
来源：http://ap.chemitech.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sy.jctech888.com.cn

[M03] 执行外部命令
来源：http://hr.bjjhwx.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fm.shxzukj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ch.newstarts.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qh.jianghongdianzi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fd.szxytkj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mn.huixinmuqiang.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ic.wgjwhj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://sj.shxzskj.cn

C#:   Process.Start("ls", "-l");
来源：http://eu.hahajie.cn

[M04] 获取当前工作目录
来源：http://ql.nicolike.cn

Py:   os.getcwd()
来源：http://sj.9csxet.cn

PHP:  getcwd();
来源：http://qo.huixinmuqiang.cn

JS:   process.cwd()
来源：http://li.shxzskj.cn

TS:   process.cwd()
来源：http://cp.panjiajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://es.huixinmuqiang.cn

Go:   os.Getwd()
来源：http://id.521024.cn

Ruby: Dir.pwd
来源：http://ml.yuexingan06.cn

C#:   Directory.GetCurrentDirectory()
来源：http://li.wgjwhj.cn

[M05] 设置退出码
来源：http://ul.asd995.cn

Py:   sys.exit(1)
来源：http://zp.hnjuh.cn

PHP:  exit(1);
来源：http://ke.jianghongdianzi.cn

JS:   process.exit(1)
来源：http://or.huanxung.cn

TS:   process.exit(1)
来源：http://yj.nicolike.cn

Java: System.exit(1)
来源：http://dc.lnxyls.cn

Go:   os.Exit(1)
来源：http://zc.hahajie.cn

Ruby: exit 1
来源：http://od.gzmigu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jq.shxzskj.cn

[M06] 向标准错误输出
来源：http://wa.hnjuh.cn

Py:   print("err", file=sys.stderr)
来源：http://me.huanxung.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://js.wgjwhj.cn

JS:   console.error("err")
来源：http://at.szsharing.cn

TS:   console.error("err")
来源：http://zq.huixinmuqiang.cn

Java: System.err.println("err")
来源：http://ec.szsharing.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fy.panjiajie.cn

Ruby: warn "err"
来源：http://rf.hahajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://sp.yuexingan06.cn

[M07] 判断是否为主入口
来源：http://ux.asd995.cn

Py:   if __name__ == "__main__":
来源：http://pi.huixiangedu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mx.bookmarksfly.cn

JS:   require.main === module
来源：http://vw.hahajie.cn

TS:   require.main === module
来源：http://sy.chemitech.net.cn

Java: public static void main(String[] args)
来源：http://oc.jctech888.com.cn

Go:   func main()
来源：http://lr.wgjwhj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ri.521024.cn

C#:   static void Main(string[] args)
来源：http://id.jianghongdianzi.cn

[M08] 获取系统与运行时信息
来源：http://qo.hahajie.cn

Py:   platform.system();  platform.python_version()
来源：http://ii.521024.cn

PHP:  PHP_OS;  phpversion();
来源：http://zp.jctech888.com.cn

JS:   process.platform;  process.version
来源：http://ju.nszjky.cn

TS:   process.platform;  process.version
来源：http://ye.bookmarksfly.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yj.shxzukj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://lx.jctech888.com.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mv.yuntaijiaju.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://po.chemitech.net.cn

================================================================================
来源：http://ss.huixiangedu.cn

N. 数据结构与算法
来源：http://gi.asd995.cn

================================================================================
来源：http://dc.jctech888.com.cn

[N01] 二分查找（有序数组）
来源：http://no.huixinmuqiang.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sq.jianghongdianzi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mu.szxytkj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cg.hahajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pb.szsharing.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ah.jctech888.com.cn

Go:   sort.SearchInts(arr, x)
来源：http://cp.shxzskj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yb.bookmarksfly.cn


<!-- 参考信息 -->