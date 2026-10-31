代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://my.nszjky.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cm.szxytkj.cn

[J05] 时间加减（加 7 天）
来源：http://bi.shxzukj.cn

Py:   now + timedelta(days=7)
来源：http://fa.shxzukj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qg.shxzskj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ts.bookmarksfly.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sg.szsharing.cn

Java: LocalDate.now().plusDays(7)
来源：http://ed.asd995.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bt.muxihuayi.cn

Ruby: Time.now + 7 * 86400
来源：http://kc.bookmarksfly.cn

C#:   DateTime.Now.AddDays(7)
来源：http://tn.huixinmuqiang.cn

[J06] 计算两时间之差
来源：http://tl.yuexingan06.cn

Py:   (end - start).total_seconds()
来源：http://bg.nicolike.cn

PHP:  $end->diff($start)->days;
来源：http://zl.asd995.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ca.9csxet.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ad.jctech888.com.cn

Java: Duration.between(start, end).toSeconds()
来源：http://se.521024.cn

Go:   end.Sub(start).Hours()
来源：http://ch.colortex.cn

Ruby: end - start                 # 返回秒数
来源：http://dw.haigaiapp.cn

C#:   (end - start).TotalSeconds
来源：http://ry.shxzskj.cn

[J07] 比较两个日期
来源：http://rx.shtwfgs.cn

Py:   d1 < d2;  d1 == d2
来源：http://tr.yuexingan06.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mu.nszjky.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lb.shxzukj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://tq.szxytkj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wl.huanxung.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://px.szxytkj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vz.nszjky.cn

C#:   d1 < d2;  d1 == d2
来源：http://bf.yuexingan06.cn

[J08] 提取年月日与星期
来源：http://ml.haigaiapp.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nx.bookmarksfly.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hg.hnjuh.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lu.asd995.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zm.jianghongdianzi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://eh.jctech888.com.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yr.nszjky.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sn.szsharing.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pa.panjiajie.cn

[J09] 时区处理
来源：http://jx.521024.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vb.hahajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qi.nszjky.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bb.yuntaijiaju.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hy.haigaiapp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xy.bookmarksfly.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vu.shtwfgs.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://oe.chemitech.net.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cd.shxzskj.cn

[J10] 取今天 / 本月第一天
来源：http://aj.521024.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jk.colortex.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xw.nicolike.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://co.newstarts.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://el.9csxet.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ih.huixiangedu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sl.colortex.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bo.wgjwhj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://iz.asd995.cn

================================================================================
来源：http://ze.wgjwhj.cn

K. JSON 与序列化
来源：http://pk.chemitech.net.cn

================================================================================
来源：http://mu.yuntaijiaju.cn

[K01] 对象转 JSON 字符串
来源：http://su.asd995.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bs.colortex.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yc.wgjwhj.cn

JS:   JSON.stringify(obj)
来源：http://nt.yuexingan06.cn

TS:   JSON.stringify(obj)
来源：http://uk.asd995.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nx.yuexingan06.cn

Go:   json.Marshal(obj)
来源：http://tr.szsharing.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dz.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ls.hahajie.cn

[K02] JSON 字符串转对象
来源：http://xu.9csxet.cn

Py:   json.loads(s)
来源：http://ny.yuntaijiaju.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zw.asd995.cn

JS:   JSON.parse(s)
来源：http://jl.huixiangedu.cn

TS:   JSON.parse(s)
来源：http://ra.huanxung.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sf.shtwfgs.cn

Go:   json.Unmarshal(data, &v)
来源：http://vr.bookmarksfly.cn

Ruby: JSON.parse(s)
来源：http://ha.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bc.huanxung.cn

[K03] JSON 美化输出（带缩进）
来源：http://gr.haigaiapp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bi.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bk.shxzskj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://yy.nszjky.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://di.jctech888.com.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://at.szxytkj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yv.yuntaijiaju.cn

Ruby: JSON.pretty_generate(obj)
来源：http://au.hahajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mn.newstarts.cn

[K04] 读取 JSON 文件
来源：http://cy.nicolike.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bo.haigaiapp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://al.nszjky.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hk.521024.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xa.yuntaijiaju.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rs.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uz.huixiangedu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ky.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ab.lnxyls.cn

[K05] 深拷贝对象
来源：http://ll.wgjwhj.cn

Py:   copy.deepcopy(obj)
来源：http://we.nicolike.cn

PHP:  unserialize(serialize($obj));
来源：http://cq.huanxung.cn

JS:   structuredClone(obj)
来源：http://ji.szxytkj.cn

TS:   structuredClone(obj)
来源：http://iy.newstarts.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kb.haigaiapp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ww.hahajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ji.panjiajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ic.yuntaijiaju.cn

[K06] 解析 URL 查询串
来源：http://lq.szxytkj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sv.szxytkj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sa.asd995.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vv.yuexingan06.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wf.521024.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.bookmarksfly.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hl.huixinmuqiang.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wi.chemitech.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ym.jctech888.com.cn

