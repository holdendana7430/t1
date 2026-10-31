代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ln.huixiangedu.cn

[J04] 时间戳与日期互转
来源：http://fp.chemitech.net.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://oz.huixinmuqiang.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pb.panjiajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dg.huixiangedu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vq.muxihuayi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://aw.szxytkj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vn.szxytkj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lw.panjiajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wb.521024.cn

[J05] 时间加减（加 7 天）
来源：http://dg.chemitech.net.cn

Py:   now + timedelta(days=7)
来源：http://rw.asd995.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ei.jctech888.com.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gk.wgjwhj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qp.nszjky.cn

Java: LocalDate.now().plusDays(7)
来源：http://kv.bookmarksfly.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://au.yuexingan06.cn

Ruby: Time.now + 7 * 86400
来源：http://ir.yuexingan06.cn

C#:   DateTime.Now.AddDays(7)
来源：http://re.nszjky.cn

[J06] 计算两时间之差
来源：http://fl.521024.cn

Py:   (end - start).total_seconds()
来源：http://yc.haigaiapp.cn

PHP:  $end->diff($start)->days;
来源：http://aq.9csxet.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ub.jctech888.com.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sd.9csxet.cn

Java: Duration.between(start, end).toSeconds()
来源：http://oz.huixiangedu.cn

Go:   end.Sub(start).Hours()
来源：http://eb.shxzskj.cn

Ruby: end - start                 # 返回秒数
来源：http://ho.shxzskj.cn

C#:   (end - start).TotalSeconds
来源：http://sz.chemitech.net.cn

[J07] 比较两个日期
来源：http://yp.nszjky.cn

Py:   d1 < d2;  d1 == d2
来源：http://er.yuexingan06.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zo.chemitech.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://da.hnjuh.cn

TS:   d1.getTime() < d2.getTime()
来源：http://lb.nicolike.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gf.hahajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://an.hahajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xs.chemitech.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://qw.szsharing.cn

[J08] 提取年月日与星期
来源：http://aq.yuexingan06.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lf.nszjky.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fd.muxihuayi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pl.hahajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://my.jctech888.com.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://st.yuexingan06.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mt.wgjwhj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cj.bookmarksfly.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yd.nicolike.cn

[J09] 时区处理
来源：http://ig.huanxung.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ld.asd995.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jq.shxzskj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nd.shxzukj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hu.huixinmuqiang.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yw.muxihuayi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qg.huixiangedu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ba.yuexingan06.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dc.shtwfgs.cn

[J10] 取今天 / 本月第一天
来源：http://gp.jctech888.com.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kt.yuntaijiaju.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hy.bookmarksfly.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ol.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ov.lnxyls.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nf.haigaiapp.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ar.muxihuayi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vi.521024.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://af.jctech888.com.cn

================================================================================
来源：http://oe.wgjwhj.cn

K. JSON 与序列化
来源：http://ls.jctech888.com.cn

================================================================================
来源：http://sr.nszjky.cn

[K01] 对象转 JSON 字符串
来源：http://ur.nszjky.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vv.haigaiapp.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ns.jctech888.com.cn

JS:   JSON.stringify(obj)
来源：http://el.yuntaijiaju.cn

TS:   JSON.stringify(obj)
来源：http://pw.hahajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ro.huanxung.cn

Go:   json.Marshal(obj)
来源：http://fs.jctech888.com.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bv.asd995.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://md.nicolike.cn

[K02] JSON 字符串转对象
来源：http://ye.chemitech.net.cn

Py:   json.loads(s)
来源：http://uu.bookmarksfly.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://si.chemitech.net.cn

JS:   JSON.parse(s)
来源：http://xk.chemitech.net.cn

TS:   JSON.parse(s)
来源：http://cd.huixiangedu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wz.shxzskj.cn

Go:   json.Unmarshal(data, &v)
来源：http://oc.nicolike.cn

Ruby: JSON.parse(s)
来源：http://qw.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bl.bjjhwx.cn

[K03] JSON 美化输出（带缩进）
来源：http://ml.nicolike.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tk.muxihuayi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rx.huixiangedu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://sp.asd995.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ve.chemitech.net.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ma.lnxyls.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ue.yuexingan06.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vf.hnjuh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ob.szsharing.cn

[K04] 读取 JSON 文件
来源：http://lb.huixinmuqiang.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ix.lnxyls.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://aa.hnjuh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nb.huanxung.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nw.huixinmuqiang.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xn.panjiajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mw.haigaiapp.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rj.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ft.szxytkj.cn

[K05] 深拷贝对象
来源：http://lk.yuntaijiaju.cn

Py:   copy.deepcopy(obj)
来源：http://eh.yuexingan06.cn

PHP:  unserialize(serialize($obj));
来源：http://oc.panjiajie.cn

JS:   structuredClone(obj)
来源：http://xh.yuntaijiaju.cn

