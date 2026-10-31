代发 wailian999

Py:   (end - start).total_seconds()
来源：http://sm.bookmarksfly.cn

PHP:  $end->diff($start)->days;
来源：http://se.huixiangedu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xd.panjiajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ag.huixinmuqiang.cn

Java: Duration.between(start, end).toSeconds()
来源：http://yo.huixiangedu.cn

Go:   end.Sub(start).Hours()
来源：http://ax.nszjky.cn

Ruby: end - start                 # 返回秒数
来源：http://gr.huixiangedu.cn

C#:   (end - start).TotalSeconds
来源：http://yk.9csxet.cn

[J07] 比较两个日期
来源：http://mm.szsharing.cn

Py:   d1 < d2;  d1 == d2
来源：http://bv.szsharing.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rg.gzmigu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://eu.nicolike.cn

TS:   d1.getTime() < d2.getTime()
来源：http://tx.muxihuayi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kd.shtwfgs.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wa.colortex.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xa.colortex.cn

C#:   d1 < d2;  d1 == d2
来源：http://tn.shxzskj.cn

[J08] 提取年月日与星期
来源：http://es.nicolike.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yy.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ln.shxzskj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ck.muxihuayi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://au.colortex.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vw.gzmigu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ui.bookmarksfly.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qf.nszjky.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://da.nszjky.cn

[J09] 时区处理
来源：http://od.huanxung.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ay.haigaiapp.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://la.huanxung.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pq.gzmigu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oc.9csxet.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://iq.shtwfgs.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zg.yuntaijiaju.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tc.shxzukj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ow.nicolike.cn

[J10] 取今天 / 本月第一天
来源：http://zn.colortex.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zj.muxihuayi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uk.shxzukj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://eo.521024.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hb.colortex.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ln.hnjuh.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dc.lnxyls.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://la.haigaiapp.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kz.muxihuayi.cn

================================================================================
来源：http://ak.newstarts.cn

K. JSON 与序列化
来源：http://fk.bjjhwx.cn

================================================================================
来源：http://ku.shtwfgs.cn

[K01] 对象转 JSON 字符串
来源：http://yx.yuexingan06.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uu.nicolike.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dy.jianghongdianzi.cn

JS:   JSON.stringify(obj)
来源：http://vt.nszjky.cn

TS:   JSON.stringify(obj)
来源：http://kz.huanxung.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zb.huixiangedu.cn

Go:   json.Marshal(obj)
来源：http://dy.asd995.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vn.nicolike.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://nu.521024.cn

[K02] JSON 字符串转对象
来源：http://oe.haigaiapp.cn

Py:   json.loads(s)
来源：http://rk.colortex.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://um.muxihuayi.cn

JS:   JSON.parse(s)
来源：http://cl.nszjky.cn

TS:   JSON.parse(s)
来源：http://hx.szxytkj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wi.huixiangedu.cn

Go:   json.Unmarshal(data, &v)
来源：http://zn.jianghongdianzi.cn

Ruby: JSON.parse(s)
来源：http://sq.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mn.chemitech.net.cn

[K03] JSON 美化输出（带缩进）
来源：http://dc.9csxet.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jv.szsharing.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nv.yuntaijiaju.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://me.yuntaijiaju.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vn.bookmarksfly.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fu.shxzskj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nd.asd995.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ja.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://no.szxytkj.cn

[K04] 读取 JSON 文件
来源：http://wj.shtwfgs.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ek.yuntaijiaju.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://py.521024.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://es.yuexingan06.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lg.szxytkj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zv.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zl.shtwfgs.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://nt.asd995.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://py.521024.cn

[K05] 深拷贝对象
来源：http://qc.9csxet.cn

Py:   copy.deepcopy(obj)
来源：http://mh.huixiangedu.cn

PHP:  unserialize(serialize($obj));
来源：http://di.asd995.cn

JS:   structuredClone(obj)
来源：http://ab.shxzukj.cn

TS:   structuredClone(obj)
来源：http://by.gzmigu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wa.wgjwhj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mw.haigaiapp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zx.nicolike.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xm.huixiangedu.cn

[K06] 解析 URL 查询串
来源：http://ga.huixiangedu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rs.huixiangedu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zi.muxihuayi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zg.haigaiapp.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qy.shxzukj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dh.szsharing.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fe.colortex.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vu.szxytkj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ey.asd995.cn

[K07] 进制转换
来源：http://zr.chemitech.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lg.yuntaijiaju.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zi.shxzskj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yw.szxytkj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vs.chemitech.net.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dm.huixiangedu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fo.haigaiapp.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gq.huixiangedu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yx.hnjuh.cn

[K08] 二进制序列化（非 JSON）
来源：http://wy.wgjwhj.cn

Py:   pickle.dumps(obj)
来源：http://rt.muxihuayi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xv.nszjky.cn

JS:   v8.serialize(obj)        // Node
来源：http://jr.huanxung.cn