[K07] 进制转换
来源：http://ym.huixinmuqiang.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ga.wgjwhj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rc.521024.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qa.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://en.chemitech.net.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mb.haigaiapp.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://em.haigaiapp.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cm.shxzukj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sw.muxihuayi.cn

[K08] 二进制序列化（非 JSON）
来源：http://bb.szsharing.cn

Py:   pickle.dumps(obj)
来源：http://yt.shxzskj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hy.lnxyls.cn

JS:   v8.serialize(obj)        // Node
来源：http://ni.huanxung.cn

TS:   v8.serialize(obj)        // Node
来源：http://mq.jianghongdianzi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nm.huanxung.cn

Go:   encoding/gob
来源：http://vl.haigaiapp.cn

Ruby: Marshal.dump(obj)
来源：http://es.wgjwhj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yx.jianghongdianzi.cn

================================================================================
来源：http://dr.shxzukj.cn

L. 网络请求
来源：http://ao.haigaiapp.cn

================================================================================
来源：http://fe.szsharing.cn

[L01] 发送 GET 请求
来源：http://up.muxihuayi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ai.lnxyls.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ev.haigaiapp.cn

JS:   await fetch(url)
来源：http://jx.9csxet.cn

TS:   await fetch(url)
来源：http://pc.wgjwhj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sp.gzmigu.cn

Go:   resp, err := http.Get(url)
来源：http://hw.szsharing.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://tt.shxzskj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hv.nicolike.cn

[L02] 发送 POST JSON
来源：http://ch.yuexingan06.cn

Py:   requests.post(url, json={"a": 1})
来源：http://at.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kk.szxytkj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yk.bookmarksfly.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://um.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dt.hnjuh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ai.colortex.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ar.bookmarksfly.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qe.521024.cn

[L03] 设置自定义请求头
来源：http://zs.huixiangedu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gj.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bw.nszjky.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://us.szxytkj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nk.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xo.asd995.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ci.huixiangedu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://de.chemitech.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nw.asd995.cn

[L04] 设置超时
来源：http://ui.huixiangedu.cn

Py:   requests.get(url, timeout=5)
来源：http://bw.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://js.shtwfgs.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fr.yuntaijiaju.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ut.gzmigu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wn.newstarts.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://to.nszjky.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://oe.szsharing.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jj.yuntaijiaju.cn

[L05] 上传文件（multipart）
来源：http://yo.szsharing.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ip.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bg.huixinmuqiang.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hm.hahajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vv.huanxung.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pr.9csxet.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fl.9csxet.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rz.wgjwhj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xw.lnxyls.cn

[L06] 解析响应为 JSON
来源：http://uf.hnjuh.cn

Py:   resp.json()
来源：http://ts.newstarts.cn

PHP:  json_decode($body, true);
来源：http://ta.jianghongdianzi.cn

JS:   await resp.json()
来源：http://cr.9csxet.cn

TS:   await resp.json()
来源：http://nu.gzmigu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qa.nszjky.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://oh.muxihuayi.cn

Ruby: JSON.parse(resp.body)
来源：http://vu.colortex.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hq.nicolike.cn

[L07] 处理 HTTP 状态码
来源：http://it.nszjky.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jg.9csxet.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://do.bookmarksfly.cn

JS:   resp.ok;  resp.status
来源：http://wx.521024.cn

TS:   resp.ok;  resp.status
来源：http://iv.9csxet.cn

Java: resp.statusCode()
来源：http://xr.lnxyls.cn

Go:   resp.StatusCode
来源：http://to.muxihuayi.cn

Ruby: resp.code.to_i
来源：http://qb.muxihuayi.cn

C#:   (int)resp.StatusCode
来源：http://xe.chemitech.net.cn

[L08] 并发请求多个地址
来源：http://kt.gzmigu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sj.nicolike.cn

PHP:  curl_multi_init() 系列
来源：http://pt.huanxung.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nf.521024.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kh.jctech888.com.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tg.asd995.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bl.yuexingan06.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ke.lnxyls.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gn.newstarts.cn

================================================================================
来源：http://vz.shtwfgs.cn

M. 命令行 / 进程 / 环境
来源：http://om.gzmigu.cn

================================================================================
来源：http://nu.colortex.cn

[M01] 读取命令行参数
来源：http://cj.panjiajie.cn

Py:   sys.argv[1:]
来源：http://mo.shxzskj.cn

PHP:  $argv;  $argc;
来源：http://nc.bjjhwx.cn

JS:   process.argv.slice(2)
来源：http://oc.lnxyls.cn

TS:   process.argv.slice(2)
来源：http://nd.yuntaijiaju.cn

Java: args 数组（main 方法参数）
来源：http://dj.yuexingan06.cn

Go:   os.Args[1:]
来源：http://ml.shxzskj.cn

