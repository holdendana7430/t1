代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://tt.haigaiapp.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cr.hahajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ep.szxytkj.cn

Java: LocalDate.now().plusDays(7)
来源：http://ry.jianghongdianzi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sc.jctech888.com.cn

Ruby: Time.now + 7 * 86400
来源：http://ie.wgjwhj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://fs.huanxung.cn

[J06] 计算两时间之差
来源：http://cj.chemitech.net.cn

Py:   (end - start).total_seconds()
来源：http://oo.chemitech.net.cn

PHP:  $end->diff($start)->days;
来源：http://qs.9csxet.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jn.shxzskj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jc.huanxung.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ue.shtwfgs.cn

Go:   end.Sub(start).Hours()
来源：http://qv.hahajie.cn

Ruby: end - start                 # 返回秒数
来源：http://lx.chemitech.net.cn

C#:   (end - start).TotalSeconds
来源：http://lc.shtwfgs.cn

[J07] 比较两个日期
来源：http://rq.huixiangedu.cn

Py:   d1 < d2;  d1 == d2
来源：http://mp.yuntaijiaju.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vn.shtwfgs.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gk.newstarts.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rt.jctech888.com.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ww.bookmarksfly.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xp.hnjuh.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vx.szsharing.cn

C#:   d1 < d2;  d1 == d2
来源：http://sd.521024.cn

[J08] 提取年月日与星期
来源：http://ki.jianghongdianzi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fo.hahajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fb.huixiangedu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pt.shxzskj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zm.wgjwhj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xh.haigaiapp.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mb.chemitech.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hs.chemitech.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bn.nicolike.cn

[J09] 时区处理
来源：http://ty.gzmigu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wp.9csxet.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yp.9csxet.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dh.gzmigu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hl.hahajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qg.jctech888.com.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tv.521024.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ls.szxytkj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://oa.chemitech.net.cn

[J10] 取今天 / 本月第一天
来源：http://st.lnxyls.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xn.wgjwhj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gu.muxihuayi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nj.lnxyls.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nk.haigaiapp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ba.szxytkj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://oj.bookmarksfly.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pv.gzmigu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lg.panjiajie.cn

================================================================================
来源：http://hi.haigaiapp.cn

K. JSON 与序列化
来源：http://qx.yuntaijiaju.cn

================================================================================
来源：http://br.521024.cn

[K01] 对象转 JSON 字符串
来源：http://yl.bjjhwx.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zd.shxzskj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nt.jctech888.com.cn

JS:   JSON.stringify(obj)
来源：http://sp.gzmigu.cn

TS:   JSON.stringify(obj)
来源：http://ew.shtwfgs.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qx.yuntaijiaju.cn

Go:   json.Marshal(obj)
来源：http://uf.colortex.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qk.nicolike.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://td.shxzskj.cn

[K02] JSON 字符串转对象
来源：http://ky.yuntaijiaju.cn

Py:   json.loads(s)
来源：http://xq.bookmarksfly.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wn.panjiajie.cn

JS:   JSON.parse(s)
来源：http://ho.colortex.cn

TS:   JSON.parse(s)
来源：http://fs.521024.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gz.bookmarksfly.cn

Go:   json.Unmarshal(data, &v)
来源：http://fd.haigaiapp.cn

Ruby: JSON.parse(s)
来源：http://nf.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bj.huixiangedu.cn

[K03] JSON 美化输出（带缩进）
来源：http://jb.521024.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zy.wgjwhj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ar.szsharing.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ox.asd995.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nn.haigaiapp.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tv.hnjuh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tn.colortex.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ev.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://oc.shxzukj.cn

[K04] 读取 JSON 文件
来源：http://jm.haigaiapp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xq.hahajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qh.wgjwhj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dw.yuntaijiaju.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jq.haigaiapp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hj.newstarts.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qb.panjiajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wc.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vg.bookmarksfly.cn

[K05] 深拷贝对象
来源：http://oc.haigaiapp.cn

Py:   copy.deepcopy(obj)
来源：http://qi.shxzskj.cn

PHP:  unserialize(serialize($obj));
来源：http://rb.colortex.cn

JS:   structuredClone(obj)
来源：http://ub.yuntaijiaju.cn

TS:   structuredClone(obj)
来源：http://qc.521024.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ml.muxihuayi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yg.hnjuh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ml.panjiajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mv.szsharing.cn

[K06] 解析 URL 查询串
来源：http://ss.lnxyls.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zj.nszjky.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zx.bjjhwx.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sz.jianghongdianzi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gs.gzmigu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tw.bookmarksfly.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fa.jctech888.com.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ra.shxzskj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mn.asd995.cn

[K07] 进制转换
来源：http://ts.hnjuh.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://oj.bookmarksfly.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lq.asd995.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ks.huanxung.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hq.wgjwhj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://oi.huixiangedu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://il.yuexingan06.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ed.nszjky.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cu.szsharing.cn