TS:   v8.serialize(obj)        // Node
来源：http://er.nszjky.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dt.jianghongdianzi.cn

Go:   encoding/gob
来源：http://qv.bookmarksfly.cn

Ruby: Marshal.dump(obj)
来源：http://uw.shtwfgs.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dh.panjiajie.cn

================================================================================
来源：http://lk.shxzukj.cn

L. 网络请求
来源：http://jg.jctech888.com.cn

================================================================================
来源：http://vs.shxzukj.cn

[L01] 发送 GET 请求
来源：http://nb.huanxung.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jt.shxzskj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sr.bookmarksfly.cn

JS:   await fetch(url)
来源：http://uv.gzmigu.cn

TS:   await fetch(url)
来源：http://gr.shxzskj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qr.jctech888.com.cn

Go:   resp, err := http.Get(url)
来源：http://kk.hnjuh.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://cl.yuexingan06.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zb.asd995.cn

[L02] 发送 POST JSON
来源：http://nn.nszjky.cn

Py:   requests.post(url, json={"a": 1})
来源：http://yu.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ib.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wf.shtwfgs.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nu.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jz.haigaiapp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cd.huanxung.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xb.lnxyls.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gs.colortex.cn

[L03] 设置自定义请求头
来源：http://lv.yuntaijiaju.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jw.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://di.jianghongdianzi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qh.yuntaijiaju.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dj.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://if.newstarts.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uw.wgjwhj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hl.panjiajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yo.yuexingan06.cn

[L04] 设置超时
来源：http://yo.lnxyls.cn

Py:   requests.get(url, timeout=5)
来源：http://ck.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ka.huixinmuqiang.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mw.panjiajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cm.lnxyls.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ic.chemitech.net.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://er.yuntaijiaju.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pn.yuntaijiaju.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mm.panjiajie.cn

[L05] 上传文件（multipart）
来源：http://lj.shxzskj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hu.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bt.yuntaijiaju.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://no.hahajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://oy.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://iz.yuntaijiaju.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cm.huixinmuqiang.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jc.nicolike.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hl.bookmarksfly.cn

[L06] 解析响应为 JSON
来源：http://zm.hnjuh.cn

Py:   resp.json()
来源：http://dp.huixinmuqiang.cn

PHP:  json_decode($body, true);
来源：http://of.jctech888.com.cn

JS:   await resp.json()
来源：http://gg.haigaiapp.cn

TS:   await resp.json()
来源：http://kw.jctech888.com.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ve.gzmigu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ni.lnxyls.cn

Ruby: JSON.parse(resp.body)
来源：http://if.yuntaijiaju.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lp.huixiangedu.cn

[L07] 处理 HTTP 状态码
来源：http://pf.newstarts.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mo.szsharing.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cd.gzmigu.cn

JS:   resp.ok;  resp.status
来源：http://wz.colortex.cn

TS:   resp.ok;  resp.status
来源：http://ki.hahajie.cn

Java: resp.statusCode()
来源：http://vh.shxzukj.cn

Go:   resp.StatusCode
来源：http://zr.shtwfgs.cn

Ruby: resp.code.to_i
来源：http://ty.bjjhwx.cn

C#:   (int)resp.StatusCode
来源：http://gk.muxihuayi.cn

[L08] 并发请求多个地址
来源：http://nn.nszjky.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://iz.szxytkj.cn

PHP:  curl_multi_init() 系列
来源：http://du.szxytkj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zs.hahajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rf.panjiajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vm.huanxung.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mv.gzmigu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://iq.521024.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kt.chemitech.net.cn

================================================================================
来源：http://cm.gzmigu.cn

M. 命令行 / 进程 / 环境
来源：http://cv.colortex.cn

================================================================================
来源：http://qp.huixinmuqiang.cn

[M01] 读取命令行参数
来源：http://ze.panjiajie.cn

Py:   sys.argv[1:]
来源：http://hv.hnjuh.cn

PHP:  $argv;  $argc;
来源：http://pl.yuexingan06.cn

JS:   process.argv.slice(2)
来源：http://oe.asd995.cn

TS:   process.argv.slice(2)
来源：http://fi.nszjky.cn

Java: args 数组（main 方法参数）
来源：http://oj.hahajie.cn

Go:   os.Args[1:]
来源：http://nr.shtwfgs.cn

Ruby: ARGV
来源：http://eo.asd995.cn

C#:   args 数组（Main 方法参数）
来源：http://un.jianghongdianzi.cn

[M02] 读取环境变量
来源：http://qs.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://sp.chemitech.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zg.9csxet.cn

JS:   process.env.HOME
来源：http://rp.wgjwhj.cn

TS:   process.env.HOME
来源：http://sx.bookmarksfly.cn

Java: System.getenv("HOME")
来源：http://gw.shxzskj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jc.shxzskj.cn

