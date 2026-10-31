代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zv.szsharing.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ub.shtwfgs.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lj.hnjuh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://se.shtwfgs.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uj.chemitech.net.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ss.huixinmuqiang.cn

[J05] 时间加减（加 7 天）
来源：http://jd.newstarts.cn

Py:   now + timedelta(days=7)
来源：http://pe.bookmarksfly.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wm.yuntaijiaju.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rp.panjiajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://za.szxytkj.cn

Java: LocalDate.now().plusDays(7)
来源：http://xs.panjiajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qa.newstarts.cn

Ruby: Time.now + 7 * 86400
来源：http://hy.haigaiapp.cn

C#:   DateTime.Now.AddDays(7)
来源：http://be.gzmigu.cn

[J06] 计算两时间之差
来源：http://qr.gzmigu.cn

Py:   (end - start).total_seconds()
来源：http://cl.muxihuayi.cn

PHP:  $end->diff($start)->days;
来源：http://ln.huixiangedu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qi.huixinmuqiang.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://st.huixinmuqiang.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dq.chemitech.net.cn

Go:   end.Sub(start).Hours()
来源：http://nr.jctech888.com.cn

Ruby: end - start                 # 返回秒数
来源：http://am.szsharing.cn

C#:   (end - start).TotalSeconds
来源：http://ln.szsharing.cn

[J07] 比较两个日期
来源：http://bj.hahajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://jy.hahajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tl.nicolike.cn

JS:   d1.getTime() < d2.getTime()
来源：http://cr.yuexingan06.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ev.jctech888.com.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wm.hnjuh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://oa.asd995.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fw.jianghongdianzi.cn

C#:   d1 < d2;  d1 == d2
来源：http://hu.9csxet.cn

[J08] 提取年月日与星期
来源：http://wv.shxzskj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tr.wgjwhj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nv.hnjuh.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xe.asd995.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ov.9csxet.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ef.jianghongdianzi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sd.huanxung.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ba.yuexingan06.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://da.haigaiapp.cn

[J09] 时区处理
来源：http://sd.shxzskj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jy.muxihuayi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ph.nicolike.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dz.521024.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kr.yuexingan06.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kq.jctech888.com.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qp.huanxung.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://os.newstarts.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sk.haigaiapp.cn

[J10] 取今天 / 本月第一天
来源：http://dh.huixinmuqiang.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ul.521024.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bi.jianghongdianzi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ko.nszjky.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://go.hnjuh.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vc.yuexingan06.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bn.521024.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wn.asd995.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ys.szsharing.cn

================================================================================
来源：http://uh.lnxyls.cn

K. JSON 与序列化
来源：http://tt.asd995.cn

================================================================================
来源：http://yi.colortex.cn

[K01] 对象转 JSON 字符串
来源：http://zr.9csxet.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vr.gzmigu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zm.bookmarksfly.cn

JS:   JSON.stringify(obj)
来源：http://dc.asd995.cn

TS:   JSON.stringify(obj)
来源：http://lc.wgjwhj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zr.szxytkj.cn

Go:   json.Marshal(obj)
来源：http://xy.colortex.cn

Ruby: obj.to_json                                     // require "json"
来源：http://oi.lnxyls.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vh.jianghongdianzi.cn

[K02] JSON 字符串转对象
来源：http://nd.9csxet.cn

Py:   json.loads(s)
来源：http://eb.colortex.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://et.shtwfgs.cn

JS:   JSON.parse(s)
来源：http://ce.hnjuh.cn

TS:   JSON.parse(s)
来源：http://op.asd995.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jb.newstarts.cn

Go:   json.Unmarshal(data, &v)
来源：http://mo.hahajie.cn

Ruby: JSON.parse(s)
来源：http://sg.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ty.newstarts.cn

[K03] JSON 美化输出（带缩进）
来源：http://zy.szxytkj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rw.panjiajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cp.szxytkj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gl.shxzukj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bb.wgjwhj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dq.521024.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dq.521024.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gr.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ma.panjiajie.cn

[K04] 读取 JSON 文件
来源：http://nf.colortex.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dc.panjiajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fh.9csxet.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jd.panjiajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mq.521024.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hg.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hy.chemitech.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://lf.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dh.521024.cn

[K05] 深拷贝对象
来源：http://js.yuntaijiaju.cn

Py:   copy.deepcopy(obj)
来源：http://cj.wgjwhj.cn

PHP:  unserialize(serialize($obj));
来源：http://wq.wgjwhj.cn

JS:   structuredClone(obj)
来源：http://ow.nszjky.cn

TS:   structuredClone(obj)
来源：http://gk.huanxung.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ed.colortex.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://le.asd995.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sj.colortex.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ti.gzmigu.cn

