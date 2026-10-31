代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mm.panjiajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gf.szsharing.cn

[J05] 时间加减（加 7 天）
来源：http://yx.shxzskj.cn

Py:   now + timedelta(days=7)
来源：http://ee.hahajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://on.huixiangedu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.9csxet.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vr.haigaiapp.cn

Java: LocalDate.now().plusDays(7)
来源：http://ef.nszjky.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cc.hahajie.cn

Ruby: Time.now + 7 * 86400
来源：http://un.9csxet.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vf.szsharing.cn

[J06] 计算两时间之差
来源：http://uh.huixinmuqiang.cn

Py:   (end - start).total_seconds()
来源：http://xi.szxytkj.cn

PHP:  $end->diff($start)->days;
来源：http://dq.521024.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gb.shtwfgs.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fq.colortex.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mk.wgjwhj.cn

Go:   end.Sub(start).Hours()
来源：http://ik.yuntaijiaju.cn

Ruby: end - start                 # 返回秒数
来源：http://on.lnxyls.cn

C#:   (end - start).TotalSeconds
来源：http://bd.newstarts.cn

[J07] 比较两个日期
来源：http://qr.jctech888.com.cn

Py:   d1 < d2;  d1 == d2
来源：http://zt.hnjuh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://io.chemitech.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://li.hnjuh.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mv.huixiangedu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xw.521024.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tk.szsharing.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fy.huixiangedu.cn

C#:   d1 < d2;  d1 == d2
来源：http://lf.newstarts.cn

[J08] 提取年月日与星期
来源：http://er.shtwfgs.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://eb.yuntaijiaju.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cx.asd995.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qm.gzmigu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tj.521024.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rb.shxzukj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://it.colortex.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://en.szxytkj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kg.haigaiapp.cn

[J09] 时区处理
来源：http://vt.szsharing.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ae.bookmarksfly.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pj.9csxet.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://to.newstarts.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cq.haigaiapp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yd.shtwfgs.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rn.yuexingan06.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ru.jctech888.com.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qr.chemitech.net.cn

[J10] 取今天 / 本月第一天
来源：http://mt.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cy.521024.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fg.wgjwhj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ha.muxihuayi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xl.shxzukj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ww.panjiajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ar.colortex.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vh.asd995.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://et.huixinmuqiang.cn

================================================================================
来源：http://eo.newstarts.cn

K. JSON 与序列化
来源：http://lj.shtwfgs.cn

================================================================================
来源：http://gz.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://sq.huanxung.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vp.shxzukj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ng.panjiajie.cn

JS:   JSON.stringify(obj)
来源：http://ae.wgjwhj.cn

TS:   JSON.stringify(obj)
来源：http://dz.jianghongdianzi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lb.asd995.cn

Go:   json.Marshal(obj)
来源：http://qb.lnxyls.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mb.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://we.jianghongdianzi.cn

[K02] JSON 字符串转对象
来源：http://kz.hnjuh.cn

Py:   json.loads(s)
来源：http://oo.huixinmuqiang.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://si.bookmarksfly.cn

JS:   JSON.parse(s)
来源：http://oh.colortex.cn

TS:   JSON.parse(s)
来源：http://zr.bjjhwx.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://py.lnxyls.cn

Go:   json.Unmarshal(data, &v)
来源：http://vw.gzmigu.cn

Ruby: JSON.parse(s)
来源：http://gz.hnjuh.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cv.chemitech.net.cn

[K03] JSON 美化输出（带缩进）
来源：http://td.jianghongdianzi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rn.521024.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fo.newstarts.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://co.jianghongdianzi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fo.gzmigu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xi.muxihuayi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wm.nicolike.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rl.colortex.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tz.hahajie.cn

[K04] 读取 JSON 文件
来源：http://tu.hnjuh.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vm.huanxung.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gl.nicolike.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://de.asd995.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zf.haigaiapp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yl.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://aa.nszjky.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gj.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://li.szsharing.cn

[K05] 深拷贝对象
来源：http://is.jianghongdianzi.cn

Py:   copy.deepcopy(obj)
来源：http://dn.yuntaijiaju.cn

PHP:  unserialize(serialize($obj));
来源：http://er.hahajie.cn

JS:   structuredClone(obj)
来源：http://is.shtwfgs.cn

TS:   structuredClone(obj)
来源：http://fw.szxytkj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://np.lnxyls.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ls.szxytkj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qi.lnxyls.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xl.shxzukj.cn

[K06] 解析 URL 查询串
来源：http://zi.szsharing.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wx.asd995.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sp.szxytkj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gr.asd995.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://io.yuexingan06.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xq.haigaiapp.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pd.panjiajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oz.szxytkj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bj.nicolike.cn

