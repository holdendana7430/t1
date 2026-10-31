代发 wailian999

Py:   (end - start).total_seconds()
来源：http://dh.9csxet.cn

PHP:  $end->diff($start)->days;
来源：http://di.yuntaijiaju.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hy.wgjwhj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kw.lnxyls.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bl.yuexingan06.cn

Go:   end.Sub(start).Hours()
来源：http://ms.yuntaijiaju.cn

Ruby: end - start                 # 返回秒数
来源：http://ci.szxytkj.cn

C#:   (end - start).TotalSeconds
来源：http://zt.jctech888.com.cn

[J07] 比较两个日期
来源：http://by.bookmarksfly.cn

Py:   d1 < d2;  d1 == d2
来源：http://sf.huixinmuqiang.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jj.newstarts.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xe.asd995.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ou.yuexingan06.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kb.haigaiapp.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jv.shxzukj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cd.hahajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://mt.bookmarksfly.cn

[J08] 提取年月日与星期
来源：http://fz.panjiajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ce.lnxyls.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ge.muxihuayi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nx.szxytkj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pf.szsharing.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ac.shxzskj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://su.521024.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nk.newstarts.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nv.hahajie.cn

[J09] 时区处理
来源：http://jz.lnxyls.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rw.szxytkj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tu.shxzskj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xh.chemitech.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yc.chemitech.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jw.newstarts.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ux.9csxet.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://na.szsharing.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zn.newstarts.cn

[J10] 取今天 / 本月第一天
来源：http://xa.lnxyls.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vg.haigaiapp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xa.9csxet.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://em.nszjky.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://st.huixiangedu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kh.hnjuh.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yc.gzmigu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pn.chemitech.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sy.lnxyls.cn

================================================================================
来源：http://ki.huixinmuqiang.cn

K. JSON 与序列化
来源：http://us.szxytkj.cn

================================================================================
来源：http://ju.nicolike.cn

[K01] 对象转 JSON 字符串
来源：http://rp.haigaiapp.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jg.wgjwhj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ko.chemitech.net.cn

JS:   JSON.stringify(obj)
来源：http://vg.chemitech.net.cn

TS:   JSON.stringify(obj)
来源：http://sc.huanxung.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gw.szsharing.cn

Go:   json.Marshal(obj)
来源：http://pg.jctech888.com.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ag.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://sw.bookmarksfly.cn

[K02] JSON 字符串转对象
来源：http://yd.bjjhwx.cn

Py:   json.loads(s)
来源：http://ea.jianghongdianzi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ph.newstarts.cn

JS:   JSON.parse(s)
来源：http://ka.huanxung.cn

TS:   JSON.parse(s)
来源：http://ko.521024.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jf.muxihuayi.cn

Go:   json.Unmarshal(data, &v)
来源：http://eg.chemitech.net.cn

Ruby: JSON.parse(s)
来源：http://hq.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mx.hahajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://as.hahajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ab.nszjky.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fp.bookmarksfly.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ts.bookmarksfly.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ru.shtwfgs.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ue.asd995.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hp.huixinmuqiang.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rb.asd995.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wx.521024.cn

[K04] 读取 JSON 文件
来源：http://do.9csxet.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kz.bjjhwx.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ac.huanxung.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://so.nszjky.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kr.huanxung.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wb.shxzukj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gk.newstarts.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ig.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rb.yuntaijiaju.cn

[K05] 深拷贝对象
来源：http://et.jianghongdianzi.cn

Py:   copy.deepcopy(obj)
来源：http://uk.shxzskj.cn

PHP:  unserialize(serialize($obj));
来源：http://qt.9csxet.cn

JS:   structuredClone(obj)
来源：http://uo.panjiajie.cn

TS:   structuredClone(obj)
来源：http://fb.lnxyls.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ln.yuexingan06.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tw.shxzukj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xj.hnjuh.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wu.9csxet.cn

[K06] 解析 URL 查询串
来源：http://sw.bjjhwx.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ax.shxzskj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qb.shtwfgs.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ov.asd995.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gz.asd995.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pn.huanxung.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pz.newstarts.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xn.yuntaijiaju.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://te.huanxung.cn

[K07] 进制转换
来源：http://si.huixinmuqiang.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://en.asd995.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yy.hahajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ai.lnxyls.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jw.szxytkj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fg.jianghongdianzi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mo.szsharing.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bj.bjjhwx.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cp.shtwfgs.cn

[K08] 二进制序列化（非 JSON）
来源：http://wg.bookmarksfly.cn

Py:   pickle.dumps(obj)
来源：http://hb.bjjhwx.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nx.hnjuh.cn

JS:   v8.serialize(obj)        // Node
来源：http://rm.shtwfgs.cn

