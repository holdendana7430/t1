代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ou.nszjky.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ve.newstarts.cn

[J05] 时间加减（加 7 天）
来源：http://sc.jctech888.com.cn

Py:   now + timedelta(days=7)
来源：http://fc.colortex.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bl.nicolike.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qf.yuexingan06.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lf.wgjwhj.cn

Java: LocalDate.now().plusDays(7)
来源：http://de.bookmarksfly.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ag.bookmarksfly.cn

Ruby: Time.now + 7 * 86400
来源：http://qx.bjjhwx.cn

C#:   DateTime.Now.AddDays(7)
来源：http://uq.huixinmuqiang.cn

[J06] 计算两时间之差
来源：http://wz.gzmigu.cn

Py:   (end - start).total_seconds()
来源：http://iy.shtwfgs.cn

PHP:  $end->diff($start)->days;
来源：http://yk.shxzskj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fp.szxytkj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mt.panjiajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://er.chemitech.net.cn

Go:   end.Sub(start).Hours()
来源：http://um.hnjuh.cn

Ruby: end - start                 # 返回秒数
来源：http://tf.jianghongdianzi.cn

C#:   (end - start).TotalSeconds
来源：http://pa.panjiajie.cn

[J07] 比较两个日期
来源：http://ej.9csxet.cn

Py:   d1 < d2;  d1 == d2
来源：http://bw.hnjuh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lk.haigaiapp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://oq.szsharing.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xe.bjjhwx.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zl.shxzukj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lr.nszjky.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ev.hnjuh.cn

C#:   d1 < d2;  d1 == d2
来源：http://bt.bookmarksfly.cn

[J08] 提取年月日与星期
来源：http://rg.huixinmuqiang.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bc.szxytkj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://af.bjjhwx.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ff.panjiajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uy.nicolike.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ey.jctech888.com.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vk.bjjhwx.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://iy.shtwfgs.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ue.colortex.cn

[J09] 时区处理
来源：http://jj.yuexingan06.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gd.lnxyls.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ms.hnjuh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oj.huanxung.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zx.bookmarksfly.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vl.huixinmuqiang.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jc.hahajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qk.haigaiapp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rx.gzmigu.cn

[J10] 取今天 / 本月第一天
来源：http://cj.shxzukj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vd.huixiangedu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rc.huanxung.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wp.hnjuh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ho.nicolike.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ak.huixinmuqiang.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://de.yuexingan06.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dl.9csxet.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nn.hnjuh.cn

================================================================================
来源：http://ef.huixiangedu.cn

K. JSON 与序列化
来源：http://ak.hnjuh.cn

================================================================================
来源：http://kg.huixinmuqiang.cn

[K01] 对象转 JSON 字符串
来源：http://bo.shxzukj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zn.colortex.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://th.nszjky.cn

JS:   JSON.stringify(obj)
来源：http://eh.asd995.cn

TS:   JSON.stringify(obj)
来源：http://ja.shxzukj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bn.jianghongdianzi.cn

Go:   json.Marshal(obj)
来源：http://my.shxzskj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://in.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://eg.hnjuh.cn

[K02] JSON 字符串转对象
来源：http://en.huanxung.cn

Py:   json.loads(s)
来源：http://rm.yuntaijiaju.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gy.huixiangedu.cn

JS:   JSON.parse(s)
来源：http://xr.asd995.cn

TS:   JSON.parse(s)
来源：http://wc.hahajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://it.haigaiapp.cn

Go:   json.Unmarshal(data, &v)
来源：http://ga.huixinmuqiang.cn

Ruby: JSON.parse(s)
来源：http://aw.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tu.bjjhwx.cn

[K03] JSON 美化输出（带缩进）
来源：http://gc.wgjwhj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://my.lnxyls.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xs.gzmigu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qq.shxzskj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yt.asd995.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oq.bookmarksfly.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uz.nszjky.cn

Ruby: JSON.pretty_generate(obj)
来源：http://cp.shxzskj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mn.nicolike.cn

[K04] 读取 JSON 文件
来源：http://wh.9csxet.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://em.colortex.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xc.wgjwhj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://if.hahajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tm.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qj.9csxet.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rh.9csxet.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vb.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jm.huixinmuqiang.cn

[K05] 深拷贝对象
来源：http://zd.gzmigu.cn

Py:   copy.deepcopy(obj)
来源：http://il.521024.cn

PHP:  unserialize(serialize($obj));
来源：http://pj.panjiajie.cn

JS:   structuredClone(obj)
来源：http://zz.huanxung.cn

TS:   structuredClone(obj)
来源：http://hb.yuntaijiaju.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ta.gzmigu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hv.szsharing.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://oj.yuntaijiaju.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tp.jianghongdianzi.cn

[K06] 解析 URL 查询串
来源：http://ga.hnjuh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pu.nszjky.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://uj.hahajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iq.chemitech.net.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qp.gzmigu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pg.shtwfgs.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qa.bookmarksfly.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://io.colortex.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nm.yuntaijiaju.cn

