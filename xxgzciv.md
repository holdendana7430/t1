代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jk.asd995.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lp.huixiangedu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pl.nicolike.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qt.hahajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ns.chemitech.net.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://oj.szxytkj.cn

[J05] 时间加减（加 7 天）
来源：http://uc.bjjhwx.cn

Py:   now + timedelta(days=7)
来源：http://kd.huanxung.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://dj.shxzskj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jj.yuntaijiaju.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zj.colortex.cn

Java: LocalDate.now().plusDays(7)
来源：http://mh.shxzukj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gd.haigaiapp.cn

Ruby: Time.now + 7 * 86400
来源：http://ay.huixiangedu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://eu.asd995.cn

[J06] 计算两时间之差
来源：http://wz.huixiangedu.cn

Py:   (end - start).total_seconds()
来源：http://xo.szsharing.cn

PHP:  $end->diff($start)->days;
来源：http://bc.9csxet.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pv.newstarts.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mz.nicolike.cn

Java: Duration.between(start, end).toSeconds()
来源：http://cn.panjiajie.cn

Go:   end.Sub(start).Hours()
来源：http://jo.gzmigu.cn

Ruby: end - start                 # 返回秒数
来源：http://rm.huanxung.cn

C#:   (end - start).TotalSeconds
来源：http://df.gzmigu.cn

[J07] 比较两个日期
来源：http://fe.haigaiapp.cn

Py:   d1 < d2;  d1 == d2
来源：http://mn.newstarts.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ti.shxzukj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ml.yuntaijiaju.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yh.nszjky.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ha.521024.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://op.muxihuayi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bw.panjiajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://vy.wgjwhj.cn

[J08] 提取年月日与星期
来源：http://ph.huanxung.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ai.haigaiapp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wr.muxihuayi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yp.wgjwhj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bt.muxihuayi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jz.9csxet.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ir.bjjhwx.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pd.huanxung.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yi.newstarts.cn

[J09] 时区处理
来源：http://yh.shxzskj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://im.yuntaijiaju.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yj.nszjky.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jl.huixiangedu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hn.asd995.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nj.shxzskj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kh.chemitech.net.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tb.jctech888.com.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vi.shtwfgs.cn

[J10] 取今天 / 本月第一天
来源：http://it.yuexingan06.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ww.szxytkj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://iw.521024.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dl.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cd.huanxung.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ma.shxzskj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ln.hnjuh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cc.nicolike.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hw.521024.cn

================================================================================
来源：http://wz.szsharing.cn

K. JSON 与序列化
来源：http://xz.9csxet.cn

================================================================================
来源：http://tb.yuexingan06.cn

[K01] 对象转 JSON 字符串
来源：http://cn.gzmigu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wu.bookmarksfly.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gv.panjiajie.cn

JS:   JSON.stringify(obj)
来源：http://vt.nszjky.cn

TS:   JSON.stringify(obj)
来源：http://cv.haigaiapp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qp.huixiangedu.cn

Go:   json.Marshal(obj)
来源：http://zo.gzmigu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://db.lnxyls.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fy.shxzskj.cn

[K02] JSON 字符串转对象
来源：http://ap.521024.cn

Py:   json.loads(s)
来源：http://ya.haigaiapp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hh.shxzskj.cn

JS:   JSON.parse(s)
来源：http://ep.wgjwhj.cn

TS:   JSON.parse(s)
来源：http://rn.colortex.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yd.nszjky.cn

Go:   json.Unmarshal(data, &v)
来源：http://ot.gzmigu.cn

Ruby: JSON.parse(s)
来源：http://ks.521024.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qq.shtwfgs.cn

[K03] JSON 美化输出（带缩进）
来源：http://uv.nszjky.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://se.bookmarksfly.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://if.bookmarksfly.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bp.shxzskj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://do.haigaiapp.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pe.9csxet.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fp.yuntaijiaju.cn

Ruby: JSON.pretty_generate(obj)
来源：http://cd.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vu.bjjhwx.cn

[K04] 读取 JSON 文件
来源：http://fg.huanxung.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pj.huanxung.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ca.9csxet.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rh.yuntaijiaju.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gw.muxihuayi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://oa.shxzukj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://in.panjiajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ay.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://eh.newstarts.cn

[K05] 深拷贝对象
来源：http://vm.szxytkj.cn

Py:   copy.deepcopy(obj)
来源：http://ya.newstarts.cn

PHP:  unserialize(serialize($obj));
来源：http://um.muxihuayi.cn

JS:   structuredClone(obj)
来源：http://pj.szxytkj.cn

TS:   structuredClone(obj)
来源：http://gq.bjjhwx.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fn.colortex.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gy.lnxyls.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bd.9csxet.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wu.yuntaijiaju.cn

