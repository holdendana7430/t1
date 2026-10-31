代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ud.muxihuayi.cn

[J04] 时间戳与日期互转
来源：http://oz.newstarts.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dz.haigaiapp.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ss.szxytkj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ze.bookmarksfly.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://rb.shtwfgs.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kb.hnjuh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bb.yuexingan06.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ac.521024.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nw.9csxet.cn

[J05] 时间加减（加 7 天）
来源：http://wj.jctech888.com.cn

Py:   now + timedelta(days=7)
来源：http://ch.wgjwhj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rz.huixinmuqiang.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ph.nszjky.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fn.yuexingan06.cn

Java: LocalDate.now().plusDays(7)
来源：http://of.szxytkj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nl.nicolike.cn

Ruby: Time.now + 7 * 86400
来源：http://hk.yuexingan06.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ty.muxihuayi.cn

[J06] 计算两时间之差
来源：http://hy.shxzskj.cn

Py:   (end - start).total_seconds()
来源：http://xv.jctech888.com.cn

PHP:  $end->diff($start)->days;
来源：http://bz.newstarts.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bk.huanxung.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dn.szxytkj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lj.shxzskj.cn

Go:   end.Sub(start).Hours()
来源：http://qh.shtwfgs.cn

Ruby: end - start                 # 返回秒数
来源：http://fe.lnxyls.cn

C#:   (end - start).TotalSeconds
来源：http://xn.yuexingan06.cn

[J07] 比较两个日期
来源：http://xa.bookmarksfly.cn

Py:   d1 < d2;  d1 == d2
来源：http://og.bjjhwx.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zo.shtwfgs.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ye.szsharing.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fv.panjiajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://oy.521024.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nx.asd995.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xt.jctech888.com.cn

C#:   d1 < d2;  d1 == d2
来源：http://ug.nszjky.cn

[J08] 提取年月日与星期
来源：http://gd.jianghongdianzi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://oi.colortex.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oe.nszjky.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ks.newstarts.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fq.521024.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qs.hnjuh.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kp.hahajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lm.yuntaijiaju.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fa.shtwfgs.cn

[J09] 时区处理
来源：http://vv.newstarts.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hv.521024.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tt.szxytkj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yx.huixiangedu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ea.lnxyls.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yb.lnxyls.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lo.shtwfgs.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fw.huixiangedu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pn.szxytkj.cn

[J10] 取今天 / 本月第一天
来源：http://fd.yuntaijiaju.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fu.jctech888.com.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lp.lnxyls.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qb.newstarts.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sv.bjjhwx.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bj.yuexingan06.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xr.lnxyls.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qm.szxytkj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://si.huanxung.cn

================================================================================
来源：http://bz.shtwfgs.cn

K. JSON 与序列化
来源：http://sd.colortex.cn

================================================================================
来源：http://ts.bjjhwx.cn

[K01] 对象转 JSON 字符串
来源：http://mb.hnjuh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tp.muxihuayi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://eg.panjiajie.cn

JS:   JSON.stringify(obj)
来源：http://xg.szsharing.cn

TS:   JSON.stringify(obj)
来源：http://mr.bjjhwx.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ni.wgjwhj.cn

Go:   json.Marshal(obj)
来源：http://sh.asd995.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wt.9csxet.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vu.colortex.cn

[K02] JSON 字符串转对象
来源：http://lv.nicolike.cn

Py:   json.loads(s)
来源：http://zt.szsharing.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uu.hahajie.cn

JS:   JSON.parse(s)
来源：http://dn.muxihuayi.cn

TS:   JSON.parse(s)
来源：http://sc.asd995.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zx.huanxung.cn

Go:   json.Unmarshal(data, &v)
来源：http://fm.nszjky.cn

Ruby: JSON.parse(s)
来源：http://la.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vb.gzmigu.cn

[K03] JSON 美化输出（带缩进）
来源：http://tl.huixiangedu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://og.huixiangedu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tk.jctech888.com.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vg.huixinmuqiang.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://pq.9csxet.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qh.newstarts.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ms.521024.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qb.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ii.shtwfgs.cn

[K04] 读取 JSON 文件
来源：http://co.asd995.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ro.shxzukj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uh.haigaiapp.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vy.shxzukj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eh.chemitech.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jn.newstarts.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://em.jianghongdianzi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gc.521024.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://of.lnxyls.cn

[K05] 深拷贝对象
来源：http://zf.chemitech.net.cn

Py:   copy.deepcopy(obj)
来源：http://nd.chemitech.net.cn

PHP:  unserialize(serialize($obj));
来源：http://us.shtwfgs.cn

JS:   structuredClone(obj)
来源：http://uq.hahajie.cn

TS:   structuredClone(obj)
来源：http://cz.hnjuh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qj.shxzukj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ax.asd995.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yc.asd995.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wd.asd995.cn

