代发 wailian999

TS:   new Date("2024-01-02")
来源：http://au.huanxung.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mj.yuntaijiaju.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://td.szsharing.cn

Ruby: Date.parse("2024-01-02")
来源：http://ne.huixinmuqiang.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wp.jianghongdianzi.cn

[J04] 时间戳与日期互转
来源：http://gy.hahajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rp.muxihuayi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gr.hnjuh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://by.panjiajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.shxzukj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vr.9csxet.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://za.colortex.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dh.huixinmuqiang.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qb.colortex.cn

[J05] 时间加减（加 7 天）
来源：http://sv.shxzskj.cn

Py:   now + timedelta(days=7)
来源：http://wg.newstarts.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vv.szxytkj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mh.szsharing.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pz.nicolike.cn

Java: LocalDate.now().plusDays(7)
来源：http://sh.wgjwhj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qe.nicolike.cn

Ruby: Time.now + 7 * 86400
来源：http://mo.huixiangedu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ne.panjiajie.cn

[J06] 计算两时间之差
来源：http://sw.hahajie.cn

Py:   (end - start).total_seconds()
来源：http://tb.colortex.cn

PHP:  $end->diff($start)->days;
来源：http://sr.shtwfgs.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ay.colortex.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cy.hnjuh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bo.szsharing.cn

Go:   end.Sub(start).Hours()
来源：http://xc.hnjuh.cn

Ruby: end - start                 # 返回秒数
来源：http://zk.lnxyls.cn

C#:   (end - start).TotalSeconds
来源：http://dc.huixinmuqiang.cn

[J07] 比较两个日期
来源：http://yw.nicolike.cn

Py:   d1 < d2;  d1 == d2
来源：http://tx.shxzskj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lc.hnjuh.cn

JS:   d1.getTime() < d2.getTime()
来源：http://dr.gzmigu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mv.asd995.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qg.yuexingan06.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ze.bookmarksfly.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bg.asd995.cn

C#:   d1 < d2;  d1 == d2
来源：http://mq.yuntaijiaju.cn

[J08] 提取年月日与星期
来源：http://ce.panjiajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fo.lnxyls.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hd.szsharing.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gh.nicolike.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ap.huixinmuqiang.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sn.hahajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tx.panjiajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zb.jianghongdianzi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://re.szsharing.cn

[J09] 时区处理
来源：http://uq.shtwfgs.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cr.shxzukj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yu.gzmigu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ku.hnjuh.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zs.bookmarksfly.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yc.haigaiapp.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ye.shxzskj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wd.yuntaijiaju.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fu.jctech888.com.cn

[J10] 取今天 / 本月第一天
来源：http://pr.hnjuh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://lw.huanxung.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ie.jctech888.com.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ql.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ck.asd995.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yj.lnxyls.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ha.szsharing.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zr.newstarts.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mo.huixinmuqiang.cn

================================================================================
来源：http://zd.521024.cn

K. JSON 与序列化
来源：http://bi.haigaiapp.cn

================================================================================
来源：http://do.hahajie.cn

[K01] 对象转 JSON 字符串
来源：http://wn.haigaiapp.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lv.shxzukj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ct.muxihuayi.cn

JS:   JSON.stringify(obj)
来源：http://tn.gzmigu.cn

TS:   JSON.stringify(obj)
来源：http://cu.huixiangedu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://si.jianghongdianzi.cn

Go:   json.Marshal(obj)
来源：http://wf.chemitech.net.cn

Ruby: obj.to_json                                     // require "json"
来源：http://yq.huanxung.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://sv.gzmigu.cn

[K02] JSON 字符串转对象
来源：http://tw.muxihuayi.cn

Py:   json.loads(s)
来源：http://sc.huixinmuqiang.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vd.shxzukj.cn

JS:   JSON.parse(s)
来源：http://cn.bjjhwx.cn

TS:   JSON.parse(s)
来源：http://ek.nszjky.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://to.newstarts.cn

Go:   json.Unmarshal(data, &v)
来源：http://dl.muxihuayi.cn

Ruby: JSON.parse(s)
来源：http://hi.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fn.muxihuayi.cn

[K03] JSON 美化输出（带缩进）
来源：http://pr.chemitech.net.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nx.gzmigu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tj.colortex.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qc.yuntaijiaju.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://jr.huixinmuqiang.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kt.shtwfgs.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://py.haigaiapp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hz.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yj.chemitech.net.cn

[K04] 读取 JSON 文件
来源：http://kv.shtwfgs.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://di.szxytkj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fh.nszjky.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oz.huixiangedu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cm.shtwfgs.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://eh.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ae.hahajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zl.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ns.yuexingan06.cn

[K05] 深拷贝对象
来源：http://wy.bookmarksfly.cn

Py:   copy.deepcopy(obj)
来源：http://tx.bookmarksfly.cn

