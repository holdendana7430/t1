代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rz.huixinmuqiang.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ja.yuexingan06.cn

[J05] 时间加减（加 7 天）
来源：http://ye.huanxung.cn

Py:   now + timedelta(days=7)
来源：http://cx.jctech888.com.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ce.huixinmuqiang.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gy.huixinmuqiang.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zs.huixiangedu.cn

Java: LocalDate.now().plusDays(7)
来源：http://ji.chemitech.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://em.panjiajie.cn

Ruby: Time.now + 7 * 86400
来源：http://wl.huanxung.cn

C#:   DateTime.Now.AddDays(7)
来源：http://px.jctech888.com.cn

[J06] 计算两时间之差
来源：http://zl.hnjuh.cn

Py:   (end - start).total_seconds()
来源：http://ja.lnxyls.cn

PHP:  $end->diff($start)->days;
来源：http://lm.shxzukj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qz.9csxet.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rg.szxytkj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bi.shtwfgs.cn

Go:   end.Sub(start).Hours()
来源：http://qw.haigaiapp.cn

Ruby: end - start                 # 返回秒数
来源：http://bu.gzmigu.cn

C#:   (end - start).TotalSeconds
来源：http://lt.nszjky.cn

[J07] 比较两个日期
来源：http://li.haigaiapp.cn

Py:   d1 < d2;  d1 == d2
来源：http://jr.521024.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rl.szsharing.cn

JS:   d1.getTime() < d2.getTime()
来源：http://iz.hahajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qx.yuntaijiaju.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ip.newstarts.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cp.nicolike.cn

Ruby: d1 < d2;  d1 == d2
来源：http://sz.asd995.cn

C#:   d1 < d2;  d1 == d2
来源：http://ig.huixinmuqiang.cn

[J08] 提取年月日与星期
来源：http://of.521024.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lx.asd995.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zo.colortex.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ss.chemitech.net.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://eo.huanxung.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fm.jianghongdianzi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wr.shtwfgs.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cw.chemitech.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uc.szsharing.cn

[J09] 时区处理
来源：http://np.wgjwhj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cm.nszjky.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ed.jctech888.com.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wq.yuntaijiaju.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hj.newstarts.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://px.panjiajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fc.szxytkj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vj.hnjuh.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ue.shxzukj.cn

[J10] 取今天 / 本月第一天
来源：http://it.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://iz.bjjhwx.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zh.521024.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ki.bookmarksfly.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vf.yuntaijiaju.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ls.bjjhwx.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://de.asd995.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ic.newstarts.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fy.9csxet.cn

================================================================================
来源：http://gv.hahajie.cn

K. JSON 与序列化
来源：http://ot.hahajie.cn

================================================================================
来源：http://ev.panjiajie.cn

[K01] 对象转 JSON 字符串
来源：http://no.yuexingan06.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jt.szsharing.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://as.shxzskj.cn

JS:   JSON.stringify(obj)
来源：http://tw.asd995.cn

TS:   JSON.stringify(obj)
来源：http://hh.chemitech.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ki.jianghongdianzi.cn

Go:   json.Marshal(obj)
来源：http://kf.colortex.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vb.colortex.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://iv.bjjhwx.cn

[K02] JSON 字符串转对象
来源：http://rw.asd995.cn

Py:   json.loads(s)
来源：http://du.hnjuh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://io.yuexingan06.cn

JS:   JSON.parse(s)
来源：http://tn.shxzskj.cn

TS:   JSON.parse(s)
来源：http://hn.jctech888.com.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vn.szxytkj.cn

Go:   json.Unmarshal(data, &v)
来源：http://kq.haigaiapp.cn

Ruby: JSON.parse(s)
来源：http://lh.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fq.hnjuh.cn

[K03] JSON 美化输出（带缩进）
来源：http://fz.yuntaijiaju.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ce.chemitech.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nd.wgjwhj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://mi.huixiangedu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bz.nicolike.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hp.nszjky.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xk.9csxet.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qx.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jp.hnjuh.cn

[K04] 读取 JSON 文件
来源：http://ma.shxzukj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ml.bookmarksfly.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ui.hahajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jd.nszjky.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jn.bookmarksfly.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://oi.newstarts.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://iu.haigaiapp.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://pv.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://il.yuexingan06.cn

[K05] 深拷贝对象
来源：http://gx.wgjwhj.cn

Py:   copy.deepcopy(obj)
来源：http://da.jctech888.com.cn

PHP:  unserialize(serialize($obj));
来源：http://ot.panjiajie.cn

JS:   structuredClone(obj)
来源：http://ay.szsharing.cn

TS:   structuredClone(obj)
来源：http://wj.huixiangedu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://cw.shxzukj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ve.bookmarksfly.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ox.9csxet.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zy.nicolike.cn

