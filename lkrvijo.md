代发 wailian999

Py:   (end - start).total_seconds()
来源：http://yy.jianghongdianzi.cn

PHP:  $end->diff($start)->days;
来源：http://hz.hahajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wd.huixiangedu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vw.chemitech.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ub.wgjwhj.cn

Go:   end.Sub(start).Hours()
来源：http://pw.yuexingan06.cn

Ruby: end - start                 # 返回秒数
来源：http://xv.huixiangedu.cn

C#:   (end - start).TotalSeconds
来源：http://qd.hnjuh.cn

[J07] 比较两个日期
来源：http://nl.nicolike.cn

Py:   d1 < d2;  d1 == d2
来源：http://aw.huixinmuqiang.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bk.bjjhwx.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ry.bookmarksfly.cn

TS:   d1.getTime() < d2.getTime()
来源：http://oc.asd995.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zd.colortex.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://re.yuntaijiaju.cn

Ruby: d1 < d2;  d1 == d2
来源：http://nk.szxytkj.cn

C#:   d1 < d2;  d1 == d2
来源：http://zd.asd995.cn

[J08] 提取年月日与星期
来源：http://qx.huanxung.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qd.yuntaijiaju.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gj.chemitech.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wv.gzmigu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dl.yuntaijiaju.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rn.yuexingan06.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ka.huanxung.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ra.nszjky.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wd.bjjhwx.cn

[J09] 时区处理
来源：http://cl.huixiangedu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vo.nszjky.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zm.hnjuh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xj.jianghongdianzi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oq.hnjuh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bi.huixiangedu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pr.jianghongdianzi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pw.521024.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xk.szxytkj.cn

[J10] 取今天 / 本月第一天
来源：http://vn.9csxet.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://no.shxzskj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bz.haigaiapp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://th.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fp.bjjhwx.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ai.jianghongdianzi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://le.jctech888.com.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hu.huanxung.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zr.jianghongdianzi.cn

================================================================================
来源：http://va.hnjuh.cn

K. JSON 与序列化
来源：http://rr.jctech888.com.cn

================================================================================
来源：http://va.huanxung.cn

[K01] 对象转 JSON 字符串
来源：http://wm.nszjky.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fj.yuexingan06.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zb.9csxet.cn

JS:   JSON.stringify(obj)
来源：http://cg.szxytkj.cn

TS:   JSON.stringify(obj)
来源：http://tg.9csxet.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bm.hnjuh.cn

Go:   json.Marshal(obj)
来源：http://kx.bjjhwx.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cz.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hx.jianghongdianzi.cn

[K02] JSON 字符串转对象
来源：http://xo.shtwfgs.cn

Py:   json.loads(s)
来源：http://wu.huixinmuqiang.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jy.jianghongdianzi.cn

JS:   JSON.parse(s)
来源：http://mj.haigaiapp.cn

TS:   JSON.parse(s)
来源：http://wx.huanxung.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tv.shtwfgs.cn

Go:   json.Unmarshal(data, &v)
来源：http://bp.shtwfgs.cn

Ruby: JSON.parse(s)
来源：http://cg.colortex.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://aq.newstarts.cn

[K03] JSON 美化输出（带缩进）
来源：http://yi.jianghongdianzi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://li.hnjuh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://uu.panjiajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://md.lnxyls.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rb.huixiangedu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wm.nicolike.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tp.szxytkj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://er.szxytkj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dv.wgjwhj.cn

[K04] 读取 JSON 文件
来源：http://eb.shxzskj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ql.hahajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tv.hnjuh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ds.muxihuayi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iy.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://id.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://eo.nszjky.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://pn.colortex.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zm.chemitech.net.cn

[K05] 深拷贝对象
来源：http://ch.bookmarksfly.cn

Py:   copy.deepcopy(obj)
来源：http://dh.huixinmuqiang.cn

PHP:  unserialize(serialize($obj));
来源：http://ce.shtwfgs.cn

JS:   structuredClone(obj)
来源：http://th.newstarts.cn

TS:   structuredClone(obj)
来源：http://yp.9csxet.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rd.huixiangedu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://eo.yuexingan06.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qm.yuexingan06.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qr.shtwfgs.cn

[K06] 解析 URL 查询串
来源：http://qp.muxihuayi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nr.jctech888.com.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vc.nicolike.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nv.panjiajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gy.wgjwhj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ts.hahajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xt.newstarts.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dd.huanxung.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uz.muxihuayi.cn

[K07] 进制转换
来源：http://qo.huanxung.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nk.huanxung.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yq.9csxet.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ks.asd995.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zm.gzmigu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://af.haigaiapp.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ze.chemitech.net.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vw.lnxyls.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tk.nicolike.cn

[K08] 二进制序列化（非 JSON）
来源：http://aq.bookmarksfly.cn

Py:   pickle.dumps(obj)
来源：http://ie.hnjuh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ju.huixinmuqiang.cn