[K07] 进制转换
来源：http://jr.hahajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jv.9csxet.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pl.szsharing.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wz.nicolike.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jn.huixinmuqiang.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://is.gzmigu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mg.shtwfgs.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ua.colortex.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://iq.yuntaijiaju.cn

[K08] 二进制序列化（非 JSON）
来源：http://cx.lnxyls.cn

Py:   pickle.dumps(obj)
来源：http://ue.bjjhwx.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ub.hahajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://em.huixiangedu.cn

TS:   v8.serialize(obj)        // Node
来源：http://kd.jianghongdianzi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fr.szxytkj.cn

Go:   encoding/gob
来源：http://ju.huixinmuqiang.cn

Ruby: Marshal.dump(obj)
来源：http://ys.colortex.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dt.haigaiapp.cn

================================================================================
来源：http://mz.szsharing.cn

L. 网络请求
来源：http://kp.wgjwhj.cn

================================================================================
来源：http://ll.panjiajie.cn

[L01] 发送 GET 请求
来源：http://mk.lnxyls.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xx.9csxet.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tp.521024.cn

JS:   await fetch(url)
来源：http://yw.yuexingan06.cn

TS:   await fetch(url)
来源：http://kf.colortex.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gq.nicolike.cn

Go:   resp, err := http.Get(url)
来源：http://zy.jianghongdianzi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://lo.haigaiapp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uf.bjjhwx.cn

[L02] 发送 POST JSON
来源：http://qd.szsharing.cn

Py:   requests.post(url, json={"a": 1})
来源：http://os.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mw.hahajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ov.bjjhwx.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pd.colortex.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pq.szxytkj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://to.lnxyls.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://aw.szsharing.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://md.haigaiapp.cn

[L03] 设置自定义请求头
来源：http://vm.jianghongdianzi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vd.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qr.shxzskj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yy.chemitech.net.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tu.asd995.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zj.chemitech.net.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nk.shxzskj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ds.hahajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ux.bookmarksfly.cn

[L04] 设置超时
来源：http://tn.huixinmuqiang.cn

Py:   requests.get(url, timeout=5)
来源：http://fk.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fz.lnxyls.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ls.szxytkj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dl.wgjwhj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xu.gzmigu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yc.hnjuh.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fm.shxzskj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pm.bookmarksfly.cn

[L05] 上传文件（multipart）
来源：http://ud.jctech888.com.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nh.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hq.wgjwhj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hn.yuntaijiaju.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vu.hnjuh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yw.chemitech.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zn.bookmarksfly.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nb.hahajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nt.jianghongdianzi.cn

[L06] 解析响应为 JSON
来源：http://qk.asd995.cn

Py:   resp.json()
来源：http://ku.newstarts.cn

PHP:  json_decode($body, true);
来源：http://ub.szxytkj.cn

JS:   await resp.json()
来源：http://ci.szxytkj.cn

TS:   await resp.json()
来源：http://lu.chemitech.net.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ky.shxzukj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zj.jctech888.com.cn

Ruby: JSON.parse(resp.body)
来源：http://do.jctech888.com.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pl.haigaiapp.cn

[L07] 处理 HTTP 状态码
来源：http://bi.shxzukj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qe.nicolike.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rs.hahajie.cn

JS:   resp.ok;  resp.status
来源：http://mu.bookmarksfly.cn

TS:   resp.ok;  resp.status
来源：http://vc.shxzukj.cn

Java: resp.statusCode()
来源：http://bx.shxzskj.cn

Go:   resp.StatusCode
来源：http://aj.hnjuh.cn

Ruby: resp.code.to_i
来源：http://bp.szxytkj.cn

C#:   (int)resp.StatusCode
来源：http://yn.huixiangedu.cn

[L08] 并发请求多个地址
来源：http://nn.nszjky.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xj.szxytkj.cn

PHP:  curl_multi_init() 系列
来源：http://yy.asd995.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nz.yuexingan06.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ua.521024.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wz.szxytkj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xd.yuexingan06.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://eo.asd995.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ra.shxzukj.cn

================================================================================
来源：http://ln.muxihuayi.cn

M. 命令行 / 进程 / 环境
来源：http://en.521024.cn

================================================================================
来源：http://lz.shxzukj.cn

[M01] 读取命令行参数
来源：http://gc.asd995.cn

Py:   sys.argv[1:]
来源：http://nw.huanxung.cn

PHP:  $argv;  $argc;
来源：http://ml.hahajie.cn

JS:   process.argv.slice(2)
来源：http://fk.huixinmuqiang.cn

TS:   process.argv.slice(2)
来源：http://op.shtwfgs.cn

Java: args 数组（main 方法参数）
来源：http://xw.lnxyls.cn

Go:   os.Args[1:]
来源：http://kh.jianghongdianzi.cn

Ruby: ARGV
来源：http://hv.shxzukj.cn

