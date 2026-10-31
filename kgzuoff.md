代发 wailian999

TS:   new Date("2024-01-02")
来源：http://ad.jctech888.com.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mm.huixinmuqiang.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ud.muxihuayi.cn

Ruby: Date.parse("2024-01-02")
来源：http://rs.chemitech.net.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cs.panjiajie.cn

[J04] 时间戳与日期互转
来源：http://mz.bjjhwx.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jr.huixinmuqiang.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ng.wgjwhj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://we.9csxet.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wb.521024.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://em.shtwfgs.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zr.yuexingan06.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zp.chemitech.net.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://uj.huixiangedu.cn

[J05] 时间加减（加 7 天）
来源：http://ib.colortex.cn

Py:   now + timedelta(days=7)
来源：http://wb.hahajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://hj.nicolike.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://am.yuntaijiaju.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sv.jianghongdianzi.cn

Java: LocalDate.now().plusDays(7)
来源：http://ix.yuntaijiaju.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yv.wgjwhj.cn

Ruby: Time.now + 7 * 86400
来源：http://uz.hnjuh.cn

C#:   DateTime.Now.AddDays(7)
来源：http://fl.bookmarksfly.cn

[J06] 计算两时间之差
来源：http://rn.huixinmuqiang.cn

Py:   (end - start).total_seconds()
来源：http://tq.haigaiapp.cn

PHP:  $end->diff($start)->days;
来源：http://lx.jctech888.com.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ca.nszjky.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://il.bjjhwx.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ur.szsharing.cn

Go:   end.Sub(start).Hours()
来源：http://je.shxzukj.cn

Ruby: end - start                 # 返回秒数
来源：http://zj.szxytkj.cn

C#:   (end - start).TotalSeconds
来源：http://yg.huanxung.cn

[J07] 比较两个日期
来源：http://qv.shxzukj.cn

Py:   d1 < d2;  d1 == d2
来源：http://bf.nszjky.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://da.haigaiapp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wi.muxihuayi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rd.huanxung.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ih.szsharing.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ff.jianghongdianzi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qb.huixiangedu.cn

C#:   d1 < d2;  d1 == d2
来源：http://zi.gzmigu.cn

[J08] 提取年月日与星期
来源：http://el.gzmigu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lm.shtwfgs.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sj.shxzskj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zv.asd995.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://go.muxihuayi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ns.chemitech.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mz.lnxyls.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://of.shtwfgs.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uq.bookmarksfly.cn

[J09] 时区处理
来源：http://nd.chemitech.net.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ku.gzmigu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://po.gzmigu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fj.nszjky.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hp.chemitech.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hg.yuexingan06.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bb.9csxet.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fk.szsharing.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ny.bookmarksfly.cn

[J10] 取今天 / 本月第一天
来源：http://vs.shxzukj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ds.asd995.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://eq.yuntaijiaju.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vt.nicolike.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://op.haigaiapp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ih.shxzskj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bt.9csxet.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zl.hahajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://df.huanxung.cn

================================================================================
来源：http://fz.shtwfgs.cn

K. JSON 与序列化
来源：http://iq.9csxet.cn

================================================================================
来源：http://mi.asd995.cn

[K01] 对象转 JSON 字符串
来源：http://ux.shtwfgs.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://po.hnjuh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vu.jianghongdianzi.cn

JS:   JSON.stringify(obj)
来源：http://pd.asd995.cn

TS:   JSON.stringify(obj)
来源：http://on.bjjhwx.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hr.shtwfgs.cn

Go:   json.Marshal(obj)
来源：http://vo.shxzskj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ec.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://tm.newstarts.cn

[K02] JSON 字符串转对象
来源：http://tz.nicolike.cn

Py:   json.loads(s)
来源：http://ig.yuntaijiaju.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zw.shxzukj.cn

JS:   JSON.parse(s)
来源：http://gq.haigaiapp.cn

TS:   JSON.parse(s)
来源：http://fb.bjjhwx.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ym.haigaiapp.cn

Go:   json.Unmarshal(data, &v)
来源：http://co.shxzskj.cn

Ruby: JSON.parse(s)
来源：http://lb.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lh.huixiangedu.cn

[K03] JSON 美化输出（带缩进）
来源：http://qt.shtwfgs.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wc.yuexingan06.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wb.shxzskj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wo.panjiajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://px.lnxyls.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hc.shtwfgs.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dj.bjjhwx.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jc.szsharing.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ac.panjiajie.cn

[K04] 读取 JSON 文件
来源：http://sm.yuntaijiaju.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qx.hnjuh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pi.szxytkj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gd.hnjuh.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qm.9csxet.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rb.9csxet.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://aq.panjiajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://tt.asd995.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sl.jctech888.com.cn

[K05] 深拷贝对象
来源：http://ly.chemitech.net.cn

