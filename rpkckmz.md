代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bu.shxzukj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://mt.colortex.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tw.newstarts.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mj.asd995.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://js.chemitech.net.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vc.lnxyls.cn

[J05] 时间加减（加 7 天）
来源：http://ht.nszjky.cn

Py:   now + timedelta(days=7)
来源：http://yz.nicolike.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pk.521024.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sg.jianghongdianzi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://et.szsharing.cn

Java: LocalDate.now().plusDays(7)
来源：http://la.nszjky.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://im.muxihuayi.cn

Ruby: Time.now + 7 * 86400
来源：http://ss.hahajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ed.lnxyls.cn

[J06] 计算两时间之差
来源：http://pu.lnxyls.cn

Py:   (end - start).total_seconds()
来源：http://ol.wgjwhj.cn

PHP:  $end->diff($start)->days;
来源：http://ri.huixinmuqiang.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cy.shxzskj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bu.colortex.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gj.panjiajie.cn

Go:   end.Sub(start).Hours()
来源：http://bu.hnjuh.cn

Ruby: end - start                 # 返回秒数
来源：http://yr.jctech888.com.cn

C#:   (end - start).TotalSeconds
来源：http://yo.asd995.cn

[J07] 比较两个日期
来源：http://wh.newstarts.cn

Py:   d1 < d2;  d1 == d2
来源：http://am.haigaiapp.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vv.gzmigu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://dj.haigaiapp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ip.yuntaijiaju.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uk.szxytkj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fv.haigaiapp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wi.panjiajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://ul.huixiangedu.cn

[J08] 提取年月日与星期
来源：http://jk.bjjhwx.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xw.haigaiapp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://eh.huixiangedu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://af.huixinmuqiang.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://si.lnxyls.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://oe.jctech888.com.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mz.shxzukj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fx.gzmigu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pa.gzmigu.cn

[J09] 时区处理
来源：http://wi.panjiajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cu.nszjky.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xh.haigaiapp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rm.huixiangedu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wi.bookmarksfly.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vl.521024.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://in.asd995.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cl.wgjwhj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pb.shxzskj.cn

[J10] 取今天 / 本月第一天
来源：http://sw.9csxet.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://qy.shxzskj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ik.hnjuh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://by.haigaiapp.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sd.newstarts.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tc.bjjhwx.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fi.colortex.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kv.hnjuh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ii.bookmarksfly.cn

================================================================================
来源：http://jf.szxytkj.cn

K. JSON 与序列化
来源：http://do.huanxung.cn

================================================================================
来源：http://mq.asd995.cn

[K01] 对象转 JSON 字符串
来源：http://ui.lnxyls.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gf.panjiajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bt.hnjuh.cn

JS:   JSON.stringify(obj)
来源：http://xo.nicolike.cn

TS:   JSON.stringify(obj)
来源：http://ae.huanxung.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ww.yuntaijiaju.cn

Go:   json.Marshal(obj)
来源：http://cb.haigaiapp.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qe.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://me.nszjky.cn

[K02] JSON 字符串转对象
来源：http://nw.9csxet.cn

Py:   json.loads(s)
来源：http://ne.nszjky.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ev.haigaiapp.cn

JS:   JSON.parse(s)
来源：http://ch.yuntaijiaju.cn

TS:   JSON.parse(s)
来源：http://fz.nszjky.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://py.nszjky.cn

Go:   json.Unmarshal(data, &v)
来源：http://cv.asd995.cn

Ruby: JSON.parse(s)
来源：http://iy.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mh.nszjky.cn

[K03] JSON 美化输出（带缩进）
来源：http://qe.gzmigu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qx.szsharing.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qa.szxytkj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://oo.nicolike.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://dj.shxzukj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ov.shxzskj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://br.nszjky.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ve.shxzskj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yq.panjiajie.cn

[K04] 读取 JSON 文件
来源：http://le.yuntaijiaju.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hg.521024.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tp.wgjwhj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bb.jianghongdianzi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pc.hnjuh.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://te.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bn.jianghongdianzi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zp.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://oe.bookmarksfly.cn

[K05] 深拷贝对象
来源：http://em.shxzukj.cn

Py:   copy.deepcopy(obj)
来源：http://pq.jianghongdianzi.cn

PHP:  unserialize(serialize($obj));
来源：http://zl.nszjky.cn

JS:   structuredClone(obj)
来源：http://wf.huixiangedu.cn

TS:   structuredClone(obj)
来源：http://rq.huanxung.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://oi.newstarts.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hh.lnxyls.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ee.nicolike.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gi.yuexingan06.cn