[K06] 解析 URL 查询串
来源：http://ql.yuexingan06.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yj.colortex.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lv.9csxet.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lc.huanxung.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sl.shtwfgs.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hk.shtwfgs.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zf.yuntaijiaju.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cm.chemitech.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jh.9csxet.cn

[K07] 进制转换
来源：http://zc.lnxyls.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ot.haigaiapp.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cx.hnjuh.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://re.wgjwhj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qh.haigaiapp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://td.shxzukj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qa.szsharing.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rh.9csxet.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wh.huixinmuqiang.cn

[K08] 二进制序列化（非 JSON）
来源：http://gq.asd995.cn

Py:   pickle.dumps(obj)
来源：http://ue.shxzukj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xn.huixinmuqiang.cn

JS:   v8.serialize(obj)        // Node
来源：http://as.szsharing.cn

TS:   v8.serialize(obj)        // Node
来源：http://cc.huixiangedu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vu.yuntaijiaju.cn

Go:   encoding/gob
来源：http://jz.newstarts.cn

Ruby: Marshal.dump(obj)
来源：http://rc.gzmigu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kl.haigaiapp.cn

================================================================================
来源：http://lz.bookmarksfly.cn

L. 网络请求
来源：http://kl.shtwfgs.cn

================================================================================
来源：http://lp.szsharing.cn

[L01] 发送 GET 请求
来源：http://pq.colortex.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dk.521024.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wv.szxytkj.cn

JS:   await fetch(url)
来源：http://ov.yuntaijiaju.cn

TS:   await fetch(url)
来源：http://ux.hahajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ky.jianghongdianzi.cn

Go:   resp, err := http.Get(url)
来源：http://ow.shxzskj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://nc.nicolike.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kb.hnjuh.cn

[L02] 发送 POST JSON
来源：http://fu.bjjhwx.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cs.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wk.bookmarksfly.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://to.panjiajie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xb.colortex.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://du.jctech888.com.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pb.shxzskj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gm.bookmarksfly.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://no.hnjuh.cn

[L03] 设置自定义请求头
来源：http://dy.shxzukj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cb.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ka.521024.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pa.asd995.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yi.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bk.newstarts.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://eb.hahajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ux.lnxyls.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ya.colortex.cn

[L04] 设置超时
来源：http://nn.szsharing.cn

Py:   requests.get(url, timeout=5)
来源：http://ul.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rt.lnxyls.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://na.hnjuh.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fc.colortex.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cz.bookmarksfly.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uf.bookmarksfly.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tb.521024.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gc.shtwfgs.cn

[L05] 上传文件（multipart）
来源：http://sk.huixinmuqiang.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://la.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gr.shxzskj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://oe.muxihuayi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zo.haigaiapp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zc.huanxung.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lg.521024.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sv.haigaiapp.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wt.gzmigu.cn

[L06] 解析响应为 JSON
来源：http://bi.chemitech.net.cn

Py:   resp.json()
来源：http://od.wgjwhj.cn

PHP:  json_decode($body, true);
来源：http://yw.jctech888.com.cn

JS:   await resp.json()
来源：http://db.yuexingan06.cn

TS:   await resp.json()
来源：http://jn.nicolike.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bh.yuexingan06.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lq.colortex.cn

Ruby: JSON.parse(resp.body)
来源：http://kz.huanxung.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://th.chemitech.net.cn

[L07] 处理 HTTP 状态码
来源：http://od.panjiajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tw.huixiangedu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://oc.hahajie.cn

JS:   resp.ok;  resp.status
来源：http://it.asd995.cn

TS:   resp.ok;  resp.status
来源：http://xr.hnjuh.cn

Java: resp.statusCode()
来源：http://di.jianghongdianzi.cn

Go:   resp.StatusCode
来源：http://at.nicolike.cn

Ruby: resp.code.to_i
来源：http://vp.huixiangedu.cn

C#:   (int)resp.StatusCode
来源：http://dr.shxzskj.cn

[L08] 并发请求多个地址
来源：http://lh.lnxyls.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gi.bjjhwx.cn

PHP:  curl_multi_init() 系列
来源：http://kw.bookmarksfly.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zf.9csxet.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nj.lnxyls.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bz.bookmarksfly.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://io.huixiangedu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sr.shtwfgs.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mu.haigaiapp.cn

================================================================================
来源：http://fc.jctech888.com.cn

M. 命令行 / 进程 / 环境
来源：http://es.yuntaijiaju.cn

================================================================================
来源：http://vn.panjiajie.cn

[M01] 读取命令行参数
来源：http://br.chemitech.net.cn

Py:   sys.argv[1:]
来源：http://ib.bookmarksfly.cn

PHP:  $argv;  $argc;
来源：http://bf.lnxyls.cn

JS:   process.argv.slice(2)
来源：http://zy.shxzukj.cn

TS:   process.argv.slice(2)
来源：http://ef.haigaiapp.cn

Java: args 数组（main 方法参数）
来源：http://mf.shxzskj.cn