[K06] 解析 URL 查询串
来源：http://di.wgjwhj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tc.nicolike.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sc.bjjhwx.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cd.9csxet.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rp.jianghongdianzi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tt.521024.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sx.shxzskj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zg.lnxyls.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mx.szxytkj.cn

[K07] 进制转换
来源：http://wx.shxzskj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sh.9csxet.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tg.9csxet.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://md.yuntaijiaju.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tf.muxihuayi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cl.nszjky.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ti.jctech888.com.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fp.521024.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tc.yuntaijiaju.cn

[K08] 二进制序列化（非 JSON）
来源：http://io.szsharing.cn

Py:   pickle.dumps(obj)
来源：http://uz.hahajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ff.huanxung.cn

JS:   v8.serialize(obj)        // Node
来源：http://xk.lnxyls.cn

TS:   v8.serialize(obj)        // Node
来源：http://fr.huanxung.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ld.haigaiapp.cn

Go:   encoding/gob
来源：http://xm.huanxung.cn

Ruby: Marshal.dump(obj)
来源：http://xu.colortex.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dq.shtwfgs.cn

================================================================================
来源：http://qb.521024.cn

L. 网络请求
来源：http://oh.szxytkj.cn

================================================================================
来源：http://qr.muxihuayi.cn

[L01] 发送 GET 请求
来源：http://pt.9csxet.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xm.colortex.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ou.nicolike.cn

JS:   await fetch(url)
来源：http://so.nicolike.cn

TS:   await fetch(url)
来源：http://oj.szxytkj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kb.panjiajie.cn

Go:   resp, err := http.Get(url)
来源：http://nt.chemitech.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://du.9csxet.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nb.yuntaijiaju.cn

[L02] 发送 POST JSON
来源：http://vl.shxzukj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://sl.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rl.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qx.521024.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gm.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yl.muxihuayi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lk.gzmigu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sw.szsharing.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ym.jianghongdianzi.cn

[L03] 设置自定义请求头
来源：http://yq.bookmarksfly.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fd.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hk.shxzukj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tx.newstarts.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pb.521024.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://im.huixiangedu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zd.huanxung.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ku.chemitech.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ev.nszjky.cn

[L04] 设置超时
来源：http://yo.gzmigu.cn

Py:   requests.get(url, timeout=5)
来源：http://kq.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sx.asd995.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://up.nszjky.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dq.newstarts.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xs.9csxet.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sp.shxzukj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wy.panjiajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ec.wgjwhj.cn

[L05] 上传文件（multipart）
来源：http://vz.9csxet.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nq.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yx.muxihuayi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mi.chemitech.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fy.jianghongdianzi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mp.shxzukj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ih.huanxung.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kx.yuexingan06.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qg.521024.cn

[L06] 解析响应为 JSON
来源：http://gh.9csxet.cn

Py:   resp.json()
来源：http://nx.huixiangedu.cn

PHP:  json_decode($body, true);
来源：http://md.shtwfgs.cn

JS:   await resp.json()
来源：http://he.panjiajie.cn

TS:   await resp.json()
来源：http://fk.lnxyls.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ah.bjjhwx.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tj.bookmarksfly.cn

Ruby: JSON.parse(resp.body)
来源：http://du.asd995.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fp.muxihuayi.cn

[L07] 处理 HTTP 状态码
来源：http://lr.hnjuh.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xi.9csxet.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xk.nszjky.cn

JS:   resp.ok;  resp.status
来源：http://ng.bjjhwx.cn

TS:   resp.ok;  resp.status
来源：http://lm.muxihuayi.cn

Java: resp.statusCode()
来源：http://xe.szsharing.cn

Go:   resp.StatusCode
来源：http://rf.9csxet.cn

Ruby: resp.code.to_i
来源：http://ck.bjjhwx.cn

C#:   (int)resp.StatusCode
来源：http://rc.hahajie.cn

[L08] 并发请求多个地址
来源：http://bk.nicolike.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pm.wgjwhj.cn

PHP:  curl_multi_init() 系列
来源：http://lr.yuexingan06.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ej.9csxet.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xj.shtwfgs.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hf.asd995.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yb.szxytkj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rp.yuexingan06.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://el.szxytkj.cn

================================================================================
来源：http://bz.shxzukj.cn

M. 命令行 / 进程 / 环境
来源：http://jd.szsharing.cn

================================================================================
来源：http://hm.haigaiapp.cn

[M01] 读取命令行参数
来源：http://yo.jianghongdianzi.cn

Py:   sys.argv[1:]
来源：http://ga.bookmarksfly.cn

PHP:  $argv;  $argc;
来源：http://md.szsharing.cn

JS:   process.argv.slice(2)
来源：http://me.bookmarksfly.cn