[K06] 解析 URL 查询串
来源：http://mi.colortex.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ej.wgjwhj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pz.szxytkj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kb.gzmigu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rp.huanxung.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ru.newstarts.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hx.haigaiapp.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bs.wgjwhj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://im.huanxung.cn

[K07] 进制转换
来源：http://un.jctech888.com.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://el.colortex.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qt.bjjhwx.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kg.gzmigu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pu.muxihuayi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yl.shxzskj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sc.jctech888.com.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ma.huixinmuqiang.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kd.hahajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://ux.chemitech.net.cn

Py:   pickle.dumps(obj)
来源：http://eb.jctech888.com.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fd.bookmarksfly.cn

JS:   v8.serialize(obj)        // Node
来源：http://me.szxytkj.cn

TS:   v8.serialize(obj)        // Node
来源：http://tt.colortex.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ql.newstarts.cn

Go:   encoding/gob
来源：http://tg.newstarts.cn

Ruby: Marshal.dump(obj)
来源：http://sv.huixinmuqiang.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://li.huixiangedu.cn

================================================================================
来源：http://qm.hahajie.cn

L. 网络请求
来源：http://op.hnjuh.cn

================================================================================
来源：http://ot.yuntaijiaju.cn

[L01] 发送 GET 请求
来源：http://eg.asd995.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mc.wgjwhj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jb.muxihuayi.cn

JS:   await fetch(url)
来源：http://pj.lnxyls.cn

TS:   await fetch(url)
来源：http://am.huanxung.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ot.nicolike.cn

Go:   resp, err := http.Get(url)
来源：http://cp.szxytkj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hj.haigaiapp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://te.chemitech.net.cn

[L02] 发送 POST JSON
来源：http://tg.huixiangedu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://se.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mg.521024.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zt.chemitech.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fe.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pt.hahajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ie.bookmarksfly.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ug.shtwfgs.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bz.nicolike.cn

[L03] 设置自定义请求头
来源：http://db.panjiajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pr.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://oi.yuexingan06.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qh.hnjuh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lt.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ni.521024.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ow.nicolike.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nv.jctech888.com.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://un.jctech888.com.cn

[L04] 设置超时
来源：http://ek.szsharing.cn

Py:   requests.get(url, timeout=5)
来源：http://io.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dq.szsharing.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rv.521024.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://at.wgjwhj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lz.yuntaijiaju.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ux.huixiangedu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cg.nicolike.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ht.colortex.cn

[L05] 上传文件（multipart）
来源：http://oj.asd995.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gn.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hh.szsharing.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vm.521024.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vu.wgjwhj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cw.nszjky.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ed.huixinmuqiang.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://po.hnjuh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vu.newstarts.cn

[L06] 解析响应为 JSON
来源：http://uu.colortex.cn

Py:   resp.json()
来源：http://qm.muxihuayi.cn

PHP:  json_decode($body, true);
来源：http://pw.muxihuayi.cn

JS:   await resp.json()
来源：http://ka.chemitech.net.cn

TS:   await resp.json()
来源：http://fw.szxytkj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xj.gzmigu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nw.chemitech.net.cn

Ruby: JSON.parse(resp.body)
来源：http://bk.nszjky.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pq.shxzskj.cn

[L07] 处理 HTTP 状态码
来源：http://yu.haigaiapp.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zz.nszjky.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ag.muxihuayi.cn

JS:   resp.ok;  resp.status
来源：http://kd.huixinmuqiang.cn

TS:   resp.ok;  resp.status
来源：http://ro.521024.cn

Java: resp.statusCode()
来源：http://yc.muxihuayi.cn

Go:   resp.StatusCode
来源：http://fg.huixinmuqiang.cn

Ruby: resp.code.to_i
来源：http://no.nicolike.cn

C#:   (int)resp.StatusCode
来源：http://me.shxzskj.cn

[L08] 并发请求多个地址
来源：http://ea.jctech888.com.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bw.szxytkj.cn

PHP:  curl_multi_init() 系列
来源：http://nw.huixiangedu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qg.huixinmuqiang.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pm.521024.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ft.nicolike.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mo.colortex.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rg.bookmarksfly.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://df.nicolike.cn

================================================================================
来源：http://nc.yuntaijiaju.cn

M. 命令行 / 进程 / 环境
来源：http://jq.panjiajie.cn

================================================================================
来源：http://bk.nszjky.cn

[M01] 读取命令行参数
来源：http://vv.jctech888.com.cn

Py:   sys.argv[1:]
来源：http://xp.9csxet.cn

PHP:  $argv;  $argc;
来源：http://pr.9csxet.cn

JS:   process.argv.slice(2)
来源：http://dc.huanxung.cn

TS:   process.argv.slice(2)
来源：http://cf.shtwfgs.cn

Java: args 数组（main 方法参数）
来源：http://om.huixiangedu.cn