[K06] 解析 URL 查询串
来源：http://kd.szsharing.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zx.haigaiapp.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wh.521024.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vm.shxzskj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uo.szsharing.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jj.szsharing.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://eu.shxzukj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yb.colortex.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://re.yuexingan06.cn

[K07] 进制转换
来源：http://ck.521024.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://as.panjiajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://iv.panjiajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lp.shxzskj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qi.huixiangedu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fw.asd995.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yr.huixiangedu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jm.lnxyls.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ql.bjjhwx.cn

[K08] 二进制序列化（非 JSON）
来源：http://uc.chemitech.net.cn

Py:   pickle.dumps(obj)
来源：http://ro.szxytkj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mq.colortex.cn

JS:   v8.serialize(obj)        // Node
来源：http://pd.szxytkj.cn

TS:   v8.serialize(obj)        // Node
来源：http://jh.shxzukj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://si.szsharing.cn

Go:   encoding/gob
来源：http://ip.colortex.cn

Ruby: Marshal.dump(obj)
来源：http://tt.shtwfgs.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bi.huanxung.cn

================================================================================
来源：http://sz.yuntaijiaju.cn

L. 网络请求
来源：http://zv.521024.cn

================================================================================
来源：http://mu.yuntaijiaju.cn

[L01] 发送 GET 请求
来源：http://bb.haigaiapp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sl.shxzskj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uy.chemitech.net.cn

JS:   await fetch(url)
来源：http://zc.yuntaijiaju.cn

TS:   await fetch(url)
来源：http://zj.nicolike.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mm.haigaiapp.cn

Go:   resp, err := http.Get(url)
来源：http://aj.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qc.bookmarksfly.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ax.yuexingan06.cn

[L02] 发送 POST JSON
来源：http://md.huanxung.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qv.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ly.nszjky.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wu.yuntaijiaju.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fg.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vs.nicolike.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ig.huanxung.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ug.shxzskj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://af.huanxung.cn

[L03] 设置自定义请求头
来源：http://nu.huixiangedu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ji.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qt.bookmarksfly.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bb.colortex.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ic.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wv.jctech888.com.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vv.szsharing.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wi.521024.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lm.yuntaijiaju.cn

[L04] 设置超时
来源：http://bj.nszjky.cn

Py:   requests.get(url, timeout=5)
来源：http://eg.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kx.yuexingan06.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pa.gzmigu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pl.haigaiapp.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hg.nicolike.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bx.muxihuayi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://oe.shxzskj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rq.szsharing.cn

[L05] 上传文件（multipart）
来源：http://hc.chemitech.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bf.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bx.huixiangedu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sm.muxihuayi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://il.muxihuayi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nr.szsharing.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://up.shtwfgs.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://do.nicolike.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ws.muxihuayi.cn

[L06] 解析响应为 JSON
来源：http://jf.huixinmuqiang.cn

Py:   resp.json()
来源：http://sc.bookmarksfly.cn

PHP:  json_decode($body, true);
来源：http://kl.huanxung.cn

JS:   await resp.json()
来源：http://dx.shtwfgs.cn

TS:   await resp.json()
来源：http://zx.9csxet.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://we.521024.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wh.newstarts.cn

Ruby: JSON.parse(resp.body)
来源：http://ur.jianghongdianzi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uj.521024.cn

[L07] 处理 HTTP 状态码
来源：http://vj.hnjuh.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wp.hnjuh.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yj.gzmigu.cn

JS:   resp.ok;  resp.status
来源：http://pr.9csxet.cn

TS:   resp.ok;  resp.status
来源：http://ka.muxihuayi.cn

Java: resp.statusCode()
来源：http://jh.lnxyls.cn

Go:   resp.StatusCode
来源：http://kd.lnxyls.cn

Ruby: resp.code.to_i
来源：http://zy.huixinmuqiang.cn

C#:   (int)resp.StatusCode
来源：http://ef.hnjuh.cn

[L08] 并发请求多个地址
来源：http://gd.bookmarksfly.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ju.shxzskj.cn

PHP:  curl_multi_init() 系列
来源：http://py.jianghongdianzi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hu.huixiangedu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cj.gzmigu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://to.shxzukj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yz.hnjuh.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ue.colortex.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ow.newstarts.cn

================================================================================
来源：http://qr.gzmigu.cn

M. 命令行 / 进程 / 环境
来源：http://hr.huanxung.cn

================================================================================
来源：http://hy.wgjwhj.cn

[M01] 读取命令行参数
来源：http://dz.shxzskj.cn

Py:   sys.argv[1:]
来源：http://up.jianghongdianzi.cn

PHP:  $argv;  $argc;
来源：http://tx.yuexingan06.cn

