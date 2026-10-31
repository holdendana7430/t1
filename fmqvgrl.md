代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rj.huixinmuqiang.cn

[J04] 时间戳与日期互转
来源：http://hq.colortex.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fx.chemitech.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zj.nicolike.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pi.shxzskj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://pk.chemitech.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kw.asd995.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://oz.bookmarksfly.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pv.wgjwhj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zb.jianghongdianzi.cn

[J05] 时间加减（加 7 天）
来源：http://wi.hahajie.cn

Py:   now + timedelta(days=7)
来源：http://xi.521024.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nr.bookmarksfly.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wc.shxzskj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xt.shxzukj.cn

Java: LocalDate.now().plusDays(7)
来源：http://is.szxytkj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uy.9csxet.cn

Ruby: Time.now + 7 * 86400
来源：http://qu.haigaiapp.cn

C#:   DateTime.Now.AddDays(7)
来源：http://tx.jianghongdianzi.cn

[J06] 计算两时间之差
来源：http://wu.9csxet.cn

Py:   (end - start).total_seconds()
来源：http://gd.gzmigu.cn

PHP:  $end->diff($start)->days;
来源：http://rw.lnxyls.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rq.shxzukj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sm.shxzukj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mg.bookmarksfly.cn

Go:   end.Sub(start).Hours()
来源：http://eo.bookmarksfly.cn

Ruby: end - start                 # 返回秒数
来源：http://bq.yuntaijiaju.cn

C#:   (end - start).TotalSeconds
来源：http://pa.nszjky.cn

[J07] 比较两个日期
来源：http://ad.shxzskj.cn

Py:   d1 < d2;  d1 == d2
来源：http://ro.szxytkj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vb.521024.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ey.panjiajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://sn.bjjhwx.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ae.bjjhwx.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rt.gzmigu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://px.lnxyls.cn

C#:   d1 < d2;  d1 == d2
来源：http://ox.lnxyls.cn

[J08] 提取年月日与星期
来源：http://qe.shxzukj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cl.nszjky.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ak.chemitech.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pa.szsharing.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uo.yuexingan06.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sj.yuexingan06.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cp.shxzukj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cq.hahajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qw.gzmigu.cn

[J09] 时区处理
来源：http://fe.muxihuayi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dk.shtwfgs.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ck.521024.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qv.shtwfgs.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dr.wgjwhj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wa.nicolike.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hq.colortex.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qx.hahajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ss.yuntaijiaju.cn

[J10] 取今天 / 本月第一天
来源：http://zu.jctech888.com.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fb.huanxung.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pj.panjiajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pw.9csxet.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gw.szsharing.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cg.hnjuh.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rn.colortex.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rw.shxzskj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oy.chemitech.net.cn

================================================================================
来源：http://yd.shxzukj.cn

K. JSON 与序列化
来源：http://tc.szxytkj.cn

================================================================================
来源：http://ud.shtwfgs.cn

[K01] 对象转 JSON 字符串
来源：http://kk.yuntaijiaju.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wx.nszjky.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gx.chemitech.net.cn

JS:   JSON.stringify(obj)
来源：http://kf.gzmigu.cn

TS:   JSON.stringify(obj)
来源：http://ae.9csxet.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zx.asd995.cn

Go:   json.Marshal(obj)
来源：http://ed.shxzukj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://uz.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://te.nszjky.cn

[K02] JSON 字符串转对象
来源：http://hh.newstarts.cn

Py:   json.loads(s)
来源：http://ky.521024.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ch.szxytkj.cn

JS:   JSON.parse(s)
来源：http://hx.bookmarksfly.cn

TS:   JSON.parse(s)
来源：http://aq.panjiajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cz.yuexingan06.cn

Go:   json.Unmarshal(data, &v)
来源：http://ih.huixiangedu.cn

Ruby: JSON.parse(s)
来源：http://wo.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://db.huanxung.cn

[K03] JSON 美化输出（带缩进）
来源：http://ii.521024.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://at.asd995.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mc.nicolike.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gb.bjjhwx.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ex.shxzukj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ac.huixiangedu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xc.bookmarksfly.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nf.newstarts.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xr.panjiajie.cn

[K04] 读取 JSON 文件
来源：http://zd.hnjuh.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://aq.chemitech.net.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xh.wgjwhj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bc.shtwfgs.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://po.huanxung.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://te.nszjky.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gj.huixinmuqiang.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://iy.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ty.szxytkj.cn

[K05] 深拷贝对象
来源：http://lo.jctech888.com.cn

Py:   copy.deepcopy(obj)
来源：http://ov.bookmarksfly.cn

PHP:  unserialize(serialize($obj));
来源：http://xq.bjjhwx.cn

JS:   structuredClone(obj)
来源：http://gf.gzmigu.cn

TS:   structuredClone(obj)
来源：http://it.jianghongdianzi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bi.hnjuh.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ro.chemitech.net.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sc.lnxyls.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vl.huixiangedu.cn

