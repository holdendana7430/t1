代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sv.szxytkj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ec.hnjuh.cn

[J05] 时间加减（加 7 天）
来源：http://gs.newstarts.cn

Py:   now + timedelta(days=7)
来源：http://xg.newstarts.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qj.huixinmuqiang.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xk.newstarts.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://iq.shxzskj.cn

Java: LocalDate.now().plusDays(7)
来源：http://cr.colortex.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ez.yuntaijiaju.cn

Ruby: Time.now + 7 * 86400
来源：http://nw.hnjuh.cn

C#:   DateTime.Now.AddDays(7)
来源：http://cm.9csxet.cn

[J06] 计算两时间之差
来源：http://lm.panjiajie.cn

Py:   (end - start).total_seconds()
来源：http://yp.chemitech.net.cn

PHP:  $end->diff($start)->days;
来源：http://ok.hahajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mt.shtwfgs.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ox.shxzukj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ql.muxihuayi.cn

Go:   end.Sub(start).Hours()
来源：http://mo.jctech888.com.cn

Ruby: end - start                 # 返回秒数
来源：http://eq.szsharing.cn

C#:   (end - start).TotalSeconds
来源：http://et.yuntaijiaju.cn

[J07] 比较两个日期
来源：http://tz.huixinmuqiang.cn

Py:   d1 < d2;  d1 == d2
来源：http://bq.szxytkj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nf.nszjky.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kp.gzmigu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://am.hnjuh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ga.jianghongdianzi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mc.huanxung.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vi.hahajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://ci.gzmigu.cn

[J08] 提取年月日与星期
来源：http://me.nicolike.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://re.bjjhwx.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ia.haigaiapp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sr.colortex.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mi.nszjky.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ut.haigaiapp.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qd.nszjky.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ti.shxzskj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dt.bookmarksfly.cn

[J09] 时区处理
来源：http://kt.wgjwhj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ms.muxihuayi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gd.chemitech.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sk.lnxyls.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ax.hnjuh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ur.huanxung.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ye.nszjky.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fs.shxzskj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ug.haigaiapp.cn

[J10] 取今天 / 本月第一天
来源：http://nq.shxzskj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kq.haigaiapp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bk.hahajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rs.shxzskj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hr.shtwfgs.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://de.shtwfgs.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jt.colortex.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qd.yuntaijiaju.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vv.haigaiapp.cn

================================================================================
来源：http://wu.nicolike.cn

K. JSON 与序列化
来源：http://cs.szsharing.cn

================================================================================
来源：http://lz.jctech888.com.cn

[K01] 对象转 JSON 字符串
来源：http://pw.shxzukj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fs.asd995.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wd.huixinmuqiang.cn

JS:   JSON.stringify(obj)
来源：http://eh.nicolike.cn

TS:   JSON.stringify(obj)
来源：http://yu.bjjhwx.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jn.shtwfgs.cn

Go:   json.Marshal(obj)
来源：http://ff.asd995.cn

Ruby: obj.to_json                                     // require "json"
来源：http://lk.9csxet.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pw.lnxyls.cn

[K02] JSON 字符串转对象
来源：http://qp.szxytkj.cn

Py:   json.loads(s)
来源：http://ni.yuntaijiaju.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jz.chemitech.net.cn

JS:   JSON.parse(s)
来源：http://py.yuntaijiaju.cn

TS:   JSON.parse(s)
来源：http://wx.hahajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zv.lnxyls.cn

Go:   json.Unmarshal(data, &v)
来源：http://lb.jctech888.com.cn

Ruby: JSON.parse(s)
来源：http://bw.521024.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wl.shxzskj.cn

[K03] JSON 美化输出（带缩进）
来源：http://ou.9csxet.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uy.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tb.shtwfgs.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xf.wgjwhj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ya.huanxung.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kz.colortex.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jg.hnjuh.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dr.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cf.wgjwhj.cn

[K04] 读取 JSON 文件
来源：http://ya.gzmigu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://es.shxzukj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fr.521024.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bt.shxzukj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eq.asd995.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gv.newstarts.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lm.jianghongdianzi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://av.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cd.hahajie.cn

[K05] 深拷贝对象
来源：http://wk.newstarts.cn

Py:   copy.deepcopy(obj)
来源：http://ns.hahajie.cn

PHP:  unserialize(serialize($obj));
来源：http://ux.521024.cn

JS:   structuredClone(obj)
来源：http://vu.szxytkj.cn

TS:   structuredClone(obj)
来源：http://df.szxytkj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://it.lnxyls.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ez.jctech888.com.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jf.jctech888.com.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dk.hnjuh.cn

[K06] 解析 URL 查询串
来源：http://yc.asd995.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ek.haigaiapp.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gx.szsharing.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://de.gzmigu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iz.9csxet.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rf.muxihuayi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ai.bookmarksfly.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zo.hahajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bz.yuntaijiaju.cn