Ruby: ENV["HOME"]
来源：http://ao.huanxung.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ic.jianghongdianzi.cn

[M03] 执行外部命令
来源：http://ko.jianghongdianzi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bo.chemitech.net.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ql.chemitech.net.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xp.newstarts.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ef.yuexingan06.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ek.huixinmuqiang.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mt.lnxyls.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bx.newstarts.cn

C#:   Process.Start("ls", "-l");
来源：http://oa.9csxet.cn

[M04] 获取当前工作目录
来源：http://wp.gzmigu.cn

Py:   os.getcwd()
来源：http://fa.panjiajie.cn

PHP:  getcwd();
来源：http://yj.huanxung.cn

JS:   process.cwd()
来源：http://lu.jctech888.com.cn

TS:   process.cwd()
来源：http://at.nicolike.cn

Java: Path.of("").toAbsolutePath()
来源：http://iq.colortex.cn

Go:   os.Getwd()
来源：http://in.yuntaijiaju.cn

Ruby: Dir.pwd
来源：http://ko.nicolike.cn

C#:   Directory.GetCurrentDirectory()
来源：http://td.muxihuayi.cn

[M05] 设置退出码
来源：http://va.yuntaijiaju.cn

Py:   sys.exit(1)
来源：http://yd.shtwfgs.cn

PHP:  exit(1);
来源：http://my.lnxyls.cn

JS:   process.exit(1)
来源：http://sr.nicolike.cn

TS:   process.exit(1)
来源：http://bj.lnxyls.cn

Java: System.exit(1)
来源：http://ah.shxzukj.cn

Go:   os.Exit(1)
来源：http://ub.panjiajie.cn

Ruby: exit 1
来源：http://uk.521024.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wf.bookmarksfly.cn

[M06] 向标准错误输出
来源：http://cd.szxytkj.cn

Py:   print("err", file=sys.stderr)
来源：http://yl.huixinmuqiang.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ts.szxytkj.cn

JS:   console.error("err")
来源：http://hf.huanxung.cn

TS:   console.error("err")
来源：http://yp.jctech888.com.cn

Java: System.err.println("err")
来源：http://xs.huixiangedu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wu.huanxung.cn

Ruby: warn "err"
来源：http://ta.shtwfgs.cn

C#:   Console.Error.WriteLine("err")
来源：http://rh.szxytkj.cn

[M07] 判断是否为主入口
来源：http://qg.newstarts.cn

Py:   if __name__ == "__main__":
来源：http://yc.shxzukj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vw.newstarts.cn

JS:   require.main === module
来源：http://zi.hnjuh.cn

TS:   require.main === module
来源：http://le.wgjwhj.cn

Java: public static void main(String[] args)
来源：http://kj.bjjhwx.cn

Go:   func main()
来源：http://vq.nicolike.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ns.bjjhwx.cn

C#:   static void Main(string[] args)
来源：http://rz.yuntaijiaju.cn

[M08] 获取系统与运行时信息
来源：http://tk.shtwfgs.cn

Py:   platform.system();  platform.python_version()
来源：http://sj.bookmarksfly.cn

PHP:  PHP_OS;  phpversion();
来源：http://gd.haigaiapp.cn

JS:   process.platform;  process.version
来源：http://gj.yuexingan06.cn

TS:   process.platform;  process.version
来源：http://cb.521024.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pk.bookmarksfly.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://nk.colortex.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ks.nicolike.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bc.shtwfgs.cn

================================================================================
来源：http://ev.colortex.cn

N. 数据结构与算法
来源：http://gr.chemitech.net.cn

================================================================================
来源：http://oa.lnxyls.cn

[N01] 二分查找（有序数组）
来源：http://nw.nszjky.cn

Py:   bisect.bisect_left(arr, x)
来源：http://jv.huixiangedu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ho.chemitech.net.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zy.haigaiapp.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wk.huixiangedu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://lp.shtwfgs.cn

Go:   sort.SearchInts(arr, x)
来源：http://of.521024.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vw.huixiangedu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://mj.jctech888.com.cn

[N02] 排序（工程实践用内置实现）
来源：http://uz.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://le.colortex.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wb.nszjky.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://yf.wgjwhj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ms.bjjhwx.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sf.nicolike.cn

Go:   slices.Sort(arr)
来源：http://qp.chemitech.net.cn

Ruby: arr.sort
来源：http://is.bookmarksfly.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://iu.chemitech.net.cn

[N03] 快速排序（分治示例）
来源：http://ar.colortex.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bg.yuexingan06.cn

PHP:  // 递归实现，或用 usort
来源：http://xi.521024.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kl.huixinmuqiang.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kt.huixinmuqiang.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wr.wgjwhj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ao.lnxyls.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://eu.jianghongdianzi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cq.nicolike.cn

[N04] 斐波那契数列
来源：http://ah.szsharing.cn


<!-- 参考信息 -->