TS:   v8.serialize(obj)        // Node
来源：http://pv.521024.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ny.jctech888.com.cn

Go:   encoding/gob
来源：http://qw.shxzskj.cn

Ruby: Marshal.dump(obj)
来源：http://js.bjjhwx.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://od.huixinmuqiang.cn

================================================================================
来源：http://ib.huanxung.cn

L. 网络请求
来源：http://lk.asd995.cn

================================================================================
来源：http://py.hahajie.cn

[L01] 发送 GET 请求
来源：http://ce.lnxyls.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bf.szxytkj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lt.newstarts.cn

JS:   await fetch(url)
来源：http://vg.521024.cn

TS:   await fetch(url)
来源：http://ye.asd995.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bf.shtwfgs.cn

Go:   resp, err := http.Get(url)
来源：http://xo.yuntaijiaju.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ev.jianghongdianzi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fa.wgjwhj.cn

[L02] 发送 POST JSON
来源：http://gm.colortex.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xy.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sx.hahajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yl.asd995.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lc.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://te.gzmigu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rl.521024.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ob.szsharing.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zs.9csxet.cn

[L03] 设置自定义请求头
来源：http://mb.hahajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qp.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hx.bjjhwx.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uo.huanxung.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fk.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ol.haigaiapp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://me.hahajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ds.newstarts.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zb.huanxung.cn

[L04] 设置超时
来源：http://mu.chemitech.net.cn

Py:   requests.get(url, timeout=5)
来源：http://fx.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lr.hahajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wk.shxzskj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://se.huixiangedu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sr.bookmarksfly.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://px.haigaiapp.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rp.yuexingan06.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xs.9csxet.cn

[L05] 上传文件（multipart）
来源：http://fg.newstarts.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bv.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ba.521024.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xm.asd995.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zq.muxihuayi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ub.9csxet.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zh.nszjky.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dz.jctech888.com.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ul.shxzukj.cn

[L06] 解析响应为 JSON
来源：http://me.huixiangedu.cn

Py:   resp.json()
来源：http://nv.jctech888.com.cn

PHP:  json_decode($body, true);
来源：http://jj.panjiajie.cn

JS:   await resp.json()
来源：http://qv.jctech888.com.cn

TS:   await resp.json()
来源：http://hj.haigaiapp.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mz.huanxung.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vd.hahajie.cn

Ruby: JSON.parse(resp.body)
来源：http://dm.asd995.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gs.muxihuayi.cn

[L07] 处理 HTTP 状态码
来源：http://xt.haigaiapp.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rp.szsharing.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mm.huixinmuqiang.cn

JS:   resp.ok;  resp.status
来源：http://uo.gzmigu.cn

TS:   resp.ok;  resp.status
来源：http://pu.newstarts.cn

Java: resp.statusCode()
来源：http://xo.huanxung.cn

Go:   resp.StatusCode
来源：http://rv.huixiangedu.cn

Ruby: resp.code.to_i
来源：http://kz.hnjuh.cn

C#:   (int)resp.StatusCode
来源：http://ts.shxzskj.cn

[L08] 并发请求多个地址
来源：http://gl.panjiajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tt.huanxung.cn

PHP:  curl_multi_init() 系列
来源：http://el.chemitech.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zk.panjiajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jp.bjjhwx.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vd.nicolike.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tv.szsharing.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tn.huixinmuqiang.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ke.huixiangedu.cn

================================================================================
来源：http://gk.hnjuh.cn

M. 命令行 / 进程 / 环境
来源：http://oj.yuexingan06.cn

================================================================================
来源：http://dx.huixiangedu.cn

[M01] 读取命令行参数
来源：http://mj.shxzskj.cn

Py:   sys.argv[1:]
来源：http://rb.huixiangedu.cn

PHP:  $argv;  $argc;
来源：http://zj.szsharing.cn

JS:   process.argv.slice(2)
来源：http://yu.chemitech.net.cn

TS:   process.argv.slice(2)
来源：http://fh.jianghongdianzi.cn

Java: args 数组（main 方法参数）
来源：http://bh.yuexingan06.cn

Go:   os.Args[1:]
来源：http://th.szxytkj.cn

Ruby: ARGV
来源：http://ti.haigaiapp.cn

C#:   args 数组（Main 方法参数）
来源：http://xu.chemitech.net.cn

[M02] 读取环境变量
来源：http://ml.huixinmuqiang.cn

Py:   os.environ.get("HOME")
来源：http://ad.bookmarksfly.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ww.bjjhwx.cn

JS:   process.env.HOME
来源：http://sx.muxihuayi.cn

TS:   process.env.HOME
来源：http://vl.gzmigu.cn