Go:   os.Args[1:]
来源：http://ap.huixiangedu.cn

Ruby: ARGV
来源：http://gy.jctech888.com.cn

C#:   args 数组（Main 方法参数）
来源：http://ra.haigaiapp.cn

[M02] 读取环境变量
来源：http://iw.szxytkj.cn

Py:   os.environ.get("HOME")
来源：http://hm.9csxet.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://id.chemitech.net.cn

JS:   process.env.HOME
来源：http://yt.szxytkj.cn

TS:   process.env.HOME
来源：http://th.chemitech.net.cn

Java: System.getenv("HOME")
来源：http://pg.asd995.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jb.haigaiapp.cn

Ruby: ENV["HOME"]
来源：http://tq.wgjwhj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ku.521024.cn

[M03] 执行外部命令
来源：http://nq.huixinmuqiang.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zy.newstarts.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xq.asd995.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://mg.hahajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yb.huixiangedu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zw.bookmarksfly.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xv.haigaiapp.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qi.colortex.cn

C#:   Process.Start("ls", "-l");
来源：http://rs.shxzskj.cn

[M04] 获取当前工作目录
来源：http://qc.szsharing.cn

Py:   os.getcwd()
来源：http://og.muxihuayi.cn

PHP:  getcwd();
来源：http://du.shxzukj.cn

JS:   process.cwd()
来源：http://wt.colortex.cn

TS:   process.cwd()
来源：http://ur.szxytkj.cn

Java: Path.of("").toAbsolutePath()
来源：http://ce.hnjuh.cn

Go:   os.Getwd()
来源：http://yq.newstarts.cn

Ruby: Dir.pwd
来源：http://qn.szxytkj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ys.chemitech.net.cn

[M05] 设置退出码
来源：http://yi.shtwfgs.cn

Py:   sys.exit(1)
来源：http://dl.shxzskj.cn

PHP:  exit(1);
来源：http://mq.jctech888.com.cn

JS:   process.exit(1)
来源：http://gi.shxzskj.cn

TS:   process.exit(1)
来源：http://hy.jctech888.com.cn

Java: System.exit(1)
来源：http://gi.yuexingan06.cn

Go:   os.Exit(1)
来源：http://oe.asd995.cn

Ruby: exit 1
来源：http://qh.gzmigu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ux.shxzukj.cn

[M06] 向标准错误输出
来源：http://lw.lnxyls.cn

Py:   print("err", file=sys.stderr)
来源：http://kp.asd995.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kx.jianghongdianzi.cn

JS:   console.error("err")
来源：http://la.bjjhwx.cn

TS:   console.error("err")
来源：http://im.newstarts.cn

Java: System.err.println("err")
来源：http://vo.haigaiapp.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mq.huixiangedu.cn

Ruby: warn "err"
来源：http://ep.jianghongdianzi.cn

C#:   Console.Error.WriteLine("err")
来源：http://nb.chemitech.net.cn

[M07] 判断是否为主入口
来源：http://ki.521024.cn

Py:   if __name__ == "__main__":
来源：http://yd.wgjwhj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qd.bookmarksfly.cn

JS:   require.main === module
来源：http://xb.lnxyls.cn

TS:   require.main === module
来源：http://ep.wgjwhj.cn

Java: public static void main(String[] args)
来源：http://di.huanxung.cn

Go:   func main()
来源：http://vf.521024.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://es.hnjuh.cn

C#:   static void Main(string[] args)
来源：http://ig.wgjwhj.cn

[M08] 获取系统与运行时信息
来源：http://gf.yuntaijiaju.cn

Py:   platform.system();  platform.python_version()
来源：http://zo.huixinmuqiang.cn

PHP:  PHP_OS;  phpversion();
来源：http://au.shxzskj.cn

JS:   process.platform;  process.version
来源：http://bg.jctech888.com.cn

TS:   process.platform;  process.version
来源：http://fb.huixiangedu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zz.muxihuayi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://do.newstarts.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://it.jctech888.com.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://sg.9csxet.cn

================================================================================
来源：http://nm.wgjwhj.cn

N. 数据结构与算法
来源：http://em.yuntaijiaju.cn

================================================================================
来源：http://et.asd995.cn

[N01] 二分查找（有序数组）
来源：http://cb.gzmigu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sg.gzmigu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tp.haigaiapp.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rt.shxzskj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ra.lnxyls.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yx.lnxyls.cn

Go:   sort.SearchInts(arr, x)
来源：http://vo.szxytkj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ww.shtwfgs.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gl.nicolike.cn

[N02] 排序（工程实践用内置实现）
来源：http://ht.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://yu.521024.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rx.bookmarksfly.cn


<!-- 参考信息 -->