[K06] 解析 URL 查询串
来源：http://aw.bjjhwx.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lp.yuntaijiaju.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nx.shtwfgs.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jg.asd995.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ro.wgjwhj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uy.gzmigu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fx.muxihuayi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ay.bookmarksfly.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ni.jctech888.com.cn

[K07] 进制转换
来源：http://hq.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kg.yuntaijiaju.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nl.521024.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xq.muxihuayi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://iz.hnjuh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lb.szsharing.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vn.jianghongdianzi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zu.newstarts.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yo.jctech888.com.cn

[K08] 二进制序列化（非 JSON）
来源：http://cw.nicolike.cn

Py:   pickle.dumps(obj)
来源：http://xc.szsharing.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ka.hnjuh.cn

JS:   v8.serialize(obj)        // Node
来源：http://ea.wgjwhj.cn

TS:   v8.serialize(obj)        // Node
来源：http://gs.9csxet.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bf.huixiangedu.cn

Go:   encoding/gob
来源：http://ox.9csxet.cn

Ruby: Marshal.dump(obj)
来源：http://wf.bjjhwx.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nk.huixinmuqiang.cn

================================================================================
来源：http://xd.asd995.cn

L. 网络请求
来源：http://ut.yuntaijiaju.cn

================================================================================
来源：http://nf.bjjhwx.cn

[L01] 发送 GET 请求
来源：http://lr.colortex.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ws.yuntaijiaju.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ka.chemitech.net.cn

JS:   await fetch(url)
来源：http://yu.bookmarksfly.cn

TS:   await fetch(url)
来源：http://ix.nszjky.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pb.nszjky.cn

Go:   resp, err := http.Get(url)
来源：http://nz.szsharing.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qd.haigaiapp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ch.nszjky.cn

[L02] 发送 POST JSON
来源：http://ux.yuntaijiaju.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ex.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yo.szsharing.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://co.bjjhwx.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ym.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ab.lnxyls.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lk.yuntaijiaju.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mi.muxihuayi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zs.huixinmuqiang.cn

[L03] 设置自定义请求头
来源：http://ix.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://td.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cd.shtwfgs.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xo.hahajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pw.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dy.yuexingan06.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ou.nicolike.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uk.haigaiapp.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zl.jianghongdianzi.cn

[L04] 设置超时
来源：http://ly.huanxung.cn

Py:   requests.get(url, timeout=5)
来源：http://sd.521024.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wb.szsharing.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pa.szxytkj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tr.muxihuayi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hf.hahajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://av.yuntaijiaju.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yb.huixinmuqiang.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gi.szsharing.cn

[L05] 上传文件（multipart）
来源：http://ns.chemitech.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ru.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nr.lnxyls.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ve.szxytkj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gp.yuexingan06.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gw.panjiajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qa.muxihuayi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ca.shxzskj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hn.huixiangedu.cn

[L06] 解析响应为 JSON
来源：http://vv.nicolike.cn

Py:   resp.json()
来源：http://he.huanxung.cn

PHP:  json_decode($body, true);
来源：http://ob.shxzukj.cn

JS:   await resp.json()
来源：http://ti.nszjky.cn

TS:   await resp.json()
来源：http://hi.nicolike.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ft.chemitech.net.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dt.nszjky.cn

Ruby: JSON.parse(resp.body)
来源：http://uj.nszjky.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ev.yuntaijiaju.cn

[L07] 处理 HTTP 状态码
来源：http://va.gzmigu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wf.shxzskj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vc.jianghongdianzi.cn

JS:   resp.ok;  resp.status
来源：http://yu.huanxung.cn

TS:   resp.ok;  resp.status
来源：http://kc.huanxung.cn

Java: resp.statusCode()
来源：http://cj.szxytkj.cn

Go:   resp.StatusCode
来源：http://dv.colortex.cn

Ruby: resp.code.to_i
来源：http://hs.yuexingan06.cn

C#:   (int)resp.StatusCode
来源：http://ap.shtwfgs.cn

[L08] 并发请求多个地址
来源：http://qb.muxihuayi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fx.newstarts.cn

PHP:  curl_multi_init() 系列
来源：http://fj.panjiajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yq.shxzukj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vd.nicolike.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ab.wgjwhj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sr.hahajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wa.9csxet.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rr.bjjhwx.cn

================================================================================
来源：http://xg.szxytkj.cn

M. 命令行 / 进程 / 环境
来源：http://nn.shxzukj.cn

================================================================================
来源：http://cz.szsharing.cn

[M01] 读取命令行参数
来源：http://uy.yuntaijiaju.cn

Py:   sys.argv[1:]
来源：http://yi.bookmarksfly.cn

PHP:  $argv;  $argc;
来源：http://qz.szxytkj.cn

JS:   process.argv.slice(2)
来源：http://lr.newstarts.cn

TS:   process.argv.slice(2)
来源：http://rl.bjjhwx.cn

Java: args 数组（main 方法参数）
来源：http://mn.colortex.cn