JS:   v8.serialize(obj)        // Node
来源：http://hb.huixinmuqiang.cn

TS:   v8.serialize(obj)        // Node
来源：http://th.gzmigu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ir.jctech888.com.cn

Go:   encoding/gob
来源：http://ct.wgjwhj.cn

Ruby: Marshal.dump(obj)
来源：http://oz.bookmarksfly.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zf.newstarts.cn

================================================================================
来源：http://ew.huanxung.cn

L. 网络请求
来源：http://lx.shtwfgs.cn

================================================================================
来源：http://vs.haigaiapp.cn

[L01] 发送 GET 请求
来源：http://ju.haigaiapp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ul.colortex.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xh.huanxung.cn

JS:   await fetch(url)
来源：http://wr.muxihuayi.cn

TS:   await fetch(url)
来源：http://wy.bjjhwx.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cx.shtwfgs.cn

Go:   resp, err := http.Get(url)
来源：http://iw.hahajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://nv.gzmigu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fa.yuexingan06.cn

[L02] 发送 POST JSON
来源：http://vl.521024.cn

Py:   requests.post(url, json={"a": 1})
来源：http://tw.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gq.muxihuayi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://re.nszjky.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oc.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://io.szxytkj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pn.colortex.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://co.chemitech.net.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fj.bookmarksfly.cn

[L03] 设置自定义请求头
来源：http://ic.hnjuh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://az.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fh.colortex.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wa.huixiangedu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gd.521024.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ll.muxihuayi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uz.chemitech.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jy.huixinmuqiang.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kj.colortex.cn

[L04] 设置超时
来源：http://wr.newstarts.cn

Py:   requests.get(url, timeout=5)
来源：http://zc.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lu.huixinmuqiang.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nq.bookmarksfly.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cy.newstarts.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tw.nszjky.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://it.bjjhwx.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kv.nszjky.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://eg.lnxyls.cn

[L05] 上传文件（multipart）
来源：http://fi.hnjuh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tp.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://oj.wgjwhj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gj.muxihuayi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dz.jctech888.com.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fq.9csxet.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vp.nszjky.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ex.huixiangedu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://px.shxzskj.cn

[L06] 解析响应为 JSON
来源：http://dc.hahajie.cn

Py:   resp.json()
来源：http://vb.chemitech.net.cn

PHP:  json_decode($body, true);
来源：http://jc.521024.cn

JS:   await resp.json()
来源：http://sy.yuntaijiaju.cn

TS:   await resp.json()
来源：http://xt.wgjwhj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bi.hahajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qm.haigaiapp.cn

Ruby: JSON.parse(resp.body)
来源：http://kl.yuntaijiaju.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ep.yuexingan06.cn

[L07] 处理 HTTP 状态码
来源：http://rk.haigaiapp.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nh.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rn.yuntaijiaju.cn

JS:   resp.ok;  resp.status
来源：http://ir.9csxet.cn

TS:   resp.ok;  resp.status
来源：http://em.hnjuh.cn

Java: resp.statusCode()
来源：http://hr.521024.cn

Go:   resp.StatusCode
来源：http://jm.gzmigu.cn

Ruby: resp.code.to_i
来源：http://jz.jctech888.com.cn

C#:   (int)resp.StatusCode
来源：http://si.colortex.cn

[L08] 并发请求多个地址
来源：http://de.shxzskj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ia.shxzukj.cn

PHP:  curl_multi_init() 系列
来源：http://uu.lnxyls.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pa.huixiangedu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nz.huanxung.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jk.szxytkj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ak.gzmigu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://me.shtwfgs.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gb.hahajie.cn

================================================================================
来源：http://ii.shxzukj.cn

M. 命令行 / 进程 / 环境
来源：http://fs.521024.cn

================================================================================
来源：http://av.colortex.cn

[M01] 读取命令行参数
来源：http://do.521024.cn

Py:   sys.argv[1:]
来源：http://dg.shxzukj.cn

PHP:  $argv;  $argc;
来源：http://ui.huanxung.cn

JS:   process.argv.slice(2)
来源：http://ey.huixinmuqiang.cn

TS:   process.argv.slice(2)
来源：http://pl.szsharing.cn

Java: args 数组（main 方法参数）
来源：http://yn.nicolike.cn

Go:   os.Args[1:]
来源：http://ma.yuntaijiaju.cn

Ruby: ARGV
来源：http://do.colortex.cn

C#:   args 数组（Main 方法参数）
来源：http://ui.haigaiapp.cn

[M02] 读取环境变量
来源：http://sq.asd995.cn

Py:   os.environ.get("HOME")
来源：http://ol.newstarts.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://oo.shxzukj.cn

JS:   process.env.HOME
来源：http://yc.huixiangedu.cn

TS:   process.env.HOME
来源：http://xg.huixiangedu.cn

Java: System.getenv("HOME")
来源：http://bh.9csxet.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ky.yuntaijiaju.cn