[K07] 进制转换
来源：http://rd.gzmigu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sk.gzmigu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ah.newstarts.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://at.wgjwhj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lr.asd995.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vo.szsharing.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wf.yuexingan06.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bu.521024.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nt.huixiangedu.cn

[K08] 二进制序列化（非 JSON）
来源：http://jj.newstarts.cn

Py:   pickle.dumps(obj)
来源：http://mx.panjiajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xa.nicolike.cn

JS:   v8.serialize(obj)        // Node
来源：http://yc.huixiangedu.cn

TS:   v8.serialize(obj)        // Node
来源：http://xf.bookmarksfly.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gs.shxzskj.cn

Go:   encoding/gob
来源：http://hi.yuntaijiaju.cn

Ruby: Marshal.dump(obj)
来源：http://zj.asd995.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lz.lnxyls.cn

================================================================================
来源：http://ne.lnxyls.cn

L. 网络请求
来源：http://vf.nicolike.cn

================================================================================
来源：http://jz.panjiajie.cn

[L01] 发送 GET 请求
来源：http://vr.bookmarksfly.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://oh.lnxyls.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gh.colortex.cn

JS:   await fetch(url)
来源：http://ki.panjiajie.cn

TS:   await fetch(url)
来源：http://ux.wgjwhj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hs.szxytkj.cn

Go:   resp, err := http.Get(url)
来源：http://xo.jctech888.com.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qm.szsharing.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://te.asd995.cn

[L02] 发送 POST JSON
来源：http://nu.shxzskj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nz.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vv.colortex.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gp.9csxet.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wy.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ez.yuntaijiaju.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kq.9csxet.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cj.newstarts.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sp.9csxet.cn

[L03] 设置自定义请求头
来源：http://mi.szxytkj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jn.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wf.nicolike.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qe.shxzukj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mq.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tk.huixiangedu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hv.nicolike.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jy.lnxyls.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tm.muxihuayi.cn

[L04] 设置超时
来源：http://mn.521024.cn

Py:   requests.get(url, timeout=5)
来源：http://au.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ed.haigaiapp.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tw.shtwfgs.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nu.521024.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://es.huixiangedu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xu.lnxyls.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cc.shtwfgs.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dt.haigaiapp.cn

[L05] 上传文件（multipart）
来源：http://wt.wgjwhj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dg.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ef.huanxung.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ad.panjiajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wp.yuexingan06.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://do.muxihuayi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jm.huixiangedu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qa.gzmigu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lc.yuntaijiaju.cn

[L06] 解析响应为 JSON
来源：http://yn.huixinmuqiang.cn

Py:   resp.json()
来源：http://au.521024.cn

PHP:  json_decode($body, true);
来源：http://bk.szxytkj.cn

JS:   await resp.json()
来源：http://yb.chemitech.net.cn

TS:   await resp.json()
来源：http://zd.jctech888.com.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nx.shtwfgs.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jg.chemitech.net.cn

Ruby: JSON.parse(resp.body)
来源：http://iw.9csxet.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ce.haigaiapp.cn

[L07] 处理 HTTP 状态码
来源：http://fg.huixiangedu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gc.huixinmuqiang.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lv.shtwfgs.cn

JS:   resp.ok;  resp.status
来源：http://yg.521024.cn

TS:   resp.ok;  resp.status
来源：http://zb.szxytkj.cn

Java: resp.statusCode()
来源：http://tf.huixinmuqiang.cn

Go:   resp.StatusCode
来源：http://te.bookmarksfly.cn

Ruby: resp.code.to_i
来源：http://wj.nicolike.cn

C#:   (int)resp.StatusCode
来源：http://ws.huixiangedu.cn

[L08] 并发请求多个地址
来源：http://lo.yuntaijiaju.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lb.szxytkj.cn

PHP:  curl_multi_init() 系列
来源：http://es.chemitech.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nr.panjiajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eg.nszjky.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://is.521024.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yx.hnjuh.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tj.hnjuh.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nc.hnjuh.cn

================================================================================
来源：http://ru.hnjuh.cn

M. 命令行 / 进程 / 环境
来源：http://pp.bjjhwx.cn

================================================================================
来源：http://to.bookmarksfly.cn

[M01] 读取命令行参数
来源：http://fe.shtwfgs.cn

Py:   sys.argv[1:]
来源：http://ws.bjjhwx.cn

PHP:  $argv;  $argc;
来源：http://kj.hahajie.cn

JS:   process.argv.slice(2)
来源：http://zh.nicolike.cn

TS:   process.argv.slice(2)
来源：http://bn.colortex.cn

Java: args 数组（main 方法参数）
来源：http://uf.hahajie.cn

Go:   os.Args[1:]
来源：http://ry.huixinmuqiang.cn

Ruby: ARGV
来源：http://vt.521024.cn

