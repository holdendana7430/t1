代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rd.gzmigu.cn

Ruby: Time.now + 7 * 86400
来源：http://lb.shxzskj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pr.521024.cn

[J06] 计算两时间之差
来源：http://rj.shtwfgs.cn

Py:   (end - start).total_seconds()
来源：http://au.muxihuayi.cn

PHP:  $end->diff($start)->days;
来源：http://is.521024.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://od.shxzskj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gj.chemitech.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vf.shtwfgs.cn

Go:   end.Sub(start).Hours()
来源：http://ni.huixiangedu.cn

Ruby: end - start                 # 返回秒数
来源：http://sj.panjiajie.cn

C#:   (end - start).TotalSeconds
来源：http://ap.huixinmuqiang.cn

[J07] 比较两个日期
来源：http://ku.yuntaijiaju.cn

Py:   d1 < d2;  d1 == d2
来源：http://sf.shxzskj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fs.bookmarksfly.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jd.huixiangedu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ud.huixinmuqiang.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tm.hnjuh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ul.haigaiapp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://yv.jianghongdianzi.cn

C#:   d1 < d2;  d1 == d2
来源：http://ok.szsharing.cn

[J08] 提取年月日与星期
来源：http://sw.panjiajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yx.huixinmuqiang.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jr.haigaiapp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lx.hahajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wl.asd995.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fh.jianghongdianzi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jz.huanxung.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://as.szxytkj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cy.nszjky.cn

[J09] 时区处理
来源：http://fh.bookmarksfly.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lv.bookmarksfly.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hv.gzmigu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ou.hnjuh.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://th.newstarts.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xo.lnxyls.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kd.panjiajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://dg.9csxet.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ho.newstarts.cn

[J10] 取今天 / 本月第一天
来源：http://dc.jianghongdianzi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vh.shtwfgs.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bd.nicolike.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pm.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gh.hnjuh.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fr.asd995.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mu.newstarts.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ai.huanxung.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wv.521024.cn

================================================================================
来源：http://bx.nszjky.cn

K. JSON 与序列化
来源：http://zz.shxzukj.cn

================================================================================
来源：http://vt.huanxung.cn

[K01] 对象转 JSON 字符串
来源：http://rf.shxzskj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zq.hahajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://si.bookmarksfly.cn

JS:   JSON.stringify(obj)
来源：http://qj.asd995.cn

TS:   JSON.stringify(obj)
来源：http://ut.colortex.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kz.wgjwhj.cn

Go:   json.Marshal(obj)
来源：http://xe.521024.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mb.gzmigu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ug.huanxung.cn

[K02] JSON 字符串转对象
来源：http://in.yuexingan06.cn

Py:   json.loads(s)
来源：http://rt.colortex.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gh.colortex.cn

JS:   JSON.parse(s)
来源：http://hs.shxzukj.cn

TS:   JSON.parse(s)
来源：http://db.jianghongdianzi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ke.muxihuayi.cn

Go:   json.Unmarshal(data, &v)
来源：http://hd.asd995.cn

Ruby: JSON.parse(s)
来源：http://ox.colortex.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gj.colortex.cn

[K03] JSON 美化输出（带缩进）
来源：http://jg.panjiajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nz.haigaiapp.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rs.yuexingan06.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ti.nicolike.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tm.shxzskj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jb.huixiangedu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wv.shxzskj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gf.colortex.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jk.szxytkj.cn

[K04] 读取 JSON 文件
来源：http://da.muxihuayi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://eh.muxihuayi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dm.nszjky.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jr.colortex.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kp.bookmarksfly.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kf.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yg.shxzukj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qu.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cp.nicolike.cn

[K05] 深拷贝对象
来源：http://iv.hnjuh.cn

Py:   copy.deepcopy(obj)
来源：http://dp.shtwfgs.cn

PHP:  unserialize(serialize($obj));
来源：http://du.shxzskj.cn

JS:   structuredClone(obj)
来源：http://ie.muxihuayi.cn

TS:   structuredClone(obj)
来源：http://ex.chemitech.net.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ru.yuexingan06.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ov.panjiajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qm.asd995.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fa.nszjky.cn

[K06] 解析 URL 查询串
来源：http://fl.huixiangedu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mt.9csxet.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://do.521024.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xr.shxzskj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ee.huixiangedu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ug.huixiangedu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://lf.bjjhwx.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xk.9csxet.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bv.gzmigu.cn

[K07] 进制转换
来源：http://gs.szsharing.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jh.9csxet.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ua.wgjwhj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pt.nszjky.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pn.huixiangedu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://at.yuexingan06.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oc.jianghongdianzi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sk.huixinmuqiang.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://me.huixiangedu.cn

[K08] 二进制序列化（非 JSON）
来源：http://vx.shxzukj.cn