PHP:  unserialize(serialize($obj));
来源：http://ht.nszjky.cn

JS:   structuredClone(obj)
来源：http://yt.gzmigu.cn

TS:   structuredClone(obj)
来源：http://ut.shxzukj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://pn.szsharing.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ee.jctech888.com.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zt.wgjwhj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lh.huanxung.cn

[K06] 解析 URL 查询串
来源：http://ae.szxytkj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fx.shxzskj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ns.hnjuh.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ja.nszjky.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gi.huixinmuqiang.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fy.wgjwhj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ks.huanxung.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xn.haigaiapp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ko.asd995.cn

[K07] 进制转换
来源：http://ks.szxytkj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jn.yuntaijiaju.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qs.huixiangedu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nc.wgjwhj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tk.hnjuh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lb.huanxung.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kv.521024.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ty.haigaiapp.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://af.yuntaijiaju.cn

[K08] 二进制序列化（非 JSON）
来源：http://ij.jctech888.com.cn

Py:   pickle.dumps(obj)
来源：http://oz.chemitech.net.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hq.shxzukj.cn

JS:   v8.serialize(obj)        // Node
来源：http://ls.bookmarksfly.cn

TS:   v8.serialize(obj)        // Node
来源：http://hj.huixinmuqiang.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://oy.lnxyls.cn

Go:   encoding/gob
来源：http://cd.shtwfgs.cn

Ruby: Marshal.dump(obj)
来源：http://is.hahajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lc.yuntaijiaju.cn

================================================================================
来源：http://ft.jianghongdianzi.cn

L. 网络请求
来源：http://io.shxzukj.cn

================================================================================
来源：http://qw.9csxet.cn

[L01] 发送 GET 请求
来源：http://bx.yuexingan06.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://th.szxytkj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://td.hahajie.cn

JS:   await fetch(url)
来源：http://ur.wgjwhj.cn

TS:   await fetch(url)
来源：http://ty.wgjwhj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rz.hnjuh.cn

Go:   resp, err := http.Get(url)
来源：http://mp.jctech888.com.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://yx.wgjwhj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sd.gzmigu.cn

[L02] 发送 POST JSON
来源：http://oc.newstarts.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xr.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pu.9csxet.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qh.szxytkj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ow.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xb.hahajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zw.shxzskj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hi.haigaiapp.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fo.shxzskj.cn

[L03] 设置自定义请求头
来源：http://gh.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zw.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://iw.shxzukj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ym.newstarts.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yl.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wo.huanxung.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qy.yuexingan06.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wc.huanxung.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pc.shxzukj.cn

[L04] 设置超时
来源：http://lg.bookmarksfly.cn

Py:   requests.get(url, timeout=5)
来源：http://kl.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pk.chemitech.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pp.yuexingan06.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ca.nszjky.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://da.yuexingan06.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qr.shxzukj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yh.jianghongdianzi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vc.nicolike.cn

[L05] 上传文件（multipart）
来源：http://fn.lnxyls.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://he.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lu.521024.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qr.chemitech.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kj.lnxyls.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fl.lnxyls.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bw.9csxet.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yi.szxytkj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jq.chemitech.net.cn

[L06] 解析响应为 JSON
来源：http://fy.szsharing.cn

Py:   resp.json()
来源：http://zl.9csxet.cn

PHP:  json_decode($body, true);
来源：http://gl.huixinmuqiang.cn

JS:   await resp.json()
来源：http://mx.szxytkj.cn

TS:   await resp.json()
来源：http://am.521024.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zy.hahajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ef.asd995.cn

Ruby: JSON.parse(resp.body)
来源：http://xo.asd995.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mv.chemitech.net.cn

[L07] 处理 HTTP 状态码
来源：http://sd.shtwfgs.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ck.jctech888.com.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rg.asd995.cn

JS:   resp.ok;  resp.status
来源：http://dd.bookmarksfly.cn

TS:   resp.ok;  resp.status
来源：http://bu.jctech888.com.cn

Java: resp.statusCode()
来源：http://wj.hnjuh.cn

Go:   resp.StatusCode
来源：http://sj.asd995.cn

Ruby: resp.code.to_i
来源：http://tt.9csxet.cn

C#:   (int)resp.StatusCode
来源：http://cy.muxihuayi.cn

[L08] 并发请求多个地址
来源：http://qb.huanxung.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wy.newstarts.cn

PHP:  curl_multi_init() 系列
来源：http://cu.asd995.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pp.wgjwhj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xv.yuntaijiaju.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rg.szsharing.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wq.huanxung.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ip.huanxung.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qf.yuexingan06.cn

================================================================================
来源：http://qm.521024.cn

M. 命令行 / 进程 / 环境
来源：http://rv.shtwfgs.cn

================================================================================
来源：http://ba.521024.cn