TS:   structuredClone(obj)
来源：http://mq.bookmarksfly.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://aa.asd995.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mo.szxytkj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jn.muxihuayi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cu.yuexingan06.cn

[K06] 解析 URL 查询串
来源：http://wo.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://az.huixiangedu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ib.colortex.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qj.colortex.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sz.nszjky.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://oh.wgjwhj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dw.wgjwhj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pc.hahajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://av.shxzukj.cn

[K07] 进制转换
来源：http://px.bjjhwx.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://aa.muxihuayi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pb.szxytkj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rs.jctech888.com.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pp.bjjhwx.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zd.hnjuh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://id.nszjky.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jp.shxzukj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yn.chemitech.net.cn

[K08] 二进制序列化（非 JSON）
来源：http://fb.jctech888.com.cn

Py:   pickle.dumps(obj)
来源：http://tq.bjjhwx.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sh.shxzskj.cn

JS:   v8.serialize(obj)        // Node
来源：http://ix.huixinmuqiang.cn

TS:   v8.serialize(obj)        // Node
来源：http://fj.huixiangedu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kv.shxzukj.cn

Go:   encoding/gob
来源：http://zu.panjiajie.cn

Ruby: Marshal.dump(obj)
来源：http://lw.chemitech.net.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ee.chemitech.net.cn

================================================================================
来源：http://ia.shxzskj.cn

L. 网络请求
来源：http://bf.haigaiapp.cn

================================================================================
来源：http://ax.szxytkj.cn

[L01] 发送 GET 请求
来源：http://er.huanxung.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kg.jianghongdianzi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.colortex.cn

JS:   await fetch(url)
来源：http://qo.chemitech.net.cn

TS:   await fetch(url)
来源：http://zz.chemitech.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ow.colortex.cn

Go:   resp, err := http.Get(url)
来源：http://on.yuexingan06.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jt.nszjky.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uf.shtwfgs.cn

[L02] 发送 POST JSON
来源：http://cy.bookmarksfly.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wl.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://or.colortex.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://od.huixiangedu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mo.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hh.muxihuayi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hr.hahajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lj.jianghongdianzi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://oi.hahajie.cn

[L03] 设置自定义请求头
来源：http://wj.bjjhwx.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://if.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xf.yuexingan06.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sr.lnxyls.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xt.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rg.shxzukj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://oi.bookmarksfly.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ga.hahajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kl.bjjhwx.cn

[L04] 设置超时
来源：http://mq.9csxet.cn

Py:   requests.get(url, timeout=5)
来源：http://hl.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uz.huixinmuqiang.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oz.hnjuh.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fv.nicolike.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://so.muxihuayi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uy.jianghongdianzi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wu.521024.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://re.yuntaijiaju.cn

[L05] 上传文件（multipart）
来源：http://pt.bjjhwx.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dj.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ns.shxzskj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ys.szsharing.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ka.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vi.panjiajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xr.yuntaijiaju.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cl.shtwfgs.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pl.muxihuayi.cn

[L06] 解析响应为 JSON
来源：http://oc.newstarts.cn

Py:   resp.json()
来源：http://mr.shxzukj.cn

PHP:  json_decode($body, true);
来源：http://kx.nicolike.cn

JS:   await resp.json()
来源：http://pr.muxihuayi.cn

TS:   await resp.json()
来源：http://nb.nicolike.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://co.huanxung.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ci.bjjhwx.cn

Ruby: JSON.parse(resp.body)
来源：http://rb.gzmigu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dd.colortex.cn

[L07] 处理 HTTP 状态码
来源：http://lm.9csxet.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ex.jctech888.com.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hv.hahajie.cn

JS:   resp.ok;  resp.status
来源：http://dl.newstarts.cn

TS:   resp.ok;  resp.status
来源：http://sg.nicolike.cn

Java: resp.statusCode()
来源：http://xt.huixiangedu.cn

Go:   resp.StatusCode
来源：http://xy.lnxyls.cn

Ruby: resp.code.to_i
来源：http://zq.jctech888.com.cn

C#:   (int)resp.StatusCode
来源：http://wy.panjiajie.cn

[L08] 并发请求多个地址
来源：http://ic.panjiajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dc.jctech888.com.cn

PHP:  curl_multi_init() 系列
来源：http://nx.hnjuh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lf.huixiangedu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ml.szsharing.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vb.shxzukj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://du.chemitech.net.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zi.newstarts.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sd.nicolike.cn

================================================================================
来源：http://tj.asd995.cn

M. 命令行 / 进程 / 环境
来源：http://rn.asd995.cn

================================================================================
来源：http://yk.huixinmuqiang.cn

[M01] 读取命令行参数
来源：http://xm.panjiajie.cn

Py:   sys.argv[1:]
来源：http://cs.huixiangedu.cn

