代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sz.bjjhwx.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ss.colortex.cn

[J05] 时间加减（加 7 天）
来源：http://ct.szxytkj.cn

Py:   now + timedelta(days=7)
来源：http://im.nszjky.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xn.szxytkj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sj.jianghongdianzi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gx.huixiangedu.cn

Java: LocalDate.now().plusDays(7)
来源：http://st.colortex.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://iz.shxzskj.cn

Ruby: Time.now + 7 * 86400
来源：http://vy.bjjhwx.cn

C#:   DateTime.Now.AddDays(7)
来源：http://po.szsharing.cn

[J06] 计算两时间之差
来源：http://no.lnxyls.cn

Py:   (end - start).total_seconds()
来源：http://at.hahajie.cn

PHP:  $end->diff($start)->days;
来源：http://ti.nszjky.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zh.shxzskj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pj.szxytkj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://tg.shtwfgs.cn

Go:   end.Sub(start).Hours()
来源：http://dj.chemitech.net.cn

Ruby: end - start                 # 返回秒数
来源：http://lq.yuexingan06.cn

C#:   (end - start).TotalSeconds
来源：http://ou.shxzukj.cn

[J07] 比较两个日期
来源：http://xu.jianghongdianzi.cn

Py:   d1 < d2;  d1 == d2
来源：http://mq.newstarts.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hc.chemitech.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xa.huixinmuqiang.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mv.yuexingan06.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://im.jianghongdianzi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ao.huixinmuqiang.cn

Ruby: d1 < d2;  d1 == d2
来源：http://uz.colortex.cn

C#:   d1 < d2;  d1 == d2
来源：http://ck.9csxet.cn

[J08] 提取年月日与星期
来源：http://aq.gzmigu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tr.szxytkj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nh.shxzskj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yc.haigaiapp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vs.9csxet.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://oe.asd995.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xl.yuntaijiaju.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bq.huixinmuqiang.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qc.nszjky.cn

[J09] 时区处理
来源：http://wi.panjiajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://db.haigaiapp.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yi.bookmarksfly.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vf.yuexingan06.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ab.newstarts.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://at.bookmarksfly.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cb.nicolike.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://aw.jctech888.com.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jl.shtwfgs.cn

[J10] 取今天 / 本月第一天
来源：http://hj.9csxet.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kp.521024.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ro.lnxyls.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zl.shxzukj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ew.nszjky.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yn.chemitech.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kf.huanxung.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kp.bjjhwx.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cm.jianghongdianzi.cn

================================================================================
来源：http://kp.shxzukj.cn

K. JSON 与序列化
来源：http://vm.chemitech.net.cn

================================================================================
来源：http://fe.gzmigu.cn

[K01] 对象转 JSON 字符串
来源：http://tp.huixinmuqiang.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ug.shxzskj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ke.asd995.cn

JS:   JSON.stringify(obj)
来源：http://wi.szsharing.cn

TS:   JSON.stringify(obj)
来源：http://ij.hahajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://id.nszjky.cn

Go:   json.Marshal(obj)
来源：http://yc.huixinmuqiang.cn

Ruby: obj.to_json                                     // require "json"
来源：http://is.hnjuh.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vh.shxzskj.cn

[K02] JSON 字符串转对象
来源：http://nh.lnxyls.cn

Py:   json.loads(s)
来源：http://zy.jctech888.com.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ev.yuexingan06.cn

JS:   JSON.parse(s)
来源：http://cr.szxytkj.cn

TS:   JSON.parse(s)
来源：http://ah.jianghongdianzi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://io.szsharing.cn

Go:   json.Unmarshal(data, &v)
来源：http://yj.szxytkj.cn

Ruby: JSON.parse(s)
来源：http://ht.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sx.szsharing.cn

[K03] JSON 美化输出（带缩进）
来源：http://cr.jctech888.com.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rk.hnjuh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yu.lnxyls.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hf.wgjwhj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qf.521024.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pq.gzmigu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lu.panjiajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hv.9csxet.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ah.521024.cn

[K04] 读取 JSON 文件
来源：http://ct.newstarts.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yu.huixinmuqiang.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fe.gzmigu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wd.hnjuh.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ge.szsharing.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pp.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rh.lnxyls.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ft.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://au.colortex.cn

[K05] 深拷贝对象
来源：http://cc.jctech888.com.cn

Py:   copy.deepcopy(obj)
来源：http://bc.szxytkj.cn

PHP:  unserialize(serialize($obj));
来源：http://hr.colortex.cn

JS:   structuredClone(obj)
来源：http://nq.hahajie.cn

TS:   structuredClone(obj)
来源：http://ex.nszjky.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ir.shtwfgs.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ys.shxzskj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://us.521024.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yh.gzmigu.cn

[K06] 解析 URL 查询串
来源：http://us.panjiajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wc.szsharing.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xy.shxzskj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qs.szxytkj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vg.lnxyls.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sl.huixinmuqiang.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dw.muxihuayi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cm.nszjky.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zb.bookmarksfly.cn

