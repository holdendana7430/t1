代发 wailian999

Py:   (end - start).total_seconds()
来源：http://vw.huanxung.cn

PHP:  $end->diff($start)->days;
来源：http://tt.nszjky.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://km.bjjhwx.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cv.9csxet.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vp.9csxet.cn

Go:   end.Sub(start).Hours()
来源：http://xt.shxzukj.cn

Ruby: end - start                 # 返回秒数
来源：http://cm.huanxung.cn

C#:   (end - start).TotalSeconds
来源：http://xp.haigaiapp.cn

[J07] 比较两个日期
来源：http://ky.hahajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://jy.9csxet.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yw.huixinmuqiang.cn

JS:   d1.getTime() < d2.getTime()
来源：http://cr.9csxet.cn

TS:   d1.getTime() < d2.getTime()
来源：http://cf.szsharing.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ul.bjjhwx.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nx.gzmigu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ql.chemitech.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://wq.haigaiapp.cn

[J08] 提取年月日与星期
来源：http://qy.shtwfgs.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qd.huanxung.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sb.huixinmuqiang.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ct.chemitech.net.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://en.gzmigu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qu.gzmigu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xb.asd995.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pf.muxihuayi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lu.huanxung.cn

[J09] 时区处理
来源：http://qb.muxihuayi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nx.bjjhwx.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yy.haigaiapp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kj.haigaiapp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fh.shtwfgs.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pb.shxzskj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dz.jctech888.com.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://aw.nicolike.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ft.szxytkj.cn

[J10] 取今天 / 本月第一天
来源：http://ls.bjjhwx.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fi.bookmarksfly.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ki.yuexingan06.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dt.jianghongdianzi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ky.colortex.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ds.shtwfgs.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ka.yuntaijiaju.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kk.huixiangedu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cp.newstarts.cn

================================================================================
来源：http://px.hahajie.cn

K. JSON 与序列化
来源：http://ye.bookmarksfly.cn

================================================================================
来源：http://pm.muxihuayi.cn

[K01] 对象转 JSON 字符串
来源：http://jz.yuntaijiaju.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ib.9csxet.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kn.hnjuh.cn

JS:   JSON.stringify(obj)
来源：http://hu.jctech888.com.cn

TS:   JSON.stringify(obj)
来源：http://ko.huixinmuqiang.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fq.shxzukj.cn

Go:   json.Marshal(obj)
来源：http://tj.hahajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hl.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pk.hnjuh.cn

[K02] JSON 字符串转对象
来源：http://ef.9csxet.cn

Py:   json.loads(s)
来源：http://qd.521024.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://aq.haigaiapp.cn

JS:   JSON.parse(s)
来源：http://qm.haigaiapp.cn

TS:   JSON.parse(s)
来源：http://al.bjjhwx.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qf.nszjky.cn

Go:   json.Unmarshal(data, &v)
来源：http://ys.bjjhwx.cn

Ruby: JSON.parse(s)
来源：http://lg.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jx.wgjwhj.cn

[K03] JSON 美化输出（带缩进）
来源：http://gu.muxihuayi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ia.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nt.yuntaijiaju.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xs.yuntaijiaju.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qk.9csxet.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hi.9csxet.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nt.haigaiapp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://lp.521024.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kh.yuexingan06.cn

[K04] 读取 JSON 文件
来源：http://gl.szxytkj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pp.nszjky.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ys.huanxung.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xj.shtwfgs.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://el.yuexingan06.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dg.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vk.lnxyls.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://sv.colortex.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ry.jianghongdianzi.cn

[K05] 深拷贝对象
来源：http://de.panjiajie.cn

Py:   copy.deepcopy(obj)
来源：http://we.521024.cn

PHP:  unserialize(serialize($obj));
来源：http://nw.shxzskj.cn

JS:   structuredClone(obj)
来源：http://eu.gzmigu.cn

TS:   structuredClone(obj)
来源：http://ac.jianghongdianzi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ss.haigaiapp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zo.yuntaijiaju.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://du.huixinmuqiang.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://at.colortex.cn

[K06] 解析 URL 查询串
来源：http://sv.jianghongdianzi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bs.shtwfgs.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ya.colortex.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gm.nszjky.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zi.panjiajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pk.nicolike.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mw.newstarts.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pt.huixinmuqiang.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dn.colortex.cn

[K07] 进制转换
来源：http://pu.bookmarksfly.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rz.yuexingan06.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yb.chemitech.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rn.haigaiapp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fw.muxihuayi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://di.hahajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wg.hnjuh.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yl.lnxyls.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dz.muxihuayi.cn

[K08] 二进制序列化（非 JSON）
来源：http://qq.lnxyls.cn

Py:   pickle.dumps(obj)
来源：http://ee.shxzskj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pf.gzmigu.cn

