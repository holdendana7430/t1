代发 wailian999

TS:   new Date("2024-01-02")
来源：http://ha.chemitech.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fg.bookmarksfly.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tj.shtwfgs.cn

Ruby: Date.parse("2024-01-02")
来源：http://ki.shtwfgs.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fj.nicolike.cn

[J04] 时间戳与日期互转
来源：http://sm.huixiangedu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jy.yuntaijiaju.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://to.gzmigu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ny.shxzukj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://nz.yuexingan06.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ok.9csxet.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://em.nszjky.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ma.chemitech.net.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sg.521024.cn

[J05] 时间加减（加 7 天）
来源：http://go.shxzskj.cn

Py:   now + timedelta(days=7)
来源：http://qe.bookmarksfly.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xu.colortex.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bj.nszjky.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mb.newstarts.cn

Java: LocalDate.now().plusDays(7)
来源：http://ae.shxzskj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tv.muxihuayi.cn

Ruby: Time.now + 7 * 86400
来源：http://zx.521024.cn

C#:   DateTime.Now.AddDays(7)
来源：http://fi.wgjwhj.cn

[J06] 计算两时间之差
来源：http://jh.hahajie.cn

Py:   (end - start).total_seconds()
来源：http://jo.shxzskj.cn

PHP:  $end->diff($start)->days;
来源：http://jf.shxzukj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pa.muxihuayi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uq.chemitech.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mm.hnjuh.cn

Go:   end.Sub(start).Hours()
来源：http://ph.huixiangedu.cn

Ruby: end - start                 # 返回秒数
来源：http://ve.shxzskj.cn

C#:   (end - start).TotalSeconds
来源：http://tb.newstarts.cn

[J07] 比较两个日期
来源：http://vv.haigaiapp.cn

Py:   d1 < d2;  d1 == d2
来源：http://rf.hnjuh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mb.yuntaijiaju.cn

JS:   d1.getTime() < d2.getTime()
来源：http://go.haigaiapp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://op.szxytkj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ee.jianghongdianzi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fi.jctech888.com.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fn.asd995.cn

C#:   d1 < d2;  d1 == d2
来源：http://vy.lnxyls.cn

[J08] 提取年月日与星期
来源：http://zg.jctech888.com.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xa.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://le.bjjhwx.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hy.muxihuayi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jm.asd995.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ni.muxihuayi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qe.muxihuayi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yl.haigaiapp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xi.szxytkj.cn

[J09] 时区处理
来源：http://ri.wgjwhj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qk.newstarts.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xd.nszjky.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://de.gzmigu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nm.9csxet.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ui.szxytkj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ow.gzmigu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://as.yuexingan06.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tz.huixinmuqiang.cn

[J10] 取今天 / 本月第一天
来源：http://eb.wgjwhj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kp.newstarts.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://if.shxzukj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ui.yuntaijiaju.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ec.szxytkj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qx.bookmarksfly.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fh.lnxyls.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gp.yuntaijiaju.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pt.shxzskj.cn

================================================================================
来源：http://ac.jianghongdianzi.cn

K. JSON 与序列化
来源：http://mn.jctech888.com.cn

================================================================================
来源：http://vx.panjiajie.cn

[K01] 对象转 JSON 字符串
来源：http://xb.nszjky.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gd.shxzskj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rs.nicolike.cn

JS:   JSON.stringify(obj)
来源：http://cw.shxzskj.cn

TS:   JSON.stringify(obj)
来源：http://qf.hnjuh.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lp.521024.cn

Go:   json.Marshal(obj)
来源：http://ew.huanxung.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fk.shxzukj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://kg.gzmigu.cn

[K02] JSON 字符串转对象
来源：http://ne.jianghongdianzi.cn

Py:   json.loads(s)
来源：http://kt.newstarts.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mc.shxzskj.cn

JS:   JSON.parse(s)
来源：http://fy.bookmarksfly.cn

TS:   JSON.parse(s)
来源：http://oe.jianghongdianzi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cl.newstarts.cn

Go:   json.Unmarshal(data, &v)
来源：http://sz.hahajie.cn

Ruby: JSON.parse(s)
来源：http://ts.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qu.szsharing.cn

[K03] JSON 美化输出（带缩进）
来源：http://vj.yuexingan06.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ta.asd995.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gj.panjiajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ie.shtwfgs.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://eu.hahajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dc.szsharing.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ul.jctech888.com.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dh.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jx.asd995.cn

[K04] 读取 JSON 文件
来源：http://gj.panjiajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cy.panjiajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://or.panjiajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hj.lnxyls.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mp.gzmigu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dy.gzmigu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://op.shxzskj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zb.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qy.szsharing.cn

[K05] 深拷贝对象
来源：http://si.bjjhwx.cn

Py:   copy.deepcopy(obj)
来源：http://us.wgjwhj.cn