Java: System.getenv("HOME")
来源：http://yu.shxzskj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xp.9csxet.cn

Ruby: ENV["HOME"]
来源：http://rs.hnjuh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://os.jianghongdianzi.cn

[M03] 执行外部命令
来源：http://vt.wgjwhj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ph.newstarts.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mx.yuexingan06.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://lj.nszjky.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://uz.hahajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://km.521024.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ed.shxzskj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fe.jctech888.com.cn

C#:   Process.Start("ls", "-l");
来源：http://ae.haigaiapp.cn

[M04] 获取当前工作目录
来源：http://dm.shtwfgs.cn

Py:   os.getcwd()
来源：http://pl.muxihuayi.cn

PHP:  getcwd();
来源：http://ah.jianghongdianzi.cn

JS:   process.cwd()
来源：http://np.yuntaijiaju.cn

TS:   process.cwd()
来源：http://wv.bookmarksfly.cn

Java: Path.of("").toAbsolutePath()
来源：http://oo.521024.cn

Go:   os.Getwd()
来源：http://hs.9csxet.cn

Ruby: Dir.pwd
来源：http://xw.szxytkj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rf.jctech888.com.cn

[M05] 设置退出码
来源：http://pl.hnjuh.cn

Py:   sys.exit(1)
来源：http://ul.chemitech.net.cn

PHP:  exit(1);
来源：http://vf.gzmigu.cn

JS:   process.exit(1)
来源：http://lk.szsharing.cn

TS:   process.exit(1)
来源：http://qz.9csxet.cn

Java: System.exit(1)
来源：http://wo.huanxung.cn

Go:   os.Exit(1)
来源：http://sh.lnxyls.cn

Ruby: exit 1
来源：http://cq.newstarts.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hf.shtwfgs.cn

[M06] 向标准错误输出
来源：http://qp.521024.cn

Py:   print("err", file=sys.stderr)
来源：http://lf.szsharing.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://fg.panjiajie.cn

JS:   console.error("err")
来源：http://bs.yuexingan06.cn

TS:   console.error("err")
来源：http://tg.nszjky.cn

Java: System.err.println("err")
来源：http://px.wgjwhj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ic.huixinmuqiang.cn

Ruby: warn "err"
来源：http://mn.huanxung.cn

C#:   Console.Error.WriteLine("err")
来源：http://tp.shxzukj.cn

[M07] 判断是否为主入口
来源：http://mp.haigaiapp.cn

Py:   if __name__ == "__main__":
来源：http://da.lnxyls.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ga.nszjky.cn

JS:   require.main === module
来源：http://yq.nicolike.cn

TS:   require.main === module
来源：http://az.szxytkj.cn

Java: public static void main(String[] args)
来源：http://vd.szsharing.cn

Go:   func main()
来源：http://wh.shtwfgs.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wy.chemitech.net.cn

C#:   static void Main(string[] args)
来源：http://oj.shxzukj.cn

[M08] 获取系统与运行时信息
来源：http://qf.huanxung.cn

Py:   platform.system();  platform.python_version()
来源：http://eo.hahajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://st.haigaiapp.cn

JS:   process.platform;  process.version
来源：http://ac.bjjhwx.cn

TS:   process.platform;  process.version
来源：http://ya.jctech888.com.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://iy.gzmigu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gl.chemitech.net.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uy.jianghongdianzi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wb.lnxyls.cn

================================================================================
来源：http://tc.hnjuh.cn

N. 数据结构与算法
来源：http://ls.colortex.cn

================================================================================
来源：http://rq.lnxyls.cn

[N01] 二分查找（有序数组）
来源：http://tc.huixiangedu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vo.huanxung.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pv.newstarts.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yx.9csxet.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gf.yuntaijiaju.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jd.521024.cn

Go:   sort.SearchInts(arr, x)
来源：http://xt.9csxet.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mr.nszjky.cn

C#:   Array.BinarySearch(arr, x)
来源：http://tx.shxzskj.cn

[N02] 排序（工程实践用内置实现）
来源：http://br.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://vv.shxzukj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ye.newstarts.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wq.yuntaijiaju.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pw.shtwfgs.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jh.huanxung.cn

Go:   slices.Sort(arr)
来源：http://kt.shxzukj.cn

Ruby: arr.sort
来源：http://mi.yuexingan06.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bn.asd995.cn

[N03] 快速排序（分治示例）
来源：http://ad.521024.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fr.haigaiapp.cn

PHP:  // 递归实现，或用 usort
来源：http://rh.yuexingan06.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ha.colortex.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vh.wgjwhj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ci.huanxung.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://my.huanxung.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sw.shxzukj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ze.szsharing.cn

[N04] 斐波那契数列
来源：http://gr.panjiajie.cn


<!-- 参考信息 -->