JS:   v8.serialize(obj)        // Node
来源：http://dk.chemitech.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://bx.wgjwhj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://od.gzmigu.cn

Go:   encoding/gob
来源：http://mq.muxihuayi.cn

Ruby: Marshal.dump(obj)
来源：http://be.chemitech.net.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lu.lnxyls.cn

================================================================================
来源：http://hr.lnxyls.cn

L. 网络请求
来源：http://ft.lnxyls.cn

================================================================================
来源：http://ks.asd995.cn

[L01] 发送 GET 请求
来源：http://na.szsharing.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rt.chemitech.net.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yt.szsharing.cn

JS:   await fetch(url)
来源：http://nb.colortex.cn

TS:   await fetch(url)
来源：http://zo.shxzukj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yf.colortex.cn

Go:   resp, err := http.Get(url)
来源：http://oc.nicolike.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://mr.gzmigu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kh.nszjky.cn

[L02] 发送 POST JSON
来源：http://ss.muxihuayi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nd.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uo.szsharing.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tp.yuntaijiaju.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qy.asd995.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sr.jctech888.com.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kz.haigaiapp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ar.szxytkj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ck.jianghongdianzi.cn

[L03] 设置自定义请求头
来源：http://jt.gzmigu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://os.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cw.huixiangedu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fl.huanxung.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mv.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ou.jctech888.com.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ao.bookmarksfly.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lo.shxzskj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ah.huanxung.cn

[L04] 设置超时
来源：http://mu.panjiajie.cn

Py:   requests.get(url, timeout=5)
来源：http://zb.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yn.jianghongdianzi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fz.hahajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://px.bookmarksfly.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yd.colortex.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wv.yuexingan06.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lj.hahajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jf.colortex.cn

[L05] 上传文件（multipart）
来源：http://hu.bjjhwx.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ow.panjiajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://up.jctech888.com.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wq.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jn.lnxyls.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qr.haigaiapp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gh.huanxung.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dj.huanxung.cn

[L06] 解析响应为 JSON
来源：http://ql.huixinmuqiang.cn

Py:   resp.json()
来源：http://ma.asd995.cn

PHP:  json_decode($body, true);
来源：http://mv.huixinmuqiang.cn

JS:   await resp.json()
来源：http://vt.yuexingan06.cn

TS:   await resp.json()
来源：http://nt.panjiajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rm.colortex.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nu.jianghongdianzi.cn

Ruby: JSON.parse(resp.body)
来源：http://xy.9csxet.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sx.yuntaijiaju.cn

[L07] 处理 HTTP 状态码
来源：http://lp.muxihuayi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://de.bookmarksfly.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bv.nicolike.cn

JS:   resp.ok;  resp.status
来源：http://fj.huixiangedu.cn

TS:   resp.ok;  resp.status
来源：http://mi.hnjuh.cn

Java: resp.statusCode()
来源：http://ad.bookmarksfly.cn

Go:   resp.StatusCode
来源：http://pb.huanxung.cn

Ruby: resp.code.to_i
来源：http://if.szsharing.cn

C#:   (int)resp.StatusCode
来源：http://wa.bookmarksfly.cn

[L08] 并发请求多个地址
来源：http://ll.huixinmuqiang.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rm.hnjuh.cn

PHP:  curl_multi_init() 系列
来源：http://vd.shxzskj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xn.hahajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ts.huanxung.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://in.yuntaijiaju.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://et.lnxyls.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://az.shxzukj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://iw.chemitech.net.cn

================================================================================
来源：http://mx.huanxung.cn

M. 命令行 / 进程 / 环境
来源：http://vb.newstarts.cn

================================================================================
来源：http://mc.huixiangedu.cn

[M01] 读取命令行参数
来源：http://ss.bjjhwx.cn

Py:   sys.argv[1:]
来源：http://hi.shtwfgs.cn

PHP:  $argv;  $argc;
来源：http://tp.nszjky.cn

JS:   process.argv.slice(2)
来源：http://wg.haigaiapp.cn

TS:   process.argv.slice(2)
来源：http://oe.9csxet.cn

Java: args 数组（main 方法参数）
来源：http://wy.shxzukj.cn

Go:   os.Args[1:]
来源：http://ho.lnxyls.cn

Ruby: ARGV
来源：http://vm.muxihuayi.cn

C#:   args 数组（Main 方法参数）
来源：http://kk.nszjky.cn

[M02] 读取环境变量
来源：http://bp.yuntaijiaju.cn

Py:   os.environ.get("HOME")
来源：http://ll.panjiajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://az.shxzukj.cn

JS:   process.env.HOME
来源：http://dn.hnjuh.cn

TS:   process.env.HOME
来源：http://dk.asd995.cn