[M01] 读取命令行参数
来源：http://ed.bjjhwx.cn

Py:   sys.argv[1:]
来源：http://rw.szsharing.cn

PHP:  $argv;  $argc;
来源：http://yu.chemitech.net.cn

JS:   process.argv.slice(2)
来源：http://ln.521024.cn

TS:   process.argv.slice(2)
来源：http://dk.panjiajie.cn

Java: args 数组（main 方法参数）
来源：http://lx.hnjuh.cn

Go:   os.Args[1:]
来源：http://fq.muxihuayi.cn

Ruby: ARGV
来源：http://ni.haigaiapp.cn

C#:   args 数组（Main 方法参数）
来源：http://fz.nszjky.cn

[M02] 读取环境变量
来源：http://pv.jctech888.com.cn

Py:   os.environ.get("HOME")
来源：http://ay.jianghongdianzi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lx.colortex.cn

JS:   process.env.HOME
来源：http://eu.yuexingan06.cn

TS:   process.env.HOME
来源：http://ql.shxzskj.cn

Java: System.getenv("HOME")
来源：http://ij.yuntaijiaju.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tc.521024.cn

Ruby: ENV["HOME"]
来源：http://zk.wgjwhj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tm.9csxet.cn

[M03] 执行外部命令
来源：http://xk.huixiangedu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://er.bookmarksfly.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ps.colortex.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://iv.haigaiapp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ke.szsharing.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fj.colortex.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://aj.panjiajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zv.wgjwhj.cn

C#:   Process.Start("ls", "-l");
来源：http://ux.bookmarksfly.cn

[M04] 获取当前工作目录
来源：http://vc.shxzskj.cn

Py:   os.getcwd()
来源：http://lq.yuntaijiaju.cn

PHP:  getcwd();
来源：http://if.jianghongdianzi.cn

JS:   process.cwd()
来源：http://as.gzmigu.cn

TS:   process.cwd()
来源：http://wl.bjjhwx.cn

Java: Path.of("").toAbsolutePath()
来源：http://gp.521024.cn

Go:   os.Getwd()
来源：http://kr.colortex.cn

Ruby: Dir.pwd
来源：http://qz.yuexingan06.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gg.szsharing.cn

[M05] 设置退出码
来源：http://ee.521024.cn

Py:   sys.exit(1)
来源：http://ep.gzmigu.cn

PHP:  exit(1);
来源：http://rs.hahajie.cn

JS:   process.exit(1)
来源：http://pw.nszjky.cn

TS:   process.exit(1)
来源：http://is.yuntaijiaju.cn

Java: System.exit(1)
来源：http://yu.jctech888.com.cn

Go:   os.Exit(1)
来源：http://gg.nicolike.cn

Ruby: exit 1
来源：http://ww.nicolike.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fj.lnxyls.cn

[M06] 向标准错误输出
来源：http://pr.wgjwhj.cn

Py:   print("err", file=sys.stderr)
来源：http://kg.hnjuh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://br.wgjwhj.cn

JS:   console.error("err")
来源：http://ql.yuexingan06.cn

TS:   console.error("err")
来源：http://cm.shxzskj.cn

Java: System.err.println("err")
来源：http://bf.yuntaijiaju.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ha.9csxet.cn

Ruby: warn "err"
来源：http://eg.colortex.cn

C#:   Console.Error.WriteLine("err")
来源：http://fk.gzmigu.cn

[M07] 判断是否为主入口
来源：http://sx.bjjhwx.cn

Py:   if __name__ == "__main__":
来源：http://dr.muxihuayi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nq.wgjwhj.cn

JS:   require.main === module
来源：http://mx.bookmarksfly.cn

TS:   require.main === module
来源：http://jt.hnjuh.cn

Java: public static void main(String[] args)
来源：http://jc.hnjuh.cn

Go:   func main()
来源：http://fo.lnxyls.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wz.newstarts.cn

C#:   static void Main(string[] args)
来源：http://yc.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://ud.huixinmuqiang.cn

Py:   platform.system();  platform.python_version()
来源：http://jo.jctech888.com.cn

PHP:  PHP_OS;  phpversion();
来源：http://mk.lnxyls.cn

JS:   process.platform;  process.version
来源：http://yd.shxzukj.cn

TS:   process.platform;  process.version
来源：http://my.huixinmuqiang.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ca.shxzskj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://sc.szsharing.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dk.huixiangedu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://tv.jctech888.com.cn

================================================================================
来源：http://gu.newstarts.cn

N. 数据结构与算法
来源：http://lw.521024.cn

================================================================================
来源：http://lp.szxytkj.cn

[N01] 二分查找（有序数组）
来源：http://va.bjjhwx.cn

Py:   bisect.bisect_left(arr, x)
来源：http://um.huixinmuqiang.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ma.szxytkj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qx.jctech888.com.cn


<!-- 参考信息 -->