[K07] 进制转换
来源：http://ns.9csxet.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qu.szsharing.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ik.haigaiapp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lq.szsharing.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ak.521024.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xy.nicolike.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gx.bjjhwx.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qp.huixiangedu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ve.bookmarksfly.cn

[K08] 二进制序列化（非 JSON）
来源：http://gl.szsharing.cn

Py:   pickle.dumps(obj)
来源：http://lu.hnjuh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://al.hnjuh.cn

JS:   v8.serialize(obj)        // Node
来源：http://kr.chemitech.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://eb.jctech888.com.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://im.nszjky.cn

Go:   encoding/gob
来源：http://ra.jctech888.com.cn

Ruby: Marshal.dump(obj)
来源：http://wu.jianghongdianzi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://di.521024.cn

================================================================================
来源：http://up.szxytkj.cn

L. 网络请求
来源：http://lv.lnxyls.cn

================================================================================
来源：http://dz.newstarts.cn

[L01] 发送 GET 请求
来源：http://ru.huixiangedu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vl.shxzskj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vn.colortex.cn

JS:   await fetch(url)
来源：http://hz.nszjky.cn

TS:   await fetch(url)
来源：http://ih.9csxet.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ed.521024.cn

Go:   resp, err := http.Get(url)
来源：http://cd.huixiangedu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jk.jianghongdianzi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jf.521024.cn

[L02] 发送 POST JSON
来源：http://ft.huixinmuqiang.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rc.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://by.bjjhwx.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bg.jctech888.com.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kg.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jg.shxzskj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zd.gzmigu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uq.yuexingan06.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nz.lnxyls.cn

[L03] 设置自定义请求头
来源：http://lz.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dl.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zy.szsharing.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zb.bjjhwx.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tc.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ii.szxytkj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jz.9csxet.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://iu.muxihuayi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ws.panjiajie.cn

[L04] 设置超时
来源：http://kj.muxihuayi.cn

Py:   requests.get(url, timeout=5)
来源：http://bx.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bw.chemitech.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ee.yuexingan06.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sf.haigaiapp.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uz.bookmarksfly.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gu.wgjwhj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lf.newstarts.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://om.yuntaijiaju.cn

[L05] 上传文件（multipart）
来源：http://uz.yuntaijiaju.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pe.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ri.muxihuayi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gy.lnxyls.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gx.hahajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://om.panjiajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tx.hahajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kd.lnxyls.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qn.gzmigu.cn

[L06] 解析响应为 JSON
来源：http://wj.huanxung.cn

Py:   resp.json()
来源：http://yy.bookmarksfly.cn

PHP:  json_decode($body, true);
来源：http://il.yuexingan06.cn

JS:   await resp.json()
来源：http://sg.muxihuayi.cn

TS:   await resp.json()
来源：http://ce.jctech888.com.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jt.wgjwhj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kj.nicolike.cn

Ruby: JSON.parse(resp.body)
来源：http://rb.hahajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://li.asd995.cn

[L07] 处理 HTTP 状态码
来源：http://ov.gzmigu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bf.newstarts.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fq.gzmigu.cn

JS:   resp.ok;  resp.status
来源：http://to.szsharing.cn

TS:   resp.ok;  resp.status
来源：http://xn.hahajie.cn

Java: resp.statusCode()
来源：http://iu.nszjky.cn

Go:   resp.StatusCode
来源：http://wr.shxzukj.cn

Ruby: resp.code.to_i
来源：http://cv.jctech888.com.cn

C#:   (int)resp.StatusCode
来源：http://hi.newstarts.cn

[L08] 并发请求多个地址
来源：http://fb.newstarts.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rm.yuntaijiaju.cn

PHP:  curl_multi_init() 系列
来源：http://lf.shxzskj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://an.nszjky.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mw.colortex.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sv.hahajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xg.colortex.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ky.panjiajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://oe.yuntaijiaju.cn

================================================================================
来源：http://ng.shtwfgs.cn

M. 命令行 / 进程 / 环境
来源：http://eh.yuexingan06.cn

================================================================================
来源：http://ol.huixinmuqiang.cn

[M01] 读取命令行参数
来源：http://gl.jctech888.com.cn

Py:   sys.argv[1:]
来源：http://ex.bjjhwx.cn

PHP:  $argv;  $argc;
来源：http://ua.hahajie.cn

JS:   process.argv.slice(2)
来源：http://we.shtwfgs.cn

TS:   process.argv.slice(2)
来源：http://cw.szxytkj.cn

Java: args 数组（main 方法参数）
来源：http://hd.hnjuh.cn

Go:   os.Args[1:]
来源：http://dz.521024.cn