[K08] 二进制序列化（非 JSON）
来源：http://tf.jianghongdianzi.cn

Py:   pickle.dumps(obj)
来源：http://ep.szsharing.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bl.jianghongdianzi.cn

JS:   v8.serialize(obj)        // Node
来源：http://kw.hnjuh.cn

TS:   v8.serialize(obj)        // Node
来源：http://tx.gzmigu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xw.yuntaijiaju.cn

Go:   encoding/gob
来源：http://df.colortex.cn

Ruby: Marshal.dump(obj)
来源：http://gc.hahajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pa.nszjky.cn

================================================================================
来源：http://on.bjjhwx.cn

L. 网络请求
来源：http://py.bookmarksfly.cn

================================================================================
来源：http://kv.szsharing.cn

[L01] 发送 GET 请求
来源：http://oh.huixiangedu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gl.521024.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cq.yuexingan06.cn

JS:   await fetch(url)
来源：http://zc.bookmarksfly.cn

TS:   await fetch(url)
来源：http://jd.yuntaijiaju.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cp.huixiangedu.cn

Go:   resp, err := http.Get(url)
来源：http://xo.gzmigu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pn.chemitech.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ph.shxzukj.cn

[L02] 发送 POST JSON
来源：http://fe.huixinmuqiang.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ri.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bc.hahajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lq.gzmigu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fg.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ve.shxzskj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hg.521024.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ft.hnjuh.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sp.521024.cn

[L03] 设置自定义请求头
来源：http://ga.haigaiapp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qp.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nd.nszjky.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cj.panjiajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wg.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ik.nszjky.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fq.huixiangedu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zd.muxihuayi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ox.bjjhwx.cn

[L04] 设置超时
来源：http://vd.huixinmuqiang.cn

Py:   requests.get(url, timeout=5)
来源：http://xt.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mx.nicolike.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rg.shxzukj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ad.chemitech.net.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cx.jctech888.com.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ro.huanxung.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ek.muxihuayi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://su.shtwfgs.cn

[L05] 上传文件（multipart）
来源：http://tu.chemitech.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uc.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ak.szsharing.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pm.jctech888.com.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rs.521024.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://he.yuexingan06.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xl.lnxyls.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ci.hahajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mp.shxzukj.cn

[L06] 解析响应为 JSON
来源：http://wu.huanxung.cn

Py:   resp.json()
来源：http://uz.haigaiapp.cn

PHP:  json_decode($body, true);
来源：http://tc.panjiajie.cn

JS:   await resp.json()
来源：http://qf.huixiangedu.cn

TS:   await resp.json()
来源：http://sv.bjjhwx.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zr.521024.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fj.gzmigu.cn

Ruby: JSON.parse(resp.body)
来源：http://ta.bookmarksfly.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cb.521024.cn

[L07] 处理 HTTP 状态码
来源：http://vf.panjiajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qw.hnjuh.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nu.chemitech.net.cn

JS:   resp.ok;  resp.status
来源：http://bw.szxytkj.cn

TS:   resp.ok;  resp.status
来源：http://iz.shxzukj.cn

Java: resp.statusCode()
来源：http://bf.gzmigu.cn

Go:   resp.StatusCode
来源：http://ng.szxytkj.cn

Ruby: resp.code.to_i
来源：http://lc.wgjwhj.cn

C#:   (int)resp.StatusCode
来源：http://ul.nicolike.cn

[L08] 并发请求多个地址
来源：http://ma.nicolike.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ni.yuexingan06.cn

PHP:  curl_multi_init() 系列
来源：http://ax.hnjuh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://io.nicolike.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vw.yuntaijiaju.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ga.shtwfgs.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sg.muxihuayi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zm.colortex.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pq.521024.cn

================================================================================
来源：http://to.lnxyls.cn

M. 命令行 / 进程 / 环境
来源：http://xi.panjiajie.cn

================================================================================
来源：http://kh.jctech888.com.cn

[M01] 读取命令行参数
来源：http://zs.huixiangedu.cn

Py:   sys.argv[1:]
来源：http://it.nicolike.cn

PHP:  $argv;  $argc;
来源：http://if.haigaiapp.cn

JS:   process.argv.slice(2)
来源：http://cq.yuexingan06.cn

TS:   process.argv.slice(2)
来源：http://zy.huixinmuqiang.cn

Java: args 数组（main 方法参数）
来源：http://pa.521024.cn

Go:   os.Args[1:]
来源：http://mp.jctech888.com.cn

Ruby: ARGV
来源：http://nr.shtwfgs.cn

C#:   args 数组（Main 方法参数）
来源：http://jv.yuntaijiaju.cn

[M02] 读取环境变量
来源：http://tb.yuexingan06.cn