Py:   pickle.dumps(obj)
来源：http://zb.lnxyls.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://kz.nicolike.cn

JS:   v8.serialize(obj)        // Node
来源：http://wi.bookmarksfly.cn

TS:   v8.serialize(obj)        // Node
来源：http://fu.shxzskj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dx.panjiajie.cn

Go:   encoding/gob
来源：http://kr.jianghongdianzi.cn

Ruby: Marshal.dump(obj)
来源：http://lu.muxihuayi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fj.wgjwhj.cn

================================================================================
来源：http://qi.asd995.cn

L. 网络请求
来源：http://qa.nszjky.cn

================================================================================
来源：http://zt.hnjuh.cn

[L01] 发送 GET 请求
来源：http://if.huixinmuqiang.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dw.haigaiapp.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tr.yuntaijiaju.cn

JS:   await fetch(url)
来源：http://eh.nicolike.cn

TS:   await fetch(url)
来源：http://yf.muxihuayi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fo.asd995.cn

Go:   resp, err := http.Get(url)
来源：http://ep.nicolike.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://nt.shtwfgs.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://im.9csxet.cn

[L02] 发送 POST JSON
来源：http://in.szxytkj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://aa.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gh.jctech888.com.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hc.szxytkj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bz.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rr.colortex.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tl.lnxyls.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ew.panjiajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zp.huanxung.cn

[L03] 设置自定义请求头
来源：http://ys.jianghongdianzi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yg.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ct.colortex.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bv.jctech888.com.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ry.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jt.hahajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://da.bookmarksfly.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vz.shxzskj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hc.lnxyls.cn

[L04] 设置超时
来源：http://jk.nszjky.cn

Py:   requests.get(url, timeout=5)
来源：http://re.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ky.huanxung.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dz.bjjhwx.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://la.colortex.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bb.shtwfgs.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ay.521024.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vi.wgjwhj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xa.szsharing.cn

[L05] 上传文件（multipart）
来源：http://hh.muxihuayi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ku.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vt.gzmigu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://iu.nicolike.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ha.muxihuayi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ou.bookmarksfly.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sz.wgjwhj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xa.gzmigu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pb.nicolike.cn

[L06] 解析响应为 JSON
来源：http://cr.lnxyls.cn

Py:   resp.json()
来源：http://cf.shtwfgs.cn

PHP:  json_decode($body, true);
来源：http://mg.szxytkj.cn

JS:   await resp.json()
来源：http://gj.huixiangedu.cn

TS:   await resp.json()
来源：http://zk.lnxyls.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://el.huixiangedu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kt.9csxet.cn

Ruby: JSON.parse(resp.body)
来源：http://bz.nszjky.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rq.gzmigu.cn

[L07] 处理 HTTP 状态码
来源：http://tw.shxzukj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tl.yuntaijiaju.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wa.szsharing.cn

JS:   resp.ok;  resp.status
来源：http://fx.shxzskj.cn

TS:   resp.ok;  resp.status
来源：http://vh.hnjuh.cn

Java: resp.statusCode()
来源：http://lo.yuntaijiaju.cn

Go:   resp.StatusCode
来源：http://rg.hahajie.cn

Ruby: resp.code.to_i
来源：http://fx.9csxet.cn

C#:   (int)resp.StatusCode
来源：http://ik.asd995.cn

[L08] 并发请求多个地址
来源：http://eg.huanxung.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hb.bjjhwx.cn

PHP:  curl_multi_init() 系列
来源：http://ss.nicolike.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mu.wgjwhj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zh.colortex.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cv.lnxyls.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ol.panjiajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gi.colortex.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://es.wgjwhj.cn

================================================================================
来源：http://ad.9csxet.cn

M. 命令行 / 进程 / 环境
来源：http://nv.shxzukj.cn

================================================================================
来源：http://nw.nicolike.cn

[M01] 读取命令行参数
来源：http://ur.bookmarksfly.cn

Py:   sys.argv[1:]
来源：http://gs.lnxyls.cn

PHP:  $argv;  $argc;
来源：http://sg.jianghongdianzi.cn

JS:   process.argv.slice(2)
来源：http://wd.yuexingan06.cn

TS:   process.argv.slice(2)
来源：http://kd.nicolike.cn

Java: args 数组（main 方法参数）
来源：http://hx.shtwfgs.cn

Go:   os.Args[1:]
来源：http://vh.shxzskj.cn

Ruby: ARGV
来源：http://mo.asd995.cn

C#:   args 数组（Main 方法参数）
来源：http://vx.newstarts.cn

[M02] 读取环境变量
来源：http://iv.9csxet.cn

Py:   os.environ.get("HOME")
来源：http://kw.huixinmuqiang.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fs.yuexingan06.cn