Ruby: ARGV
来源：http://dg.szxytkj.cn

C#:   args 数组（Main 方法参数）
来源：http://ta.521024.cn

[M02] 读取环境变量
来源：http://dn.wgjwhj.cn

Py:   os.environ.get("HOME")
来源：http://dk.yuntaijiaju.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://eu.huixinmuqiang.cn

JS:   process.env.HOME
来源：http://ds.szsharing.cn

TS:   process.env.HOME
来源：http://ac.9csxet.cn

Java: System.getenv("HOME")
来源：http://xu.9csxet.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vz.newstarts.cn

Ruby: ENV["HOME"]
来源：http://jh.szsharing.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://os.bjjhwx.cn

[M03] 执行外部命令
来源：http://os.huanxung.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://br.lnxyls.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ir.shtwfgs.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://he.wgjwhj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zc.hnjuh.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rv.colortex.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.shtwfgs.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ms.szxytkj.cn

C#:   Process.Start("ls", "-l");
来源：http://gu.gzmigu.cn

[M04] 获取当前工作目录
来源：http://wf.shxzskj.cn

Py:   os.getcwd()
来源：http://xc.muxihuayi.cn

PHP:  getcwd();
来源：http://jh.bookmarksfly.cn

JS:   process.cwd()
来源：http://om.haigaiapp.cn

TS:   process.cwd()
来源：http://ol.asd995.cn

Java: Path.of("").toAbsolutePath()
来源：http://lw.panjiajie.cn

Go:   os.Getwd()
来源：http://tx.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://es.huixiangedu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sn.nicolike.cn

[M05] 设置退出码
来源：http://lf.gzmigu.cn

Py:   sys.exit(1)
来源：http://xi.colortex.cn

PHP:  exit(1);
来源：http://eo.bjjhwx.cn

JS:   process.exit(1)
来源：http://zx.chemitech.net.cn

TS:   process.exit(1)
来源：http://sw.jctech888.com.cn

Java: System.exit(1)
来源：http://yt.yuntaijiaju.cn

Go:   os.Exit(1)
来源：http://gl.huixinmuqiang.cn

Ruby: exit 1
来源：http://rh.lnxyls.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qt.szsharing.cn

[M06] 向标准错误输出
来源：http://pf.nicolike.cn

Py:   print("err", file=sys.stderr)
来源：http://up.huixiangedu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wy.asd995.cn

JS:   console.error("err")
来源：http://ox.asd995.cn

TS:   console.error("err")
来源：http://xm.521024.cn

Java: System.err.println("err")
来源：http://hx.wgjwhj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://an.colortex.cn

Ruby: warn "err"
来源：http://tn.huanxung.cn

C#:   Console.Error.WriteLine("err")
来源：http://kd.jianghongdianzi.cn

[M07] 判断是否为主入口
来源：http://zr.521024.cn

Py:   if __name__ == "__main__":
来源：http://pc.shtwfgs.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ao.huixiangedu.cn

JS:   require.main === module
来源：http://fo.hnjuh.cn

TS:   require.main === module
来源：http://xw.yuexingan06.cn

Java: public static void main(String[] args)
来源：http://in.muxihuayi.cn

Go:   func main()
来源：http://kx.yuntaijiaju.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zx.asd995.cn

C#:   static void Main(string[] args)
来源：http://eh.szxytkj.cn

[M08] 获取系统与运行时信息
来源：http://in.shxzskj.cn

Py:   platform.system();  platform.python_version()
来源：http://sw.bookmarksfly.cn

PHP:  PHP_OS;  phpversion();
来源：http://xc.shtwfgs.cn

JS:   process.platform;  process.version
来源：http://vr.muxihuayi.cn

TS:   process.platform;  process.version
来源：http://in.lnxyls.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zt.huanxung.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fg.huixiangedu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hf.gzmigu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://la.shtwfgs.cn

================================================================================
来源：http://xd.shtwfgs.cn

N. 数据结构与算法
来源：http://wz.hahajie.cn

================================================================================
来源：http://bl.muxihuayi.cn

[N01] 二分查找（有序数组）
来源：http://vo.asd995.cn

Py:   bisect.bisect_left(arr, x)
来源：http://da.jctech888.com.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cf.521024.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fz.bookmarksfly.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://iv.colortex.cn

Java: Arrays.binarySearch(arr, x)
来源：http://um.bjjhwx.cn

Go:   sort.SearchInts(arr, x)
来源：http://ne.huixiangedu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vl.haigaiapp.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rc.yuntaijiaju.cn

[N02] 排序（工程实践用内置实现）
来源：http://jq.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://me.hnjuh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kf.haigaiapp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jm.nszjky.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bs.nszjky.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tg.jctech888.com.cn

Go:   slices.Sort(arr)
来源：http://ve.shxzskj.cn


<!-- 参考信息 -->