C#:   args 数组（Main 方法参数）
来源：http://dv.panjiajie.cn

[M02] 读取环境变量
来源：http://nh.yuexingan06.cn

Py:   os.environ.get("HOME")
来源：http://fo.jctech888.com.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ol.bjjhwx.cn

JS:   process.env.HOME
来源：http://re.chemitech.net.cn

TS:   process.env.HOME
来源：http://eu.szxytkj.cn

Java: System.getenv("HOME")
来源：http://gr.yuexingan06.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qm.bjjhwx.cn

Ruby: ENV["HOME"]
来源：http://tr.nszjky.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://um.hnjuh.cn

[M03] 执行外部命令
来源：http://tx.jctech888.com.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://la.nicolike.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ru.asd995.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ym.huixiangedu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ip.muxihuayi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hm.jianghongdianzi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://sd.nszjky.cn

Ruby: system("ls -l");  `ls -l`
来源：http://nd.colortex.cn

C#:   Process.Start("ls", "-l");
来源：http://qt.colortex.cn

[M04] 获取当前工作目录
来源：http://dn.521024.cn

Py:   os.getcwd()
来源：http://qg.bjjhwx.cn

PHP:  getcwd();
来源：http://fw.jctech888.com.cn

JS:   process.cwd()
来源：http://lp.huixinmuqiang.cn

TS:   process.cwd()
来源：http://xj.shxzukj.cn

Java: Path.of("").toAbsolutePath()
来源：http://uh.huanxung.cn

Go:   os.Getwd()
来源：http://mz.huixiangedu.cn

Ruby: Dir.pwd
来源：http://cb.newstarts.cn

C#:   Directory.GetCurrentDirectory()
来源：http://bv.hahajie.cn

[M05] 设置退出码
来源：http://gs.huixiangedu.cn

Py:   sys.exit(1)
来源：http://ba.shtwfgs.cn

PHP:  exit(1);
来源：http://bo.hnjuh.cn

JS:   process.exit(1)
来源：http://gr.shxzukj.cn

TS:   process.exit(1)
来源：http://bp.nicolike.cn

Java: System.exit(1)
来源：http://qo.shxzskj.cn

Go:   os.Exit(1)
来源：http://dz.bjjhwx.cn

Ruby: exit 1
来源：http://qg.huixinmuqiang.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sr.hnjuh.cn

[M06] 向标准错误输出
来源：http://hm.gzmigu.cn

Py:   print("err", file=sys.stderr)
来源：http://qq.bjjhwx.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://me.9csxet.cn

JS:   console.error("err")
来源：http://gl.gzmigu.cn

TS:   console.error("err")
来源：http://lq.jianghongdianzi.cn

Java: System.err.println("err")
来源：http://rj.shxzukj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pn.hnjuh.cn

Ruby: warn "err"
来源：http://zv.haigaiapp.cn

C#:   Console.Error.WriteLine("err")
来源：http://ej.huixiangedu.cn

[M07] 判断是否为主入口
来源：http://qe.lnxyls.cn

Py:   if __name__ == "__main__":
来源：http://lo.nicolike.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qr.huanxung.cn

JS:   require.main === module
来源：http://vl.bjjhwx.cn

TS:   require.main === module
来源：http://sl.yuntaijiaju.cn

Java: public static void main(String[] args)
来源：http://fa.9csxet.cn

Go:   func main()
来源：http://ez.jianghongdianzi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ko.jianghongdianzi.cn

C#:   static void Main(string[] args)
来源：http://ql.bookmarksfly.cn

[M08] 获取系统与运行时信息
来源：http://bt.huixinmuqiang.cn

Py:   platform.system();  platform.python_version()
来源：http://pm.chemitech.net.cn

PHP:  PHP_OS;  phpversion();
来源：http://ex.nicolike.cn

JS:   process.platform;  process.version
来源：http://ea.huanxung.cn

TS:   process.platform;  process.version
来源：http://zk.yuntaijiaju.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pc.szxytkj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ki.hahajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gu.asd995.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wj.huixinmuqiang.cn

================================================================================
来源：http://tg.chemitech.net.cn

N. 数据结构与算法
来源：http://pa.szxytkj.cn

================================================================================
来源：http://uf.521024.cn

[N01] 二分查找（有序数组）
来源：http://ow.nszjky.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wc.szsharing.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kk.nicolike.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tx.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ff.wgjwhj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jy.colortex.cn

Go:   sort.SearchInts(arr, x)
来源：http://wm.shtwfgs.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://rl.huanxung.cn

C#:   Array.BinarySearch(arr, x)
来源：http://bw.jctech888.com.cn

[N02] 排序（工程实践用内置实现）
来源：http://iv.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://qb.haigaiapp.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cc.nicolike.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://rd.jianghongdianzi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ib.shxzskj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vs.hnjuh.cn

Go:   slices.Sort(arr)
来源：http://qr.huixiangedu.cn


<!-- 参考信息 -->