[K06] 解析 URL 查询串
来源：http://zw.bjjhwx.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://we.huixiangedu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ac.huixiangedu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rx.jianghongdianzi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ch.haigaiapp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ym.asd995.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mi.9csxet.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bv.shxzukj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pk.huixiangedu.cn

[K07] 进制转换
来源：http://xz.jianghongdianzi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nc.huixinmuqiang.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bq.chemitech.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cl.shxzskj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lb.shtwfgs.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ks.hahajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ms.jianghongdianzi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sj.bookmarksfly.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://po.szsharing.cn

[K08] 二进制序列化（非 JSON）
来源：http://ra.bookmarksfly.cn

Py:   pickle.dumps(obj)
来源：http://mm.szxytkj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mh.9csxet.cn

JS:   v8.serialize(obj)        // Node
来源：http://ez.nicolike.cn

TS:   v8.serialize(obj)        // Node
来源：http://ct.huixiangedu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ee.szsharing.cn

Go:   encoding/gob
来源：http://tu.lnxyls.cn

Ruby: Marshal.dump(obj)
来源：http://aw.chemitech.net.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.szsharing.cn

================================================================================
来源：http://yb.nicolike.cn

L. 网络请求
来源：http://dl.shxzskj.cn

================================================================================
来源：http://hp.jianghongdianzi.cn

[L01] 发送 GET 请求
来源：http://ac.521024.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fz.panjiajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://id.bjjhwx.cn

JS:   await fetch(url)
来源：http://ov.asd995.cn

TS:   await fetch(url)
来源：http://ws.yuntaijiaju.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ev.hnjuh.cn

Go:   resp, err := http.Get(url)
来源：http://hq.wgjwhj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qv.bjjhwx.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tl.szxytkj.cn

[L02] 发送 POST JSON
来源：http://oq.huanxung.cn

Py:   requests.post(url, json={"a": 1})
来源：http://dr.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://aj.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://to.haigaiapp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vb.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vp.colortex.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ib.lnxyls.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dv.hnjuh.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gt.huixiangedu.cn

[L03] 设置自定义请求头
来源：http://xx.haigaiapp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rj.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bn.huanxung.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rq.jctech888.com.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qx.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ni.szsharing.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vq.bjjhwx.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ah.gzmigu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kc.bjjhwx.cn

[L04] 设置超时
来源：http://sa.newstarts.cn

Py:   requests.get(url, timeout=5)
来源：http://tr.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ab.szxytkj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fr.nicolike.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gc.newstarts.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vx.lnxyls.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://js.yuexingan06.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hn.9csxet.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ka.wgjwhj.cn

[L05] 上传文件（multipart）
来源：http://kc.hnjuh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fg.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nj.hnjuh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uh.shxzukj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://to.shxzukj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kc.nszjky.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qd.jianghongdianzi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rg.yuexingan06.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://em.yuexingan06.cn

[L06] 解析响应为 JSON
来源：http://sm.yuexingan06.cn

Py:   resp.json()
来源：http://ty.muxihuayi.cn

PHP:  json_decode($body, true);
来源：http://uk.521024.cn

JS:   await resp.json()
来源：http://tv.shtwfgs.cn

TS:   await resp.json()
来源：http://jt.huixinmuqiang.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jv.bookmarksfly.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fw.chemitech.net.cn

Ruby: JSON.parse(resp.body)
来源：http://cf.hahajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zq.shxzskj.cn

[L07] 处理 HTTP 状态码
来源：http://on.521024.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xv.yuntaijiaju.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jb.shxzukj.cn

JS:   resp.ok;  resp.status
来源：http://qp.colortex.cn

TS:   resp.ok;  resp.status
来源：http://ns.haigaiapp.cn

Java: resp.statusCode()
来源：http://ez.shtwfgs.cn

Go:   resp.StatusCode
来源：http://is.huanxung.cn

Ruby: resp.code.to_i
来源：http://lq.521024.cn

C#:   (int)resp.StatusCode
来源：http://ke.hnjuh.cn

[L08] 并发请求多个地址
来源：http://zq.bookmarksfly.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xk.hnjuh.cn

PHP:  curl_multi_init() 系列
来源：http://lj.nszjky.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yw.yuntaijiaju.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tn.jianghongdianzi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ew.newstarts.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pd.shxzukj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qe.muxihuayi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zf.haigaiapp.cn

================================================================================
来源：http://ee.shtwfgs.cn

M. 命令行 / 进程 / 环境
来源：http://ax.jctech888.com.cn

================================================================================
来源：http://mt.gzmigu.cn

[M01] 读取命令行参数
来源：http://nb.hnjuh.cn

Py:   sys.argv[1:]
来源：http://yq.shxzukj.cn

PHP:  $argv;  $argc;
来源：http://nh.colortex.cn