TS:   process.argv.slice(2)
来源：http://xt.shxzukj.cn

Java: args 数组（main 方法参数）
来源：http://ud.hnjuh.cn

Go:   os.Args[1:]
来源：http://xl.521024.cn

Ruby: ARGV
来源：http://vh.nszjky.cn

C#:   args 数组（Main 方法参数）
来源：http://oh.jianghongdianzi.cn

[M02] 读取环境变量
来源：http://ex.jianghongdianzi.cn

Py:   os.environ.get("HOME")
来源：http://ve.yuexingan06.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zh.hahajie.cn

JS:   process.env.HOME
来源：http://fr.nicolike.cn

TS:   process.env.HOME
来源：http://xq.shxzskj.cn

Java: System.getenv("HOME")
来源：http://zy.huanxung.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zp.lnxyls.cn

Ruby: ENV["HOME"]
来源：http://cy.shtwfgs.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vn.panjiajie.cn

[M03] 执行外部命令
来源：http://sh.shxzukj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://it.huixinmuqiang.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gr.shtwfgs.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gp.nicolike.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xc.szxytkj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zy.jctech888.com.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://te.hahajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ep.huanxung.cn

C#:   Process.Start("ls", "-l");
来源：http://gq.yuexingan06.cn

[M04] 获取当前工作目录
来源：http://bm.hnjuh.cn

Py:   os.getcwd()
来源：http://fg.hahajie.cn

PHP:  getcwd();
来源：http://nl.huixiangedu.cn

JS:   process.cwd()
来源：http://of.bjjhwx.cn

TS:   process.cwd()
来源：http://ko.bookmarksfly.cn

Java: Path.of("").toAbsolutePath()
来源：http://ox.shxzukj.cn

Go:   os.Getwd()
来源：http://rp.chemitech.net.cn

Ruby: Dir.pwd
来源：http://vx.szsharing.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zx.9csxet.cn

[M05] 设置退出码
来源：http://dv.yuexingan06.cn

Py:   sys.exit(1)
来源：http://ke.shxzukj.cn

PHP:  exit(1);
来源：http://os.521024.cn

JS:   process.exit(1)
来源：http://jk.asd995.cn

TS:   process.exit(1)
来源：http://qt.hahajie.cn

Java: System.exit(1)
来源：http://ff.yuexingan06.cn

Go:   os.Exit(1)
来源：http://mc.panjiajie.cn

Ruby: exit 1
来源：http://go.shxzskj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wf.chemitech.net.cn

[M06] 向标准错误输出
来源：http://ik.yuexingan06.cn

Py:   print("err", file=sys.stderr)
来源：http://wo.yuntaijiaju.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://am.huixiangedu.cn

JS:   console.error("err")
来源：http://lf.nszjky.cn

TS:   console.error("err")
来源：http://ed.szxytkj.cn

Java: System.err.println("err")
来源：http://xc.9csxet.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yt.nszjky.cn

Ruby: warn "err"
来源：http://dj.asd995.cn

C#:   Console.Error.WriteLine("err")
来源：http://ke.gzmigu.cn

[M07] 判断是否为主入口
来源：http://se.yuexingan06.cn

Py:   if __name__ == "__main__":
来源：http://cd.newstarts.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wi.521024.cn

JS:   require.main === module
来源：http://bm.lnxyls.cn

TS:   require.main === module
来源：http://ku.bookmarksfly.cn

Java: public static void main(String[] args)
来源：http://wv.yuexingan06.cn

Go:   func main()
来源：http://it.shxzukj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fw.szxytkj.cn

C#:   static void Main(string[] args)
来源：http://zg.bjjhwx.cn

[M08] 获取系统与运行时信息
来源：http://tt.lnxyls.cn

Py:   platform.system();  platform.python_version()
来源：http://nz.chemitech.net.cn

PHP:  PHP_OS;  phpversion();
来源：http://jh.hahajie.cn

JS:   process.platform;  process.version
来源：http://kk.szsharing.cn

TS:   process.platform;  process.version
来源：http://yp.haigaiapp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cz.yuexingan06.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://sf.huixiangedu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vc.nszjky.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jf.9csxet.cn

================================================================================
来源：http://tz.newstarts.cn

N. 数据结构与算法
来源：http://nk.jctech888.com.cn

================================================================================
来源：http://fq.chemitech.net.cn

[N01] 二分查找（有序数组）
来源：http://px.chemitech.net.cn

Py:   bisect.bisect_left(arr, x)
来源：http://te.yuntaijiaju.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zm.haigaiapp.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tg.jctech888.com.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wy.gzmigu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://cv.shtwfgs.cn

Go:   sort.SearchInts(arr, x)
来源：http://yt.jianghongdianzi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qh.szxytkj.cn


<!-- 参考信息 -->