Java: System.getenv("HOME")
来源：http://rq.shxzskj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yj.wgjwhj.cn

Ruby: ENV["HOME"]
来源：http://gt.asd995.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cm.newstarts.cn

[M03] 执行外部命令
来源：http://pb.shxzskj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qd.yuntaijiaju.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jg.nszjky.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://th.huixinmuqiang.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fb.nszjky.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wr.jianghongdianzi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://da.521024.cn

Ruby: system("ls -l");  `ls -l`
来源：http://cs.shxzskj.cn

C#:   Process.Start("ls", "-l");
来源：http://wv.521024.cn

[M04] 获取当前工作目录
来源：http://zu.9csxet.cn

Py:   os.getcwd()
来源：http://ex.huanxung.cn

PHP:  getcwd();
来源：http://tc.huixiangedu.cn

JS:   process.cwd()
来源：http://ww.chemitech.net.cn

TS:   process.cwd()
来源：http://es.nicolike.cn

Java: Path.of("").toAbsolutePath()
来源：http://sq.shtwfgs.cn

Go:   os.Getwd()
来源：http://ez.wgjwhj.cn

Ruby: Dir.pwd
来源：http://dq.hahajie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jd.yuexingan06.cn

[M05] 设置退出码
来源：http://lu.chemitech.net.cn

Py:   sys.exit(1)
来源：http://cq.colortex.cn

PHP:  exit(1);
来源：http://gn.szxytkj.cn

JS:   process.exit(1)
来源：http://he.huanxung.cn

TS:   process.exit(1)
来源：http://qf.bjjhwx.cn

Java: System.exit(1)
来源：http://mm.wgjwhj.cn

Go:   os.Exit(1)
来源：http://ct.9csxet.cn

Ruby: exit 1
来源：http://rg.huixiangedu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qb.lnxyls.cn

[M06] 向标准错误输出
来源：http://on.colortex.cn

Py:   print("err", file=sys.stderr)
来源：http://aj.hnjuh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vt.muxihuayi.cn

JS:   console.error("err")
来源：http://dp.newstarts.cn

TS:   console.error("err")
来源：http://xr.nicolike.cn

Java: System.err.println("err")
来源：http://ng.hahajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://uk.huanxung.cn

Ruby: warn "err"
来源：http://wd.521024.cn

C#:   Console.Error.WriteLine("err")
来源：http://kr.shxzukj.cn

[M07] 判断是否为主入口
来源：http://nn.chemitech.net.cn

Py:   if __name__ == "__main__":
来源：http://ry.yuexingan06.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rv.shtwfgs.cn

JS:   require.main === module
来源：http://dz.bjjhwx.cn

TS:   require.main === module
来源：http://dr.asd995.cn

Java: public static void main(String[] args)
来源：http://ts.huixinmuqiang.cn

Go:   func main()
来源：http://fj.nicolike.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://im.wgjwhj.cn

C#:   static void Main(string[] args)
来源：http://bx.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://ew.haigaiapp.cn

Py:   platform.system();  platform.python_version()
来源：http://be.hahajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://mf.haigaiapp.cn

JS:   process.platform;  process.version
来源：http://mn.shxzskj.cn

TS:   process.platform;  process.version
来源：http://it.wgjwhj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lp.bjjhwx.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xo.muxihuayi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zy.chemitech.net.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ha.hnjuh.cn

================================================================================
来源：http://od.bookmarksfly.cn

N. 数据结构与算法
来源：http://en.lnxyls.cn

================================================================================
来源：http://sa.hahajie.cn

[N01] 二分查找（有序数组）
来源：http://en.shxzskj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://nw.panjiajie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dw.shxzskj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://st.521024.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ut.shtwfgs.cn

Java: Arrays.binarySearch(arr, x)
来源：http://le.jianghongdianzi.cn

Go:   sort.SearchInts(arr, x)
来源：http://py.shxzukj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ly.bookmarksfly.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wb.muxihuayi.cn

[N02] 排序（工程实践用内置实现）
来源：http://fv.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://qs.newstarts.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fg.chemitech.net.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://lo.bjjhwx.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://nh.muxihuayi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ch.521024.cn

Go:   slices.Sort(arr)
来源：http://vm.chemitech.net.cn

Ruby: arr.sort
来源：http://ij.nicolike.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://me.huixiangedu.cn

[N03] 快速排序（分治示例）
来源：http://gj.asd995.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fs.9csxet.cn

PHP:  // 递归实现，或用 usort
来源：http://nb.bookmarksfly.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://og.colortex.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rv.bjjhwx.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://je.haigaiapp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ls.panjiajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rd.huixiangedu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vd.yuntaijiaju.cn

[N04] 斐波那契数列
来源：http://hc.shxzskj.cn


<!-- 参考信息 -->