C#:   args 数组（Main 方法参数）
来源：http://gs.shxzskj.cn

[M02] 读取环境变量
来源：http://tk.newstarts.cn

Py:   os.environ.get("HOME")
来源：http://op.newstarts.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sy.szsharing.cn

JS:   process.env.HOME
来源：http://fu.chemitech.net.cn

TS:   process.env.HOME
来源：http://ve.shxzukj.cn

Java: System.getenv("HOME")
来源：http://df.bookmarksfly.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nx.nicolike.cn

Ruby: ENV["HOME"]
来源：http://eg.jctech888.com.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vl.hahajie.cn

[M03] 执行外部命令
来源：http://bx.muxihuayi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nl.chemitech.net.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://me.lnxyls.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://rk.hahajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vf.wgjwhj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://to.bjjhwx.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ip.colortex.cn

Ruby: system("ls -l");  `ls -l`
来源：http://la.haigaiapp.cn

C#:   Process.Start("ls", "-l");
来源：http://av.lnxyls.cn

[M04] 获取当前工作目录
来源：http://jq.shxzskj.cn

Py:   os.getcwd()
来源：http://ss.lnxyls.cn

PHP:  getcwd();
来源：http://zh.yuexingan06.cn

JS:   process.cwd()
来源：http://lz.bjjhwx.cn

TS:   process.cwd()
来源：http://rq.nszjky.cn

Java: Path.of("").toAbsolutePath()
来源：http://pf.shtwfgs.cn

Go:   os.Getwd()
来源：http://xc.bjjhwx.cn

Ruby: Dir.pwd
来源：http://ic.newstarts.cn

C#:   Directory.GetCurrentDirectory()
来源：http://co.newstarts.cn

[M05] 设置退出码
来源：http://bw.bookmarksfly.cn

Py:   sys.exit(1)
来源：http://kx.hahajie.cn

PHP:  exit(1);
来源：http://lh.shtwfgs.cn

JS:   process.exit(1)
来源：http://sv.hnjuh.cn

TS:   process.exit(1)
来源：http://fc.chemitech.net.cn

Java: System.exit(1)
来源：http://jm.jianghongdianzi.cn

Go:   os.Exit(1)
来源：http://en.nicolike.cn

Ruby: exit 1
来源：http://kg.lnxyls.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rc.yuntaijiaju.cn

[M06] 向标准错误输出
来源：http://xg.colortex.cn

Py:   print("err", file=sys.stderr)
来源：http://ls.shxzukj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ut.shtwfgs.cn

JS:   console.error("err")
来源：http://uh.jianghongdianzi.cn

TS:   console.error("err")
来源：http://wg.nszjky.cn

Java: System.err.println("err")
来源：http://uc.shxzskj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://if.521024.cn

Ruby: warn "err"
来源：http://hd.colortex.cn

C#:   Console.Error.WriteLine("err")
来源：http://ct.lnxyls.cn

[M07] 判断是否为主入口
来源：http://hj.lnxyls.cn

Py:   if __name__ == "__main__":
来源：http://pj.huixiangedu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wn.panjiajie.cn

JS:   require.main === module
来源：http://lh.shxzukj.cn

TS:   require.main === module
来源：http://hy.szsharing.cn

Java: public static void main(String[] args)
来源：http://sl.9csxet.cn

Go:   func main()
来源：http://sa.bjjhwx.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bp.521024.cn

C#:   static void Main(string[] args)
来源：http://vw.hnjuh.cn

[M08] 获取系统与运行时信息
来源：http://jy.hahajie.cn

Py:   platform.system();  platform.python_version()
来源：http://by.9csxet.cn

PHP:  PHP_OS;  phpversion();
来源：http://fa.jctech888.com.cn

JS:   process.platform;  process.version
来源：http://dz.szsharing.cn

TS:   process.platform;  process.version
来源：http://uo.shxzskj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qm.asd995.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bn.521024.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jg.jctech888.com.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://le.haigaiapp.cn

================================================================================
来源：http://cm.shtwfgs.cn

N. 数据结构与算法
来源：http://eq.gzmigu.cn

================================================================================
来源：http://ot.bjjhwx.cn

[N01] 二分查找（有序数组）
来源：http://rg.huixinmuqiang.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ga.hnjuh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yf.huanxung.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://aq.jianghongdianzi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mt.yuexingan06.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qj.chemitech.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://tk.bjjhwx.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ui.chemitech.net.cn

C#:   Array.BinarySearch(arr, x)
来源：http://it.colortex.cn

[N02] 排序（工程实践用内置实现）
来源：http://rr.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://fd.huanxung.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://me.nszjky.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vp.jianghongdianzi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://lp.lnxyls.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cg.yuexingan06.cn

Go:   slices.Sort(arr)
来源：http://kh.gzmigu.cn


<!-- 参考信息 -->