JS:   process.argv.slice(2)
来源：http://bx.shxzskj.cn

TS:   process.argv.slice(2)
来源：http://ke.bjjhwx.cn

Java: args 数组（main 方法参数）
来源：http://ki.newstarts.cn

Go:   os.Args[1:]
来源：http://fy.521024.cn

Ruby: ARGV
来源：http://qm.szsharing.cn

C#:   args 数组（Main 方法参数）
来源：http://nx.bookmarksfly.cn

[M02] 读取环境变量
来源：http://fl.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://sy.nszjky.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rd.9csxet.cn

JS:   process.env.HOME
来源：http://vl.newstarts.cn

TS:   process.env.HOME
来源：http://yo.panjiajie.cn

Java: System.getenv("HOME")
来源：http://la.521024.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kn.gzmigu.cn

Ruby: ENV["HOME"]
来源：http://gi.lnxyls.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://km.colortex.cn

[M03] 执行外部命令
来源：http://je.chemitech.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jn.asd995.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rm.szsharing.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://px.yuexingan06.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mz.gzmigu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ns.bookmarksfly.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vn.yuntaijiaju.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kh.panjiajie.cn

C#:   Process.Start("ls", "-l");
来源：http://xm.yuexingan06.cn

[M04] 获取当前工作目录
来源：http://xe.szxytkj.cn

Py:   os.getcwd()
来源：http://qr.gzmigu.cn

PHP:  getcwd();
来源：http://st.shxzukj.cn

JS:   process.cwd()
来源：http://hs.nicolike.cn

TS:   process.cwd()
来源：http://nm.muxihuayi.cn

Java: Path.of("").toAbsolutePath()
来源：http://ou.szxytkj.cn

Go:   os.Getwd()
来源：http://wm.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://vi.muxihuayi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rd.hahajie.cn

[M05] 设置退出码
来源：http://sc.asd995.cn

Py:   sys.exit(1)
来源：http://jb.bjjhwx.cn

PHP:  exit(1);
来源：http://td.9csxet.cn

JS:   process.exit(1)
来源：http://yq.lnxyls.cn

TS:   process.exit(1)
来源：http://du.yuntaijiaju.cn

Java: System.exit(1)
来源：http://sv.lnxyls.cn

Go:   os.Exit(1)
来源：http://nx.panjiajie.cn

Ruby: exit 1
来源：http://gs.szsharing.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pj.huixiangedu.cn

[M06] 向标准错误输出
来源：http://ek.nszjky.cn

Py:   print("err", file=sys.stderr)
来源：http://hz.nszjky.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://mp.panjiajie.cn

JS:   console.error("err")
来源：http://ch.jctech888.com.cn

TS:   console.error("err")
来源：http://qq.muxihuayi.cn

Java: System.err.println("err")
来源：http://lb.shxzskj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qq.nicolike.cn

Ruby: warn "err"
来源：http://dz.yuexingan06.cn

C#:   Console.Error.WriteLine("err")
来源：http://ux.shxzukj.cn

[M07] 判断是否为主入口
来源：http://xd.shtwfgs.cn

Py:   if __name__ == "__main__":
来源：http://rf.chemitech.net.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ib.huixinmuqiang.cn

JS:   require.main === module
来源：http://te.szxytkj.cn

TS:   require.main === module
来源：http://rv.szsharing.cn

Java: public static void main(String[] args)
来源：http://gx.9csxet.cn

Go:   func main()
来源：http://sl.wgjwhj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://et.colortex.cn

C#:   static void Main(string[] args)
来源：http://ic.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://xj.yuexingan06.cn

Py:   platform.system();  platform.python_version()
来源：http://qe.jianghongdianzi.cn

PHP:  PHP_OS;  phpversion();
来源：http://rm.yuexingan06.cn

JS:   process.platform;  process.version
来源：http://ja.gzmigu.cn

TS:   process.platform;  process.version
来源：http://kd.9csxet.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nv.jctech888.com.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gp.huixinmuqiang.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://po.shxzukj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qd.huixinmuqiang.cn

================================================================================
来源：http://jf.yuexingan06.cn

N. 数据结构与算法
来源：http://jc.muxihuayi.cn

================================================================================
来源：http://mb.panjiajie.cn

[N01] 二分查找（有序数组）
来源：http://cz.muxihuayi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://do.shtwfgs.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dj.521024.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qy.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://du.bjjhwx.cn

Java: Arrays.binarySearch(arr, x)
来源：http://dc.huanxung.cn

Go:   sort.SearchInts(arr, x)
来源：http://zk.muxihuayi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://js.hahajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://sz.szxytkj.cn

[N02] 排序（工程实践用内置实现）
来源：http://cz.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://sf.bookmarksfly.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://en.szxytkj.cn


<!-- 参考信息 -->