Go:   os.Args[1:]
来源：http://xa.9csxet.cn

Ruby: ARGV
来源：http://an.jctech888.com.cn

C#:   args 数组（Main 方法参数）
来源：http://hf.panjiajie.cn

[M02] 读取环境变量
来源：http://jb.gzmigu.cn

Py:   os.environ.get("HOME")
来源：http://ir.hahajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ip.nicolike.cn

JS:   process.env.HOME
来源：http://sk.lnxyls.cn

TS:   process.env.HOME
来源：http://fj.hnjuh.cn

Java: System.getenv("HOME")
来源：http://sm.lnxyls.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dw.szsharing.cn

Ruby: ENV["HOME"]
来源：http://xm.colortex.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kd.huanxung.cn

[M03] 执行外部命令
来源：http://bo.szxytkj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uk.yuexingan06.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ib.szxytkj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pf.yuexingan06.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ni.shxzukj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zk.jianghongdianzi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hk.wgjwhj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://uo.gzmigu.cn

C#:   Process.Start("ls", "-l");
来源：http://zf.nicolike.cn

[M04] 获取当前工作目录
来源：http://dq.szxytkj.cn

Py:   os.getcwd()
来源：http://jm.shxzukj.cn

PHP:  getcwd();
来源：http://oh.wgjwhj.cn

JS:   process.cwd()
来源：http://ep.hnjuh.cn

TS:   process.cwd()
来源：http://yo.huanxung.cn

Java: Path.of("").toAbsolutePath()
来源：http://km.panjiajie.cn

Go:   os.Getwd()
来源：http://kp.newstarts.cn

Ruby: Dir.pwd
来源：http://io.yuexingan06.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zn.panjiajie.cn

[M05] 设置退出码
来源：http://vu.9csxet.cn

Py:   sys.exit(1)
来源：http://uf.chemitech.net.cn

PHP:  exit(1);
来源：http://pq.bjjhwx.cn

JS:   process.exit(1)
来源：http://lo.huanxung.cn

TS:   process.exit(1)
来源：http://fw.bookmarksfly.cn

Java: System.exit(1)
来源：http://wv.lnxyls.cn

Go:   os.Exit(1)
来源：http://ex.huanxung.cn

Ruby: exit 1
来源：http://ol.huanxung.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lu.jianghongdianzi.cn

[M06] 向标准错误输出
来源：http://ws.szsharing.cn

Py:   print("err", file=sys.stderr)
来源：http://jj.nicolike.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://so.9csxet.cn

JS:   console.error("err")
来源：http://hs.hnjuh.cn

TS:   console.error("err")
来源：http://rr.colortex.cn

Java: System.err.println("err")
来源：http://bd.yuntaijiaju.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kt.yuexingan06.cn

Ruby: warn "err"
来源：http://fk.9csxet.cn

C#:   Console.Error.WriteLine("err")
来源：http://cv.shxzskj.cn

[M07] 判断是否为主入口
来源：http://mq.shxzskj.cn

Py:   if __name__ == "__main__":
来源：http://ep.hnjuh.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ud.huixiangedu.cn

JS:   require.main === module
来源：http://dx.chemitech.net.cn

TS:   require.main === module
来源：http://xq.wgjwhj.cn

Java: public static void main(String[] args)
来源：http://sl.9csxet.cn

Go:   func main()
来源：http://qf.huixinmuqiang.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mp.newstarts.cn

C#:   static void Main(string[] args)
来源：http://da.jctech888.com.cn

[M08] 获取系统与运行时信息
来源：http://qh.huixiangedu.cn

Py:   platform.system();  platform.python_version()
来源：http://vu.newstarts.cn

PHP:  PHP_OS;  phpversion();
来源：http://le.huanxung.cn

JS:   process.platform;  process.version
来源：http://cf.colortex.cn

TS:   process.platform;  process.version
来源：http://cc.shtwfgs.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qo.chemitech.net.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://kp.huixinmuqiang.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lo.yuexingan06.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://co.colortex.cn

================================================================================
来源：http://ms.shxzukj.cn

N. 数据结构与算法
来源：http://cy.hahajie.cn

================================================================================
来源：http://vy.shxzskj.cn

[N01] 二分查找（有序数组）
来源：http://eg.szxytkj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gy.jctech888.com.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zc.szxytkj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mb.nicolike.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://av.huixiangedu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://kq.colortex.cn

Go:   sort.SearchInts(arr, x)
来源：http://pu.yuexingan06.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://nm.panjiajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ht.gzmigu.cn

[N02] 排序（工程实践用内置实现）
来源：http://bs.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://zo.hnjuh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ys.haigaiapp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ml.colortex.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gp.bjjhwx.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mm.jctech888.com.cn

Go:   slices.Sort(arr)
来源：http://ml.szxytkj.cn


<!-- 参考信息 -->