Py:   copy.deepcopy(obj)
来源：http://sk.521024.cn

PHP:  unserialize(serialize($obj));
来源：http://jb.newstarts.cn

JS:   structuredClone(obj)
来源：http://yd.bookmarksfly.cn

TS:   structuredClone(obj)
来源：http://xv.gzmigu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xc.jianghongdianzi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lf.yuntaijiaju.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jx.muxihuayi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://os.nszjky.cn

[K06] 解析 URL 查询串
来源：http://ky.bookmarksfly.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nx.nszjky.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mk.colortex.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lp.panjiajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nn.huanxung.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qx.shxzskj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dg.yuntaijiaju.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ax.521024.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bu.panjiajie.cn

[K07] 进制转换
来源：http://xe.hahajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hq.shxzskj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fu.huixiangedu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bu.panjiajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://iv.shxzskj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sl.shxzskj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rq.jctech888.com.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tk.asd995.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uq.bjjhwx.cn

[K08] 二进制序列化（非 JSON）
来源：http://ps.yuntaijiaju.cn

Py:   pickle.dumps(obj)
来源：http://qo.szsharing.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://rq.shxzskj.cn

JS:   v8.serialize(obj)        // Node
来源：http://cb.panjiajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://qy.hahajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://of.jctech888.com.cn

Go:   encoding/gob
来源：http://vr.huixiangedu.cn

Ruby: Marshal.dump(obj)
来源：http://qa.newstarts.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ke.bjjhwx.cn

================================================================================
来源：http://lh.haigaiapp.cn

L. 网络请求
来源：http://cj.gzmigu.cn

================================================================================
来源：http://ku.shtwfgs.cn

[L01] 发送 GET 请求
来源：http://zz.9csxet.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://as.nszjky.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lq.nszjky.cn

JS:   await fetch(url)
来源：http://vf.asd995.cn

TS:   await fetch(url)
来源：http://ff.yuexingan06.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kl.wgjwhj.cn

Go:   resp, err := http.Get(url)
来源：http://iq.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://si.wgjwhj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pn.521024.cn

[L02] 发送 POST JSON
来源：http://uy.jctech888.com.cn

Py:   requests.post(url, json={"a": 1})
来源：http://yr.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wf.szxytkj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qe.chemitech.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jg.asd995.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jm.newstarts.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ry.nszjky.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lj.bookmarksfly.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lz.bookmarksfly.cn

[L03] 设置自定义请求头
来源：http://dc.panjiajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bq.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ss.shxzukj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sv.nszjky.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mk.colortex.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fs.asd995.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qv.shxzukj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fc.gzmigu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zl.521024.cn

[L04] 设置超时
来源：http://fh.muxihuayi.cn

Py:   requests.get(url, timeout=5)
来源：http://oj.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bp.huixiangedu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wy.wgjwhj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vt.shtwfgs.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qn.jianghongdianzi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ae.lnxyls.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://im.huanxung.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ws.chemitech.net.cn

[L05] 上传文件（multipart）
来源：http://ll.jianghongdianzi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uh.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wm.haigaiapp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wb.huanxung.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ed.bookmarksfly.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cf.newstarts.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yx.shxzukj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yv.colortex.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pt.9csxet.cn

[L06] 解析响应为 JSON
来源：http://ln.panjiajie.cn

Py:   resp.json()
来源：http://jm.jianghongdianzi.cn

PHP:  json_decode($body, true);
来源：http://eb.newstarts.cn

JS:   await resp.json()
来源：http://iu.521024.cn

TS:   await resp.json()
来源：http://ic.9csxet.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xq.shtwfgs.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rl.hnjuh.cn

Ruby: JSON.parse(resp.body)
来源：http://vy.wgjwhj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jz.yuexingan06.cn

[L07] 处理 HTTP 状态码
来源：http://pj.muxihuayi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cl.nicolike.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sd.shxzskj.cn

JS:   resp.ok;  resp.status
来源：http://eq.huixinmuqiang.cn

TS:   resp.ok;  resp.status
来源：http://hq.muxihuayi.cn

Java: resp.statusCode()
来源：http://nw.asd995.cn

Go:   resp.StatusCode
来源：http://vb.yuntaijiaju.cn

Ruby: resp.code.to_i
来源：http://te.colortex.cn

C#:   (int)resp.StatusCode
来源：http://ix.asd995.cn

[L08] 并发请求多个地址
来源：http://np.jctech888.com.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gx.haigaiapp.cn

PHP:  curl_multi_init() 系列
来源：http://zw.bookmarksfly.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cz.colortex.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://di.shxzukj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ta.lnxyls.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dk.yuexingan06.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ow.nszjky.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mc.huixiangedu.cn

================================================================================
来源：http://ns.521024.cn

M. 命令行 / 进程 / 环境
来源：http://yg.panjiajie.cn

================================================================================
来源：http://ow.asd995.cn