[K07] 进制转换
来源：http://yc.gzmigu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cs.shxzukj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ux.colortex.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ga.hahajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mv.shxzukj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://km.colortex.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lr.jianghongdianzi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cm.hnjuh.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ds.huixinmuqiang.cn

[K08] 二进制序列化（非 JSON）
来源：http://ws.521024.cn

Py:   pickle.dumps(obj)
来源：http://hb.bookmarksfly.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zf.muxihuayi.cn

JS:   v8.serialize(obj)        // Node
来源：http://os.nicolike.cn

TS:   v8.serialize(obj)        // Node
来源：http://ia.newstarts.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yj.yuntaijiaju.cn

Go:   encoding/gob
来源：http://lq.521024.cn

Ruby: Marshal.dump(obj)
来源：http://rq.szxytkj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jt.huanxung.cn

================================================================================
来源：http://xy.wgjwhj.cn

L. 网络请求
来源：http://wr.jianghongdianzi.cn

================================================================================
来源：http://vx.yuntaijiaju.cn

[L01] 发送 GET 请求
来源：http://fa.haigaiapp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ju.shtwfgs.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nl.huanxung.cn

JS:   await fetch(url)
来源：http://wz.jianghongdianzi.cn

TS:   await fetch(url)
来源：http://xh.shxzukj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zj.shtwfgs.cn

Go:   resp, err := http.Get(url)
来源：http://cp.9csxet.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://mz.asd995.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rn.huixiangedu.cn

[L02] 发送 POST JSON
来源：http://ya.9csxet.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ch.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ey.shxzskj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ff.hahajie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vu.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xl.huixiangedu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ez.asd995.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bx.gzmigu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fe.yuexingan06.cn

[L03] 设置自定义请求头
来源：http://mh.panjiajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cz.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dl.szsharing.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uy.huanxung.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ef.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bz.asd995.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://oa.nicolike.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mn.szxytkj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ml.lnxyls.cn

[L04] 设置超时
来源：http://wd.shtwfgs.cn

Py:   requests.get(url, timeout=5)
来源：http://yt.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://du.panjiajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ii.szxytkj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rj.shxzskj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sr.huixinmuqiang.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://oh.jianghongdianzi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mv.huixiangedu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://eo.panjiajie.cn

[L05] 上传文件（multipart）
来源：http://cm.gzmigu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yc.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ud.shtwfgs.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qb.bjjhwx.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://eh.huanxung.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tk.jianghongdianzi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nw.asd995.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xy.bjjhwx.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gg.yuexingan06.cn

[L06] 解析响应为 JSON
来源：http://sw.bookmarksfly.cn

Py:   resp.json()
来源：http://ep.jianghongdianzi.cn

PHP:  json_decode($body, true);
来源：http://sw.nicolike.cn

JS:   await resp.json()
来源：http://mi.jianghongdianzi.cn

TS:   await resp.json()
来源：http://gu.jctech888.com.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ok.shxzskj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lz.huixinmuqiang.cn

Ruby: JSON.parse(resp.body)
来源：http://lf.newstarts.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fn.nszjky.cn

[L07] 处理 HTTP 状态码
来源：http://pe.bjjhwx.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fx.szsharing.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qe.asd995.cn

JS:   resp.ok;  resp.status
来源：http://gf.jianghongdianzi.cn

TS:   resp.ok;  resp.status
来源：http://tr.haigaiapp.cn

Java: resp.statusCode()
来源：http://va.jctech888.com.cn

Go:   resp.StatusCode
来源：http://cc.wgjwhj.cn

Ruby: resp.code.to_i
来源：http://sw.huixiangedu.cn

C#:   (int)resp.StatusCode
来源：http://sq.lnxyls.cn

[L08] 并发请求多个地址
来源：http://fz.shtwfgs.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ua.bookmarksfly.cn

PHP:  curl_multi_init() 系列
来源：http://jl.asd995.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ci.shtwfgs.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://br.yuntaijiaju.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nh.asd995.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qq.nszjky.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ge.haigaiapp.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nx.yuexingan06.cn

================================================================================
来源：http://tv.muxihuayi.cn

M. 命令行 / 进程 / 环境
来源：http://hs.521024.cn

================================================================================
来源：http://tp.chemitech.net.cn

[M01] 读取命令行参数
来源：http://yi.bookmarksfly.cn

Py:   sys.argv[1:]
来源：http://ns.wgjwhj.cn

PHP:  $argv;  $argc;
来源：http://qt.shtwfgs.cn

JS:   process.argv.slice(2)
来源：http://sh.jianghongdianzi.cn

TS:   process.argv.slice(2)
来源：http://es.9csxet.cn

Java: args 数组（main 方法参数）
来源：http://vp.bookmarksfly.cn

Go:   os.Args[1:]
来源：http://nz.haigaiapp.cn