PHP:  unserialize(serialize($obj));
来源：http://ra.szxytkj.cn

JS:   structuredClone(obj)
来源：http://vd.hahajie.cn

TS:   structuredClone(obj)
来源：http://xs.gzmigu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fl.shxzskj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kv.newstarts.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bs.jctech888.com.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wy.hnjuh.cn

[K06] 解析 URL 查询串
来源：http://oy.szsharing.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tg.nicolike.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://so.wgjwhj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lk.huixinmuqiang.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://my.shxzskj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zt.haigaiapp.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bg.hahajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://se.bookmarksfly.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vb.gzmigu.cn

[K07] 进制转换
来源：http://dh.chemitech.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fv.jianghongdianzi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jh.wgjwhj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kj.huixiangedu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zv.colortex.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fz.jctech888.com.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tj.huanxung.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://og.gzmigu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tx.9csxet.cn

[K08] 二进制序列化（非 JSON）
来源：http://tc.shxzskj.cn

Py:   pickle.dumps(obj)
来源：http://bq.asd995.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mz.hahajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://xw.muxihuayi.cn

TS:   v8.serialize(obj)        // Node
来源：http://ws.hnjuh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yn.yuexingan06.cn

Go:   encoding/gob
来源：http://kr.szsharing.cn

Ruby: Marshal.dump(obj)
来源：http://rl.bjjhwx.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dv.yuexingan06.cn

================================================================================
来源：http://he.chemitech.net.cn

L. 网络请求
来源：http://cu.nicolike.cn

================================================================================
来源：http://up.huanxung.cn

[L01] 发送 GET 请求
来源：http://lq.wgjwhj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cx.521024.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://su.shxzskj.cn

JS:   await fetch(url)
来源：http://sv.jctech888.com.cn

TS:   await fetch(url)
来源：http://os.haigaiapp.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ct.shtwfgs.cn

Go:   resp, err := http.Get(url)
来源：http://yz.jctech888.com.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://tc.bookmarksfly.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fj.gzmigu.cn

[L02] 发送 POST JSON
来源：http://xb.lnxyls.cn

Py:   requests.post(url, json={"a": 1})
来源：http://lm.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jd.gzmigu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kr.huixiangedu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ui.asd995.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vc.muxihuayi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ga.haigaiapp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zk.jianghongdianzi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xh.bjjhwx.cn

[L03] 设置自定义请求头
来源：http://im.haigaiapp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ic.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fb.chemitech.net.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bw.muxihuayi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ec.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lc.hahajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bp.shxzukj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kj.szxytkj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bl.muxihuayi.cn

[L04] 设置超时
来源：http://sg.521024.cn

Py:   requests.get(url, timeout=5)
来源：http://cc.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rq.9csxet.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ob.colortex.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sv.newstarts.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qd.muxihuayi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bw.jctech888.com.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://iw.muxihuayi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jc.szsharing.cn

[L05] 上传文件（multipart）
来源：http://dz.wgjwhj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mf.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vv.shxzskj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ns.wgjwhj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nk.shxzukj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://km.yuntaijiaju.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qo.9csxet.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fw.yuexingan06.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gp.lnxyls.cn

[L06] 解析响应为 JSON
来源：http://xg.asd995.cn

Py:   resp.json()
来源：http://wf.shtwfgs.cn

PHP:  json_decode($body, true);
来源：http://pq.hnjuh.cn

JS:   await resp.json()
来源：http://dw.wgjwhj.cn

TS:   await resp.json()
来源：http://cc.panjiajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sz.szxytkj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jk.bjjhwx.cn

Ruby: JSON.parse(resp.body)
来源：http://pe.yuntaijiaju.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vn.jianghongdianzi.cn

[L07] 处理 HTTP 状态码
来源：http://hc.huixiangedu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mn.haigaiapp.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hj.bjjhwx.cn

JS:   resp.ok;  resp.status
来源：http://yf.9csxet.cn

TS:   resp.ok;  resp.status
来源：http://mf.huixiangedu.cn

Java: resp.statusCode()
来源：http://fj.yuntaijiaju.cn

Go:   resp.StatusCode
来源：http://ax.newstarts.cn

Ruby: resp.code.to_i
来源：http://re.nszjky.cn

C#:   (int)resp.StatusCode
来源：http://yr.jctech888.com.cn

[L08] 并发请求多个地址
来源：http://wo.chemitech.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hv.huanxung.cn

PHP:  curl_multi_init() 系列
来源：http://gv.gzmigu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lm.huixiangedu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zb.jianghongdianzi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qs.szsharing.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lh.nszjky.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gr.hnjuh.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gt.shtwfgs.cn

================================================================================
来源：http://qd.shxzukj.cn

M. 命令行 / 进程 / 环境
来源：http://tz.bjjhwx.cn

================================================================================
来源：http://wm.huixiangedu.cn