PHP:  $argv;  $argc;
来源：http://ba.nszjky.cn

JS:   process.argv.slice(2)
来源：http://ua.lnxyls.cn

TS:   process.argv.slice(2)
来源：http://ss.lnxyls.cn

Java: args 数组（main 方法参数）
来源：http://yc.asd995.cn

Go:   os.Args[1:]
来源：http://kb.bookmarksfly.cn

Ruby: ARGV
来源：http://oc.bookmarksfly.cn

C#:   args 数组（Main 方法参数）
来源：http://iy.chemitech.net.cn

[M02] 读取环境变量
来源：http://bh.bookmarksfly.cn

Py:   os.environ.get("HOME")
来源：http://kj.shxzukj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://oi.jctech888.com.cn

JS:   process.env.HOME
来源：http://em.hahajie.cn

TS:   process.env.HOME
来源：http://ui.colortex.cn

Java: System.getenv("HOME")
来源：http://ex.asd995.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xn.newstarts.cn

Ruby: ENV["HOME"]
来源：http://db.asd995.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pv.asd995.cn

[M03] 执行外部命令
来源：http://ps.9csxet.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://al.newstarts.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://aq.bjjhwx.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://tk.asd995.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rs.shxzukj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xc.huanxung.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qv.bookmarksfly.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gr.bjjhwx.cn

C#:   Process.Start("ls", "-l");
来源：http://wb.haigaiapp.cn

[M04] 获取当前工作目录
来源：http://jp.huixiangedu.cn

Py:   os.getcwd()
来源：http://sp.shxzskj.cn

PHP:  getcwd();
来源：http://ft.bookmarksfly.cn

JS:   process.cwd()
来源：http://da.wgjwhj.cn

TS:   process.cwd()
来源：http://rp.shtwfgs.cn

Java: Path.of("").toAbsolutePath()
来源：http://ye.nicolike.cn

Go:   os.Getwd()
来源：http://ra.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://lo.yuexingan06.cn

C#:   Directory.GetCurrentDirectory()
来源：http://uq.nicolike.cn

[M05] 设置退出码
来源：http://gj.huanxung.cn

Py:   sys.exit(1)
来源：http://kg.wgjwhj.cn

PHP:  exit(1);
来源：http://gl.bjjhwx.cn

JS:   process.exit(1)
来源：http://ag.nszjky.cn

TS:   process.exit(1)
来源：http://rq.shxzukj.cn

Java: System.exit(1)
来源：http://ao.jctech888.com.cn

Go:   os.Exit(1)
来源：http://yc.nszjky.cn

Ruby: exit 1
来源：http://rz.lnxyls.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cb.nszjky.cn

[M06] 向标准错误输出
来源：http://yu.szxytkj.cn

Py:   print("err", file=sys.stderr)
来源：http://uy.asd995.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ie.gzmigu.cn

JS:   console.error("err")
来源：http://ut.hnjuh.cn

TS:   console.error("err")
来源：http://xi.lnxyls.cn

Java: System.err.println("err")
来源：http://ul.shxzskj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://am.asd995.cn

Ruby: warn "err"
来源：http://dm.yuexingan06.cn

C#:   Console.Error.WriteLine("err")
来源：http://hc.huixiangedu.cn

[M07] 判断是否为主入口
来源：http://te.shxzskj.cn

Py:   if __name__ == "__main__":
来源：http://qu.jianghongdianzi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hj.yuntaijiaju.cn

JS:   require.main === module
来源：http://pb.yuexingan06.cn

TS:   require.main === module
来源：http://jz.jctech888.com.cn

Java: public static void main(String[] args)
来源：http://yq.muxihuayi.cn

Go:   func main()
来源：http://wr.nicolike.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bh.gzmigu.cn

C#:   static void Main(string[] args)
来源：http://wq.szxytkj.cn

[M08] 获取系统与运行时信息
来源：http://ey.chemitech.net.cn

Py:   platform.system();  platform.python_version()
来源：http://uc.huixinmuqiang.cn

PHP:  PHP_OS;  phpversion();
来源：http://ub.huixiangedu.cn

JS:   process.platform;  process.version
来源：http://vc.shxzskj.cn

TS:   process.platform;  process.version
来源：http://qv.muxihuayi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zi.huixinmuqiang.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://nx.jctech888.com.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pr.bookmarksfly.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://iy.colortex.cn

================================================================================
来源：http://qa.panjiajie.cn

N. 数据结构与算法
来源：http://sh.yuexingan06.cn

================================================================================
来源：http://cq.nicolike.cn

[N01] 二分查找（有序数组）
来源：http://yp.hnjuh.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gv.muxihuayi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ey.shxzukj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ke.yuexingan06.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hh.gzmigu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://bk.haigaiapp.cn

Go:   sort.SearchInts(arr, x)
来源：http://rf.chemitech.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://gm.shxzskj.cn


<!-- 参考信息 -->