[M01] 读取命令行参数
来源：http://nf.nicolike.cn

Py:   sys.argv[1:]
来源：http://je.shxzukj.cn

PHP:  $argv;  $argc;
来源：http://xk.shtwfgs.cn

JS:   process.argv.slice(2)
来源：http://sk.yuexingan06.cn

TS:   process.argv.slice(2)
来源：http://mr.panjiajie.cn

Java: args 数组（main 方法参数）
来源：http://or.huixiangedu.cn

Go:   os.Args[1:]
来源：http://jh.yuexingan06.cn

Ruby: ARGV
来源：http://mq.gzmigu.cn

C#:   args 数组（Main 方法参数）
来源：http://jt.bjjhwx.cn

[M02] 读取环境变量
来源：http://da.asd995.cn

Py:   os.environ.get("HOME")
来源：http://tf.bjjhwx.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vo.wgjwhj.cn

JS:   process.env.HOME
来源：http://gx.asd995.cn

TS:   process.env.HOME
来源：http://hi.521024.cn

Java: System.getenv("HOME")
来源：http://qn.gzmigu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qf.huanxung.cn

Ruby: ENV["HOME"]
来源：http://hw.jianghongdianzi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nm.asd995.cn

[M03] 执行外部命令
来源：http://ul.shtwfgs.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fv.chemitech.net.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fv.gzmigu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hf.szsharing.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ev.yuexingan06.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ak.haigaiapp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jy.haigaiapp.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kw.szxytkj.cn

C#:   Process.Start("ls", "-l");
来源：http://os.newstarts.cn

[M04] 获取当前工作目录
来源：http://jv.yuntaijiaju.cn

Py:   os.getcwd()
来源：http://rp.jianghongdianzi.cn

PHP:  getcwd();
来源：http://ez.shxzskj.cn

JS:   process.cwd()
来源：http://ij.hnjuh.cn

TS:   process.cwd()
来源：http://um.wgjwhj.cn

Java: Path.of("").toAbsolutePath()
来源：http://op.jianghongdianzi.cn

Go:   os.Getwd()
来源：http://vo.szsharing.cn

Ruby: Dir.pwd
来源：http://we.colortex.cn

C#:   Directory.GetCurrentDirectory()
来源：http://kb.huanxung.cn

[M05] 设置退出码
来源：http://kr.hahajie.cn

Py:   sys.exit(1)
来源：http://iv.gzmigu.cn

PHP:  exit(1);
来源：http://mj.wgjwhj.cn

JS:   process.exit(1)
来源：http://hm.shtwfgs.cn

TS:   process.exit(1)
来源：http://lk.yuntaijiaju.cn

Java: System.exit(1)
来源：http://ub.colortex.cn

Go:   os.Exit(1)
来源：http://nx.panjiajie.cn

Ruby: exit 1
来源：http://yl.asd995.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zx.bjjhwx.cn

[M06] 向标准错误输出
来源：http://yf.hnjuh.cn

Py:   print("err", file=sys.stderr)
来源：http://nk.lnxyls.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://aj.9csxet.cn

JS:   console.error("err")
来源：http://nr.nszjky.cn

TS:   console.error("err")
来源：http://nb.szsharing.cn

Java: System.err.println("err")
来源：http://tk.szxytkj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ap.nszjky.cn

Ruby: warn "err"
来源：http://ek.szsharing.cn

C#:   Console.Error.WriteLine("err")
来源：http://iw.yuexingan06.cn

[M07] 判断是否为主入口
来源：http://ce.chemitech.net.cn

Py:   if __name__ == "__main__":
来源：http://ev.9csxet.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bj.huixiangedu.cn

JS:   require.main === module
来源：http://so.hahajie.cn

TS:   require.main === module
来源：http://xf.huixiangedu.cn

Java: public static void main(String[] args)
来源：http://cy.bjjhwx.cn

Go:   func main()
来源：http://on.huixiangedu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hq.hnjuh.cn

C#:   static void Main(string[] args)
来源：http://pe.9csxet.cn

[M08] 获取系统与运行时信息
来源：http://li.lnxyls.cn

Py:   platform.system();  platform.python_version()
来源：http://ib.hahajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://ad.panjiajie.cn

JS:   process.platform;  process.version
来源：http://gh.shxzskj.cn

TS:   process.platform;  process.version
来源：http://of.shxzskj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gf.panjiajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://nr.bookmarksfly.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://my.shtwfgs.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://hf.hnjuh.cn

================================================================================
来源：http://yd.colortex.cn

N. 数据结构与算法
来源：http://rm.yuntaijiaju.cn

================================================================================
来源：http://dv.yuntaijiaju.cn

[N01] 二分查找（有序数组）
来源：http://hi.szsharing.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zi.asd995.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://eh.huixinmuqiang.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cl.muxihuayi.cn


<!-- 参考信息 -->