Py:   os.environ.get("HOME")
来源：http://ly.wgjwhj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xe.9csxet.cn

JS:   process.env.HOME
来源：http://gw.yuexingan06.cn

TS:   process.env.HOME
来源：http://xl.szsharing.cn

Java: System.getenv("HOME")
来源：http://js.hnjuh.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qo.nicolike.cn

Ruby: ENV["HOME"]
来源：http://zh.yuntaijiaju.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zb.yuexingan06.cn

[M03] 执行外部命令
来源：http://bj.bjjhwx.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cg.gzmigu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rv.wgjwhj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://bd.yuexingan06.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yu.jctech888.com.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yi.jianghongdianzi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ic.hahajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tl.nszjky.cn

C#:   Process.Start("ls", "-l");
来源：http://df.yuexingan06.cn

[M04] 获取当前工作目录
来源：http://ul.nszjky.cn

Py:   os.getcwd()
来源：http://wh.colortex.cn

PHP:  getcwd();
来源：http://vv.huixiangedu.cn

JS:   process.cwd()
来源：http://cz.nszjky.cn

TS:   process.cwd()
来源：http://hi.lnxyls.cn

Java: Path.of("").toAbsolutePath()
来源：http://dv.huixinmuqiang.cn

Go:   os.Getwd()
来源：http://ms.lnxyls.cn

Ruby: Dir.pwd
来源：http://sq.szxytkj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://oc.colortex.cn

[M05] 设置退出码
来源：http://zs.haigaiapp.cn

Py:   sys.exit(1)
来源：http://tr.nicolike.cn

PHP:  exit(1);
来源：http://xp.yuexingan06.cn

JS:   process.exit(1)
来源：http://ri.chemitech.net.cn

TS:   process.exit(1)
来源：http://xl.shxzukj.cn

Java: System.exit(1)
来源：http://yn.bookmarksfly.cn

Go:   os.Exit(1)
来源：http://ib.bookmarksfly.cn

Ruby: exit 1
来源：http://pt.muxihuayi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ya.bjjhwx.cn

[M06] 向标准错误输出
来源：http://tm.huanxung.cn

Py:   print("err", file=sys.stderr)
来源：http://uv.wgjwhj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://fl.newstarts.cn

JS:   console.error("err")
来源：http://pp.haigaiapp.cn

TS:   console.error("err")
来源：http://ht.haigaiapp.cn

Java: System.err.println("err")
来源：http://uv.huixinmuqiang.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lt.huixiangedu.cn

Ruby: warn "err"
来源：http://gx.wgjwhj.cn

C#:   Console.Error.WriteLine("err")
来源：http://zh.shtwfgs.cn

[M07] 判断是否为主入口
来源：http://fn.yuntaijiaju.cn

Py:   if __name__ == "__main__":
来源：http://oq.colortex.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kh.chemitech.net.cn

JS:   require.main === module
来源：http://tw.shxzskj.cn

TS:   require.main === module
来源：http://aj.521024.cn

Java: public static void main(String[] args)
来源：http://tf.bookmarksfly.cn

Go:   func main()
来源：http://my.jianghongdianzi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fp.szsharing.cn

C#:   static void Main(string[] args)
来源：http://vm.shxzskj.cn

[M08] 获取系统与运行时信息
来源：http://jm.chemitech.net.cn

Py:   platform.system();  platform.python_version()
来源：http://ah.colortex.cn

PHP:  PHP_OS;  phpversion();
来源：http://cp.szxytkj.cn

JS:   process.platform;  process.version
来源：http://fm.yuntaijiaju.cn

TS:   process.platform;  process.version
来源：http://cm.muxihuayi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tx.colortex.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://tw.gzmigu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bz.yuexingan06.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dv.shxzukj.cn

================================================================================
来源：http://sd.jctech888.com.cn

N. 数据结构与算法
来源：http://wv.jctech888.com.cn

================================================================================
来源：http://ec.colortex.cn

[N01] 二分查找（有序数组）
来源：http://jc.shtwfgs.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ex.lnxyls.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wc.huanxung.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ob.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ca.nszjky.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ur.szsharing.cn

Go:   sort.SearchInts(arr, x)
来源：http://xq.huixinmuqiang.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ec.jianghongdianzi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jz.haigaiapp.cn

[N02] 排序（工程实践用内置实现）
来源：http://lk.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://ia.nicolike.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nj.lnxyls.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://le.shxzskj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://eo.shtwfgs.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lq.muxihuayi.cn

Go:   slices.Sort(arr)
来源：http://wb.nicolike.cn

Ruby: arr.sort
来源：http://vu.shxzskj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gb.lnxyls.cn

[N03] 快速排序（分治示例）
来源：http://cy.szsharing.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sa.9csxet.cn


<!-- 参考信息 -->