[M01] 读取命令行参数
来源：http://zw.gzmigu.cn

Py:   sys.argv[1:]
来源：http://hy.nicolike.cn

PHP:  $argv;  $argc;
来源：http://qe.9csxet.cn

JS:   process.argv.slice(2)
来源：http://eh.chemitech.net.cn

TS:   process.argv.slice(2)
来源：http://vk.jctech888.com.cn

Java: args 数组（main 方法参数）
来源：http://ea.jianghongdianzi.cn

Go:   os.Args[1:]
来源：http://ud.gzmigu.cn

Ruby: ARGV
来源：http://oy.yuexingan06.cn

C#:   args 数组（Main 方法参数）
来源：http://qw.9csxet.cn

[M02] 读取环境变量
来源：http://qg.muxihuayi.cn

Py:   os.environ.get("HOME")
来源：http://gj.huixiangedu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tx.huanxung.cn

JS:   process.env.HOME
来源：http://fp.gzmigu.cn

TS:   process.env.HOME
来源：http://yx.521024.cn

Java: System.getenv("HOME")
来源：http://sq.lnxyls.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jx.haigaiapp.cn

Ruby: ENV["HOME"]
来源：http://il.asd995.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yv.521024.cn

[M03] 执行外部命令
来源：http://tu.huixiangedu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hl.nszjky.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pu.wgjwhj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://en.lnxyls.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vv.newstarts.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yy.521024.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xc.huanxung.cn

Ruby: system("ls -l");  `ls -l`
来源：http://la.gzmigu.cn

C#:   Process.Start("ls", "-l");
来源：http://no.nszjky.cn

[M04] 获取当前工作目录
来源：http://uf.lnxyls.cn

Py:   os.getcwd()
来源：http://ed.colortex.cn

PHP:  getcwd();
来源：http://ug.szxytkj.cn

JS:   process.cwd()
来源：http://py.szxytkj.cn

TS:   process.cwd()
来源：http://kg.szsharing.cn

Java: Path.of("").toAbsolutePath()
来源：http://ax.colortex.cn

Go:   os.Getwd()
来源：http://gn.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://yo.bjjhwx.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gl.hnjuh.cn

[M05] 设置退出码
来源：http://dx.lnxyls.cn

Py:   sys.exit(1)
来源：http://ns.521024.cn

PHP:  exit(1);
来源：http://al.jctech888.com.cn

JS:   process.exit(1)
来源：http://hi.huixiangedu.cn

TS:   process.exit(1)
来源：http://vo.nszjky.cn

Java: System.exit(1)
来源：http://lu.bjjhwx.cn

Go:   os.Exit(1)
来源：http://ee.newstarts.cn

Ruby: exit 1
来源：http://ju.yuntaijiaju.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bl.shxzskj.cn

[M06] 向标准错误输出
来源：http://cp.jianghongdianzi.cn

Py:   print("err", file=sys.stderr)
来源：http://yw.colortex.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://zb.wgjwhj.cn

JS:   console.error("err")
来源：http://mo.nicolike.cn

TS:   console.error("err")
来源：http://ao.asd995.cn

Java: System.err.println("err")
来源：http://vj.lnxyls.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pu.szsharing.cn

Ruby: warn "err"
来源：http://pt.huixiangedu.cn

C#:   Console.Error.WriteLine("err")
来源：http://bv.9csxet.cn

[M07] 判断是否为主入口
来源：http://oi.huixiangedu.cn

Py:   if __name__ == "__main__":
来源：http://mw.wgjwhj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cs.szsharing.cn

JS:   require.main === module
来源：http://wi.szsharing.cn

TS:   require.main === module
来源：http://qm.gzmigu.cn

Java: public static void main(String[] args)
来源：http://rg.bookmarksfly.cn

Go:   func main()
来源：http://yw.haigaiapp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pr.jctech888.com.cn

C#:   static void Main(string[] args)
来源：http://kk.szxytkj.cn

[M08] 获取系统与运行时信息
来源：http://eg.shxzskj.cn

Py:   platform.system();  platform.python_version()
来源：http://tq.gzmigu.cn

PHP:  PHP_OS;  phpversion();
来源：http://fh.shxzskj.cn

JS:   process.platform;  process.version
来源：http://yr.jctech888.com.cn

TS:   process.platform;  process.version
来源：http://ts.newstarts.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mf.newstarts.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://eb.panjiajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://un.hahajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://hg.panjiajie.cn

================================================================================
来源：http://lg.huixiangedu.cn

N. 数据结构与算法
来源：http://ig.huixinmuqiang.cn

================================================================================
来源：http://hy.nszjky.cn

[N01] 二分查找（有序数组）
来源：http://zz.chemitech.net.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hn.newstarts.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jo.huixiangedu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mm.asd995.cn


<!-- 参考信息 -->