JS:   process.env.HOME
来源：http://iq.colortex.cn

TS:   process.env.HOME
来源：http://nb.nszjky.cn

Java: System.getenv("HOME")
来源：http://pz.bjjhwx.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oh.lnxyls.cn

Ruby: ENV["HOME"]
来源：http://ma.jianghongdianzi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bg.shtwfgs.cn

[M03] 执行外部命令
来源：http://vs.shxzskj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nw.yuntaijiaju.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vb.huanxung.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qw.bjjhwx.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ic.szsharing.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ev.gzmigu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dg.nszjky.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zp.haigaiapp.cn

C#:   Process.Start("ls", "-l");
来源：http://ga.hahajie.cn

[M04] 获取当前工作目录
来源：http://oi.wgjwhj.cn

Py:   os.getcwd()
来源：http://oe.shtwfgs.cn

PHP:  getcwd();
来源：http://ex.panjiajie.cn

JS:   process.cwd()
来源：http://zb.hahajie.cn

TS:   process.cwd()
来源：http://ip.szsharing.cn

Java: Path.of("").toAbsolutePath()
来源：http://fb.shxzskj.cn

Go:   os.Getwd()
来源：http://uq.gzmigu.cn

Ruby: Dir.pwd
来源：http://hm.shxzskj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://bu.colortex.cn

[M05] 设置退出码
来源：http://qz.521024.cn

Py:   sys.exit(1)
来源：http://lv.nicolike.cn

PHP:  exit(1);
来源：http://rf.jctech888.com.cn

JS:   process.exit(1)
来源：http://pf.asd995.cn

TS:   process.exit(1)
来源：http://kw.shxzskj.cn

Java: System.exit(1)
来源：http://pb.521024.cn

Go:   os.Exit(1)
来源：http://ir.9csxet.cn

Ruby: exit 1
来源：http://iz.panjiajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ik.newstarts.cn

[M06] 向标准错误输出
来源：http://sl.bookmarksfly.cn

Py:   print("err", file=sys.stderr)
来源：http://ut.newstarts.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gu.haigaiapp.cn

JS:   console.error("err")
来源：http://cc.hnjuh.cn

TS:   console.error("err")
来源：http://sb.panjiajie.cn

Java: System.err.println("err")
来源：http://mq.bookmarksfly.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tu.hnjuh.cn

Ruby: warn "err"
来源：http://wp.hnjuh.cn

C#:   Console.Error.WriteLine("err")
来源：http://sz.colortex.cn

[M07] 判断是否为主入口
来源：http://co.newstarts.cn

Py:   if __name__ == "__main__":
来源：http://ee.bjjhwx.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bk.colortex.cn

JS:   require.main === module
来源：http://if.521024.cn

TS:   require.main === module
来源：http://su.szxytkj.cn

Java: public static void main(String[] args)
来源：http://kv.huanxung.cn

Go:   func main()
来源：http://ky.nicolike.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xs.huixiangedu.cn

C#:   static void Main(string[] args)
来源：http://vv.nszjky.cn

[M08] 获取系统与运行时信息
来源：http://yx.nszjky.cn

Py:   platform.system();  platform.python_version()
来源：http://nl.yuexingan06.cn

PHP:  PHP_OS;  phpversion();
来源：http://wb.shxzukj.cn

JS:   process.platform;  process.version
来源：http://mh.szxytkj.cn

TS:   process.platform;  process.version
来源：http://rb.huixinmuqiang.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zh.yuexingan06.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://cl.panjiajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xr.huanxung.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://mc.shtwfgs.cn

================================================================================
来源：http://ro.jctech888.com.cn

N. 数据结构与算法
来源：http://ji.colortex.cn

================================================================================
来源：http://sj.shtwfgs.cn

[N01] 二分查找（有序数组）
来源：http://pr.muxihuayi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ge.521024.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qn.huixiangedu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xr.hnjuh.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zn.jianghongdianzi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xx.nszjky.cn

Go:   sort.SearchInts(arr, x)
来源：http://xa.hahajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://bp.jctech888.com.cn

C#:   Array.BinarySearch(arr, x)
来源：http://fl.wgjwhj.cn

[N02] 排序（工程实践用内置实现）
来源：http://is.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://fh.shxzukj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jj.colortex.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vs.9csxet.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ed.muxihuayi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zz.9csxet.cn

Go:   slices.Sort(arr)
来源：http://sl.asd995.cn

Ruby: arr.sort
来源：http://gt.shxzukj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://pc.szsharing.cn

[N03] 快速排序（分治示例）
来源：http://qz.huixiangedu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xe.jctech888.com.cn

PHP:  // 递归实现，或用 usort
来源：http://jh.shxzukj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nd.gzmigu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xp.shtwfgs.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fj.colortex.cn


<!-- 参考信息 -->