Ruby: ARGV
来源：http://nn.jctech888.com.cn

C#:   args 数组（Main 方法参数）
来源：http://tm.lnxyls.cn

[M02] 读取环境变量
来源：http://xc.9csxet.cn

Py:   os.environ.get("HOME")
来源：http://yg.lnxyls.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vr.hahajie.cn

JS:   process.env.HOME
来源：http://gs.yuexingan06.cn

TS:   process.env.HOME
来源：http://ch.hahajie.cn

Java: System.getenv("HOME")
来源：http://cm.lnxyls.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ww.bjjhwx.cn

Ruby: ENV["HOME"]
来源：http://df.haigaiapp.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zc.shtwfgs.cn

[M03] 执行外部命令
来源：http://oy.bookmarksfly.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bm.bookmarksfly.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ow.asd995.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://fk.yuntaijiaju.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://kl.bjjhwx.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yn.huanxung.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://sz.wgjwhj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pz.huixiangedu.cn

C#:   Process.Start("ls", "-l");
来源：http://kv.wgjwhj.cn

[M04] 获取当前工作目录
来源：http://hv.szsharing.cn

Py:   os.getcwd()
来源：http://fz.bjjhwx.cn

PHP:  getcwd();
来源：http://jk.jctech888.com.cn

JS:   process.cwd()
来源：http://kd.panjiajie.cn

TS:   process.cwd()
来源：http://av.shxzukj.cn

Java: Path.of("").toAbsolutePath()
来源：http://pa.panjiajie.cn

Go:   os.Getwd()
来源：http://kh.bookmarksfly.cn

Ruby: Dir.pwd
来源：http://jf.shtwfgs.cn

C#:   Directory.GetCurrentDirectory()
来源：http://kz.lnxyls.cn

[M05] 设置退出码
来源：http://dm.colortex.cn

Py:   sys.exit(1)
来源：http://su.panjiajie.cn

PHP:  exit(1);
来源：http://if.bookmarksfly.cn

JS:   process.exit(1)
来源：http://eh.gzmigu.cn

TS:   process.exit(1)
来源：http://wm.yuexingan06.cn

Java: System.exit(1)
来源：http://vg.newstarts.cn

Go:   os.Exit(1)
来源：http://yi.newstarts.cn

Ruby: exit 1
来源：http://wm.gzmigu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xo.colortex.cn

[M06] 向标准错误输出
来源：http://tf.hnjuh.cn

Py:   print("err", file=sys.stderr)
来源：http://um.hnjuh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cl.jianghongdianzi.cn

JS:   console.error("err")
来源：http://sa.shxzskj.cn

TS:   console.error("err")
来源：http://zy.huanxung.cn

Java: System.err.println("err")
来源：http://xm.chemitech.net.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dl.hahajie.cn

Ruby: warn "err"
来源：http://um.panjiajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://xv.hnjuh.cn

[M07] 判断是否为主入口
来源：http://eg.chemitech.net.cn

Py:   if __name__ == "__main__":
来源：http://gw.hahajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ez.nicolike.cn

JS:   require.main === module
来源：http://zd.bjjhwx.cn

TS:   require.main === module
来源：http://or.asd995.cn

Java: public static void main(String[] args)
来源：http://dp.jianghongdianzi.cn

Go:   func main()
来源：http://xh.chemitech.net.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ws.chemitech.net.cn

C#:   static void Main(string[] args)
来源：http://le.nicolike.cn

[M08] 获取系统与运行时信息
来源：http://jw.huixiangedu.cn

Py:   platform.system();  platform.python_version()
来源：http://nt.huanxung.cn

PHP:  PHP_OS;  phpversion();
来源：http://df.shtwfgs.cn

JS:   process.platform;  process.version
来源：http://kz.asd995.cn

TS:   process.platform;  process.version
来源：http://vg.bjjhwx.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oj.bjjhwx.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ua.huanxung.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ws.lnxyls.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ec.lnxyls.cn

================================================================================
来源：http://mw.bookmarksfly.cn

N. 数据结构与算法
来源：http://cp.yuntaijiaju.cn

================================================================================
来源：http://cs.gzmigu.cn

[N01] 二分查找（有序数组）
来源：http://dj.shtwfgs.cn

Py:   bisect.bisect_left(arr, x)
来源：http://xc.hnjuh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kc.521024.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jh.gzmigu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zv.bjjhwx.cn

Java: Arrays.binarySearch(arr, x)
来源：http://bm.hahajie.cn

Go:   sort.SearchInts(arr, x)
来源：http://jw.huanxung.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qr.nszjky.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jb.jctech888.com.cn

[N02] 排序（工程实践用内置实现）
来源：http://td.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://kw.szxytkj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wm.szxytkj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ok.huixinmuqiang.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zg.hahajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ap.wgjwhj.cn

Go:   slices.Sort(arr)
来源：http://su.wgjwhj.cn


<!-- 参考信息 -->