Ruby: ARGV
来源：http://dj.521024.cn

C#:   args 数组（Main 方法参数）
来源：http://hx.521024.cn

[M02] 读取环境变量
来源：http://op.asd995.cn

Py:   os.environ.get("HOME")
来源：http://bx.colortex.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ta.wgjwhj.cn

JS:   process.env.HOME
来源：http://xa.wgjwhj.cn

TS:   process.env.HOME
来源：http://jc.panjiajie.cn

Java: System.getenv("HOME")
来源：http://wm.huanxung.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kc.hnjuh.cn

Ruby: ENV["HOME"]
来源：http://hw.jctech888.com.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bg.colortex.cn

[M03] 执行外部命令
来源：http://wq.huixiangedu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://il.huanxung.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://sm.nszjky.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://oe.yuntaijiaju.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://un.asd995.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ti.shxzukj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://sm.wgjwhj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://np.panjiajie.cn

C#:   Process.Start("ls", "-l");
来源：http://we.colortex.cn

[M04] 获取当前工作目录
来源：http://vl.shxzukj.cn

Py:   os.getcwd()
来源：http://sl.521024.cn

PHP:  getcwd();
来源：http://ru.asd995.cn

JS:   process.cwd()
来源：http://nf.nszjky.cn

TS:   process.cwd()
来源：http://fn.colortex.cn

Java: Path.of("").toAbsolutePath()
来源：http://in.newstarts.cn

Go:   os.Getwd()
来源：http://lu.colortex.cn

Ruby: Dir.pwd
来源：http://up.nicolike.cn

C#:   Directory.GetCurrentDirectory()
来源：http://bd.chemitech.net.cn

[M05] 设置退出码
来源：http://fa.colortex.cn

Py:   sys.exit(1)
来源：http://mz.haigaiapp.cn

PHP:  exit(1);
来源：http://fd.muxihuayi.cn

JS:   process.exit(1)
来源：http://ch.huixinmuqiang.cn

TS:   process.exit(1)
来源：http://ii.huanxung.cn

Java: System.exit(1)
来源：http://po.bjjhwx.cn

Go:   os.Exit(1)
来源：http://sh.chemitech.net.cn

Ruby: exit 1
来源：http://na.huixiangedu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://em.haigaiapp.cn

[M06] 向标准错误输出
来源：http://tk.szxytkj.cn

Py:   print("err", file=sys.stderr)
来源：http://oj.lnxyls.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ah.newstarts.cn

JS:   console.error("err")
来源：http://xn.huanxung.cn

TS:   console.error("err")
来源：http://ox.hnjuh.cn

Java: System.err.println("err")
来源：http://mp.9csxet.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://px.hahajie.cn

Ruby: warn "err"
来源：http://bu.chemitech.net.cn

C#:   Console.Error.WriteLine("err")
来源：http://rj.bookmarksfly.cn

[M07] 判断是否为主入口
来源：http://sc.lnxyls.cn

Py:   if __name__ == "__main__":
来源：http://ch.huixiangedu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bm.wgjwhj.cn

JS:   require.main === module
来源：http://kf.huixinmuqiang.cn

TS:   require.main === module
来源：http://oh.nicolike.cn

Java: public static void main(String[] args)
来源：http://nx.chemitech.net.cn

Go:   func main()
来源：http://gp.wgjwhj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vn.bjjhwx.cn

C#:   static void Main(string[] args)
来源：http://rb.chemitech.net.cn

[M08] 获取系统与运行时信息
来源：http://vv.bjjhwx.cn

Py:   platform.system();  platform.python_version()
来源：http://dz.muxihuayi.cn

PHP:  PHP_OS;  phpversion();
来源：http://vy.shxzukj.cn

JS:   process.platform;  process.version
来源：http://lg.bookmarksfly.cn

TS:   process.platform;  process.version
来源：http://fd.szxytkj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cp.shxzukj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gi.wgjwhj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fj.huixiangedu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://uh.wgjwhj.cn

================================================================================
来源：http://gh.jctech888.com.cn

N. 数据结构与算法
来源：http://sm.asd995.cn

================================================================================
来源：http://ei.yuexingan06.cn

[N01] 二分查找（有序数组）
来源：http://wk.huixiangedu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://td.jctech888.com.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mw.colortex.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ms.huixinmuqiang.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xz.colortex.cn

Java: Arrays.binarySearch(arr, x)
来源：http://mb.shxzskj.cn

Go:   sort.SearchInts(arr, x)
来源：http://rz.huanxung.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qy.szsharing.cn

C#:   Array.BinarySearch(arr, x)
来源：http://aa.szxytkj.cn

[N02] 排序（工程实践用内置实现）
来源：http://zh.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://bl.bjjhwx.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://or.yuexingan06.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ql.huixiangedu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zd.huanxung.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gs.bjjhwx.cn

Go:   slices.Sort(arr)
来源：http://rq.huanxung.cn


<!-- 参考信息 -->