Ruby: ENV["HOME"]
来源：http://px.shxzukj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uq.szsharing.cn

[M03] 执行外部命令
来源：http://dr.521024.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nt.jianghongdianzi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://sj.9csxet.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qd.huixinmuqiang.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vo.hnjuh.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lw.newstarts.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qj.huixiangedu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://mc.huixinmuqiang.cn

C#:   Process.Start("ls", "-l");
来源：http://uy.nicolike.cn

[M04] 获取当前工作目录
来源：http://vc.nszjky.cn

Py:   os.getcwd()
来源：http://sq.jianghongdianzi.cn

PHP:  getcwd();
来源：http://og.newstarts.cn

JS:   process.cwd()
来源：http://pc.hnjuh.cn

TS:   process.cwd()
来源：http://db.haigaiapp.cn

Java: Path.of("").toAbsolutePath()
来源：http://ft.huanxung.cn

Go:   os.Getwd()
来源：http://yd.huanxung.cn

Ruby: Dir.pwd
来源：http://uf.szsharing.cn

C#:   Directory.GetCurrentDirectory()
来源：http://js.newstarts.cn

[M05] 设置退出码
来源：http://fm.nicolike.cn

Py:   sys.exit(1)
来源：http://yi.szsharing.cn

PHP:  exit(1);
来源：http://du.hnjuh.cn

JS:   process.exit(1)
来源：http://ei.muxihuayi.cn

TS:   process.exit(1)
来源：http://eh.huixinmuqiang.cn

Java: System.exit(1)
来源：http://np.szsharing.cn

Go:   os.Exit(1)
来源：http://yu.huixinmuqiang.cn

Ruby: exit 1
来源：http://ds.hnjuh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fy.9csxet.cn

[M06] 向标准错误输出
来源：http://du.huanxung.cn

Py:   print("err", file=sys.stderr)
来源：http://ms.huixinmuqiang.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://di.lnxyls.cn

JS:   console.error("err")
来源：http://am.chemitech.net.cn

TS:   console.error("err")
来源：http://vu.shxzukj.cn

Java: System.err.println("err")
来源：http://fk.huanxung.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qt.chemitech.net.cn

Ruby: warn "err"
来源：http://va.yuexingan06.cn

C#:   Console.Error.WriteLine("err")
来源：http://ef.chemitech.net.cn

[M07] 判断是否为主入口
来源：http://pz.gzmigu.cn

Py:   if __name__ == "__main__":
来源：http://gq.gzmigu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xk.521024.cn

JS:   require.main === module
来源：http://gq.panjiajie.cn

TS:   require.main === module
来源：http://nc.bookmarksfly.cn

Java: public static void main(String[] args)
来源：http://dp.nszjky.cn

Go:   func main()
来源：http://vx.huanxung.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://by.jianghongdianzi.cn

C#:   static void Main(string[] args)
来源：http://mn.bookmarksfly.cn

[M08] 获取系统与运行时信息
来源：http://bv.newstarts.cn

Py:   platform.system();  platform.python_version()
来源：http://mt.bjjhwx.cn

PHP:  PHP_OS;  phpversion();
来源：http://vz.wgjwhj.cn

JS:   process.platform;  process.version
来源：http://pp.asd995.cn

TS:   process.platform;  process.version
来源：http://mh.521024.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://do.nszjky.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ne.muxihuayi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vt.9csxet.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gt.haigaiapp.cn

================================================================================
来源：http://hg.yuntaijiaju.cn

N. 数据结构与算法
来源：http://pw.yuexingan06.cn

================================================================================
来源：http://sn.gzmigu.cn

[N01] 二分查找（有序数组）
来源：http://ro.muxihuayi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ta.nszjky.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sf.jianghongdianzi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zq.hnjuh.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lt.yuexingan06.cn

Java: Arrays.binarySearch(arr, x)
来源：http://dd.hahajie.cn

Go:   sort.SearchInts(arr, x)
来源：http://rg.newstarts.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yi.huanxung.cn

C#:   Array.BinarySearch(arr, x)
来源：http://lj.shxzukj.cn

[N02] 排序（工程实践用内置实现）
来源：http://me.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://rj.huixinmuqiang.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fm.lnxyls.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://sw.chemitech.net.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ff.yuexingan06.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lz.yuntaijiaju.cn

Go:   slices.Sort(arr)
来源：http://ts.muxihuayi.cn

Ruby: arr.sort
来源：http://ib.asd995.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ju.nicolike.cn

[N03] 快速排序（分治示例）
来源：http://iv.huanxung.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gk.muxihuayi.cn

PHP:  // 递归实现，或用 usort
来源：http://rn.jctech888.com.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lo.hahajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cs.szsharing.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://it.521024.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://af.hnjuh.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://so.yuntaijiaju.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wr.nszjky.cn

[N04] 斐波那契数列
来源：http://lv.huixiangedu.cn


<!-- 参考信息 -->