Go:   os.Args[1:]
来源：http://bj.jianghongdianzi.cn

Ruby: ARGV
来源：http://xn.gzmigu.cn

C#:   args 数组（Main 方法参数）
来源：http://ye.9csxet.cn

[M02] 读取环境变量
来源：http://rv.lnxyls.cn

Py:   os.environ.get("HOME")
来源：http://tq.colortex.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ll.haigaiapp.cn

JS:   process.env.HOME
来源：http://kp.szxytkj.cn

TS:   process.env.HOME
来源：http://jx.jianghongdianzi.cn

Java: System.getenv("HOME")
来源：http://nb.bjjhwx.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://er.yuexingan06.cn

Ruby: ENV["HOME"]
来源：http://no.lnxyls.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cg.panjiajie.cn

[M03] 执行外部命令
来源：http://gl.huixiangedu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zw.nszjky.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cg.yuexingan06.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vt.shtwfgs.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://bx.huanxung.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://oa.bjjhwx.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ab.hahajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://px.jctech888.com.cn

C#:   Process.Start("ls", "-l");
来源：http://kj.szxytkj.cn

[M04] 获取当前工作目录
来源：http://og.asd995.cn

Py:   os.getcwd()
来源：http://zh.yuexingan06.cn

PHP:  getcwd();
来源：http://rz.huixiangedu.cn

JS:   process.cwd()
来源：http://fh.nicolike.cn

TS:   process.cwd()
来源：http://uk.bookmarksfly.cn

Java: Path.of("").toAbsolutePath()
来源：http://ng.shtwfgs.cn

Go:   os.Getwd()
来源：http://mg.wgjwhj.cn

Ruby: Dir.pwd
来源：http://vu.jianghongdianzi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://lj.gzmigu.cn

[M05] 设置退出码
来源：http://kd.521024.cn

Py:   sys.exit(1)
来源：http://as.lnxyls.cn

PHP:  exit(1);
来源：http://ev.szsharing.cn

JS:   process.exit(1)
来源：http://mn.szsharing.cn

TS:   process.exit(1)
来源：http://so.hnjuh.cn

Java: System.exit(1)
来源：http://dd.chemitech.net.cn

Go:   os.Exit(1)
来源：http://df.huixinmuqiang.cn

Ruby: exit 1
来源：http://xv.shxzukj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qb.9csxet.cn

[M06] 向标准错误输出
来源：http://ms.hnjuh.cn

Py:   print("err", file=sys.stderr)
来源：http://xt.bookmarksfly.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jf.muxihuayi.cn

JS:   console.error("err")
来源：http://nd.wgjwhj.cn

TS:   console.error("err")
来源：http://oo.lnxyls.cn

Java: System.err.println("err")
来源：http://ih.huixinmuqiang.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xw.shtwfgs.cn

Ruby: warn "err"
来源：http://at.huixinmuqiang.cn

C#:   Console.Error.WriteLine("err")
来源：http://wi.gzmigu.cn

[M07] 判断是否为主入口
来源：http://rq.szsharing.cn

Py:   if __name__ == "__main__":
来源：http://mf.bjjhwx.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xk.bookmarksfly.cn

JS:   require.main === module
来源：http://qo.jianghongdianzi.cn

TS:   require.main === module
来源：http://tg.szxytkj.cn

Java: public static void main(String[] args)
来源：http://nv.szsharing.cn

Go:   func main()
来源：http://ez.panjiajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ca.jianghongdianzi.cn

C#:   static void Main(string[] args)
来源：http://ns.huixinmuqiang.cn

[M08] 获取系统与运行时信息
来源：http://hu.shtwfgs.cn

Py:   platform.system();  platform.python_version()
来源：http://uy.muxihuayi.cn

PHP:  PHP_OS;  phpversion();
来源：http://sp.yuexingan06.cn

JS:   process.platform;  process.version
来源：http://aj.hnjuh.cn

TS:   process.platform;  process.version
来源：http://pg.haigaiapp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ft.huanxung.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://jx.haigaiapp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jh.shxzukj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ws.jianghongdianzi.cn

================================================================================
来源：http://db.chemitech.net.cn

N. 数据结构与算法
来源：http://zs.gzmigu.cn

================================================================================
来源：http://hl.shxzskj.cn

[N01] 二分查找（有序数组）
来源：http://oq.hnjuh.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fy.muxihuayi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ax.hahajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ku.huixinmuqiang.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://em.jianghongdianzi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qj.9csxet.cn

Go:   sort.SearchInts(arr, x)
来源：http://xg.chemitech.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://so.asd995.cn

C#:   Array.BinarySearch(arr, x)
来源：http://bj.yuntaijiaju.cn

[N02] 排序（工程实践用内置实现）
来源：http://yh.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://qn.yuntaijiaju.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ap.colortex.cn


<!-- 参考信息 -->