JS:   process.argv.slice(2)
来源：http://nl.gzmigu.cn

TS:   process.argv.slice(2)
来源：http://mz.yuexingan06.cn

Java: args 数组（main 方法参数）
来源：http://gq.jctech888.com.cn

Go:   os.Args[1:]
来源：http://vj.jianghongdianzi.cn

Ruby: ARGV
来源：http://tg.jctech888.com.cn

C#:   args 数组（Main 方法参数）
来源：http://lg.wgjwhj.cn

[M02] 读取环境变量
来源：http://qy.shxzskj.cn

Py:   os.environ.get("HOME")
来源：http://tu.yuntaijiaju.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://li.huixinmuqiang.cn

JS:   process.env.HOME
来源：http://jv.chemitech.net.cn

TS:   process.env.HOME
来源：http://zj.newstarts.cn

Java: System.getenv("HOME")
来源：http://km.nicolike.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gt.huixinmuqiang.cn

Ruby: ENV["HOME"]
来源：http://ga.hahajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nw.muxihuayi.cn

[M03] 执行外部命令
来源：http://od.nicolike.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yu.huixiangedu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ds.nszjky.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://bu.lnxyls.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ap.yuexingan06.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mv.huixinmuqiang.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vj.521024.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xn.chemitech.net.cn

C#:   Process.Start("ls", "-l");
来源：http://yq.asd995.cn

[M04] 获取当前工作目录
来源：http://zu.gzmigu.cn

Py:   os.getcwd()
来源：http://nt.jctech888.com.cn

PHP:  getcwd();
来源：http://ei.gzmigu.cn

JS:   process.cwd()
来源：http://hd.yuntaijiaju.cn

TS:   process.cwd()
来源：http://uj.wgjwhj.cn

Java: Path.of("").toAbsolutePath()
来源：http://di.521024.cn

Go:   os.Getwd()
来源：http://kr.wgjwhj.cn

Ruby: Dir.pwd
来源：http://wd.szxytkj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jl.panjiajie.cn

[M05] 设置退出码
来源：http://rn.huixinmuqiang.cn

Py:   sys.exit(1)
来源：http://qk.haigaiapp.cn

PHP:  exit(1);
来源：http://bw.yuntaijiaju.cn

JS:   process.exit(1)
来源：http://sd.jianghongdianzi.cn

TS:   process.exit(1)
来源：http://cr.yuexingan06.cn

Java: System.exit(1)
来源：http://bk.muxihuayi.cn

Go:   os.Exit(1)
来源：http://xm.muxihuayi.cn

Ruby: exit 1
来源：http://me.szxytkj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dc.newstarts.cn

[M06] 向标准错误输出
来源：http://cb.chemitech.net.cn

Py:   print("err", file=sys.stderr)
来源：http://qs.szxytkj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rk.shxzukj.cn

JS:   console.error("err")
来源：http://qz.huixinmuqiang.cn

TS:   console.error("err")
来源：http://aa.jianghongdianzi.cn

Java: System.err.println("err")
来源：http://hc.asd995.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wx.newstarts.cn

Ruby: warn "err"
来源：http://dt.bjjhwx.cn

C#:   Console.Error.WriteLine("err")
来源：http://zm.bjjhwx.cn

[M07] 判断是否为主入口
来源：http://vl.bookmarksfly.cn

Py:   if __name__ == "__main__":
来源：http://hk.newstarts.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dl.nicolike.cn

JS:   require.main === module
来源：http://ft.jianghongdianzi.cn

TS:   require.main === module
来源：http://kq.nicolike.cn

Java: public static void main(String[] args)
来源：http://ov.huanxung.cn

Go:   func main()
来源：http://ts.szsharing.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fb.wgjwhj.cn

C#:   static void Main(string[] args)
来源：http://en.haigaiapp.cn

[M08] 获取系统与运行时信息
来源：http://nn.asd995.cn

Py:   platform.system();  platform.python_version()
来源：http://dv.gzmigu.cn

PHP:  PHP_OS;  phpversion();
来源：http://hc.9csxet.cn

JS:   process.platform;  process.version
来源：http://hh.bookmarksfly.cn

TS:   process.platform;  process.version
来源：http://hj.huixinmuqiang.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oq.nszjky.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xj.huixiangedu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cs.yuexingan06.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vh.521024.cn

================================================================================
来源：http://os.asd995.cn

N. 数据结构与算法
来源：http://ci.huixinmuqiang.cn

================================================================================
来源：http://kk.yuntaijiaju.cn

[N01] 二分查找（有序数组）
来源：http://xv.huanxung.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hq.colortex.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fs.hnjuh.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hv.yuntaijiaju.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ir.shtwfgs.cn

Java: Arrays.binarySearch(arr, x)
来源：http://id.hahajie.cn

Go:   sort.SearchInts(arr, x)
来源：http://xs.bookmarksfly.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mq.nszjky.cn


<!-- 参考信息 -->