代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fd.szxytkj.cn

[J04] 时间戳与日期互转
来源：http://ov.chemitech.net.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zs.hahajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dd.bookmarksfly.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://aq.chemitech.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tu.shxzskj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ok.wgjwhj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ht.9csxet.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dj.huixiangedu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pb.chemitech.net.cn

[J05] 时间加减（加 7 天）
来源：http://dh.huixiangedu.cn

Py:   now + timedelta(days=7)
来源：http://sz.hnjuh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ra.shxzukj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xm.521024.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kh.jctech888.com.cn

Java: LocalDate.now().plusDays(7)
来源：http://sl.wgjwhj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://td.521024.cn

Ruby: Time.now + 7 * 86400
来源：http://np.nszjky.cn

C#:   DateTime.Now.AddDays(7)
来源：http://eb.huixinmuqiang.cn

[J06] 计算两时间之差
来源：http://ts.colortex.cn

Py:   (end - start).total_seconds()
来源：http://xz.shtwfgs.cn

PHP:  $end->diff($start)->days;
来源：http://vq.shxzukj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jg.jianghongdianzi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yv.nicolike.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hl.gzmigu.cn

Go:   end.Sub(start).Hours()
来源：http://qt.asd995.cn

Ruby: end - start                 # 返回秒数
来源：http://qk.shxzskj.cn

C#:   (end - start).TotalSeconds
来源：http://bn.newstarts.cn

[J07] 比较两个日期
来源：http://pt.lnxyls.cn

Py:   d1 < d2;  d1 == d2
来源：http://vi.jctech888.com.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zz.lnxyls.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ar.521024.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hk.bookmarksfly.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://es.newstarts.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wk.muxihuayi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://dn.newstarts.cn

C#:   d1 < d2;  d1 == d2
来源：http://ii.haigaiapp.cn

[J08] 提取年月日与星期
来源：http://dl.yuntaijiaju.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vi.bjjhwx.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rz.wgjwhj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ac.9csxet.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hc.muxihuayi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qc.shtwfgs.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dm.nszjky.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ra.szxytkj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wc.hnjuh.cn

[J09] 时区处理
来源：http://kc.wgjwhj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jo.gzmigu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ui.muxihuayi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gc.panjiajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ab.shtwfgs.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kv.nszjky.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kx.jctech888.com.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pv.colortex.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qv.shtwfgs.cn

[J10] 取今天 / 本月第一天
来源：http://xt.newstarts.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kt.nszjky.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://am.bookmarksfly.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xv.huixiangedu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://aq.yuexingan06.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wf.jianghongdianzi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sn.lnxyls.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ha.newstarts.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xk.nicolike.cn

================================================================================
来源：http://wm.lnxyls.cn

K. JSON 与序列化
来源：http://vm.newstarts.cn

================================================================================
来源：http://za.chemitech.net.cn

[K01] 对象转 JSON 字符串
来源：http://yr.nicolike.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ks.colortex.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kp.newstarts.cn

JS:   JSON.stringify(obj)
来源：http://ly.yuntaijiaju.cn

TS:   JSON.stringify(obj)
来源：http://ad.gzmigu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ap.9csxet.cn

Go:   json.Marshal(obj)
来源：http://dk.gzmigu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://pj.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ij.521024.cn

[K02] JSON 字符串转对象
来源：http://po.newstarts.cn

Py:   json.loads(s)
来源：http://bt.huanxung.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bg.bookmarksfly.cn

JS:   JSON.parse(s)
来源：http://jj.lnxyls.cn

TS:   JSON.parse(s)
来源：http://vg.huanxung.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fs.521024.cn

Go:   json.Unmarshal(data, &v)
来源：http://gg.bookmarksfly.cn

Ruby: JSON.parse(s)
来源：http://la.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://le.nicolike.cn

[K03] JSON 美化输出（带缩进）
来源：http://hu.hahajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cp.shtwfgs.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gs.gzmigu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jh.9csxet.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://pz.jctech888.com.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lg.huanxung.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vm.shtwfgs.cn

Ruby: JSON.pretty_generate(obj)
来源：http://km.szxytkj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wu.huixinmuqiang.cn

[K04] 读取 JSON 文件
来源：http://cg.asd995.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ma.shxzukj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://py.nszjky.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hf.521024.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bn.szxytkj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tt.szsharing.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://oe.hnjuh.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zv.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zn.521024.cn

[K05] 深拷贝对象
来源：http://fh.521024.cn

Py:   copy.deepcopy(obj)
来源：http://vp.9csxet.cn

PHP:  unserialize(serialize($obj));
来源：http://sx.521024.cn

JS:   structuredClone(obj)
来源：http://ie.521024.cn

TS:   structuredClone(obj)
来源：http://pc.szxytkj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bt.shxzskj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sh.521024.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ve.jctech888.com.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://iq.huanxung.cn

[K06] 解析 URL 查询串
来源：http://gi.chemitech.net.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ct.bjjhwx.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ym.jctech888.com.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qw.lnxyls.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://al.huanxung.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ed.jianghongdianzi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://iq.muxihuayi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yx.newstarts.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nb.yuntaijiaju.cn

[K07] 进制转换
来源：http://bp.yuntaijiaju.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qx.9csxet.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rq.jctech888.com.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tf.nszjky.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xy.gzmigu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xx.jianghongdianzi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rg.huixiangedu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kd.asd995.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ca.shtwfgs.cn

[K08] 二进制序列化（非 JSON）
来源：http://bf.colortex.cn

Py:   pickle.dumps(obj)
来源：http://ws.panjiajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nf.huanxung.cn

JS:   v8.serialize(obj)        // Node
来源：http://lg.hahajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://ug.nicolike.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qi.chemitech.net.cn

Go:   encoding/gob
来源：http://xs.newstarts.cn

Ruby: Marshal.dump(obj)
来源：http://nl.yuntaijiaju.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pn.jianghongdianzi.cn

================================================================================
来源：http://ei.panjiajie.cn

L. 网络请求
来源：http://mt.chemitech.net.cn

================================================================================
来源：http://rd.shtwfgs.cn

[L01] 发送 GET 请求
来源：http://lu.panjiajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jd.shxzskj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pe.shtwfgs.cn

JS:   await fetch(url)
来源：http://kl.muxihuayi.cn

TS:   await fetch(url)
来源：http://vs.yuexingan06.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mb.hnjuh.cn

Go:   resp, err := http.Get(url)
来源：http://vx.jctech888.com.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://au.hahajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://et.bookmarksfly.cn

[L02] 发送 POST JSON
来源：http://wg.yuntaijiaju.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rx.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fn.yuexingan06.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fy.nicolike.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vp.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vp.colortex.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ei.newstarts.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ir.jianghongdianzi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://me.huixiangedu.cn

[L03] 设置自定义请求头
来源：http://ld.jianghongdianzi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://iz.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fn.bjjhwx.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jw.asd995.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pc.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vm.muxihuayi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cr.panjiajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://um.muxihuayi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kl.gzmigu.cn

[L04] 设置超时
来源：http://de.huixiangedu.cn

Py:   requests.get(url, timeout=5)
来源：http://ho.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://me.szxytkj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xd.muxihuayi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ix.yuexingan06.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://iy.szxytkj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tc.asd995.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nm.szxytkj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ug.shtwfgs.cn

[L05] 上传文件（multipart）
来源：http://wh.colortex.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zp.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yi.huanxung.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rd.521024.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tr.yuexingan06.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xf.nszjky.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ch.nicolike.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bj.shxzskj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xx.szsharing.cn

[L06] 解析响应为 JSON
来源：http://cx.nicolike.cn

Py:   resp.json()
来源：http://xj.szsharing.cn

PHP:  json_decode($body, true);
来源：http://yy.huixiangedu.cn

JS:   await resp.json()
来源：http://wg.yuexingan06.cn

TS:   await resp.json()
来源：http://ye.lnxyls.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hi.hnjuh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bs.huixiangedu.cn

Ruby: JSON.parse(resp.body)
来源：http://xn.521024.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ry.jctech888.com.cn

[L07] 处理 HTTP 状态码
来源：http://hw.gzmigu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://di.haigaiapp.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cl.yuexingan06.cn

JS:   resp.ok;  resp.status
来源：http://mv.jianghongdianzi.cn

TS:   resp.ok;  resp.status
来源：http://gw.gzmigu.cn

Java: resp.statusCode()
来源：http://th.nicolike.cn

Go:   resp.StatusCode
来源：http://kf.nszjky.cn

Ruby: resp.code.to_i
来源：http://lb.colortex.cn

C#:   (int)resp.StatusCode
来源：http://xe.shtwfgs.cn

[L08] 并发请求多个地址
来源：http://va.panjiajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ip.shxzskj.cn

PHP:  curl_multi_init() 系列
来源：http://rn.jctech888.com.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://st.yuntaijiaju.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pg.jianghongdianzi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lm.shxzskj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ls.hnjuh.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wn.yuexingan06.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sx.huanxung.cn

================================================================================
来源：http://zs.newstarts.cn

M. 命令行 / 进程 / 环境
来源：http://yg.bookmarksfly.cn

================================================================================
来源：http://qu.shxzukj.cn

[M01] 读取命令行参数
来源：http://fj.shxzskj.cn

Py:   sys.argv[1:]
来源：http://mj.muxihuayi.cn

PHP:  $argv;  $argc;
来源：http://qx.521024.cn

JS:   process.argv.slice(2)
来源：http://bh.newstarts.cn

TS:   process.argv.slice(2)
来源：http://sq.colortex.cn

Java: args 数组（main 方法参数）
来源：http://cu.hnjuh.cn

Go:   os.Args[1:]
来源：http://xv.jctech888.com.cn

Ruby: ARGV
来源：http://rv.hahajie.cn

C#:   args 数组（Main 方法参数）
来源：http://tn.yuntaijiaju.cn

[M02] 读取环境变量
来源：http://yc.521024.cn

Py:   os.environ.get("HOME")
来源：http://tj.nszjky.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gb.huixinmuqiang.cn

JS:   process.env.HOME
来源：http://rq.nicolike.cn

TS:   process.env.HOME
来源：http://ws.huanxung.cn

Java: System.getenv("HOME")
来源：http://zc.bjjhwx.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tt.newstarts.cn

Ruby: ENV["HOME"]
来源：http://kz.huixinmuqiang.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jh.colortex.cn

[M03] 执行外部命令
来源：http://bc.jianghongdianzi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://sx.haigaiapp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ei.yuntaijiaju.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pt.jianghongdianzi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wy.panjiajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mv.hahajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ab.nicolike.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vg.nszjky.cn

C#:   Process.Start("ls", "-l");
来源：http://oy.haigaiapp.cn

[M04] 获取当前工作目录
来源：http://ab.bjjhwx.cn

Py:   os.getcwd()
来源：http://ig.jctech888.com.cn

PHP:  getcwd();
来源：http://xb.panjiajie.cn

JS:   process.cwd()
来源：http://at.chemitech.net.cn

TS:   process.cwd()
来源：http://xw.hnjuh.cn

Java: Path.of("").toAbsolutePath()
来源：http://oh.yuexingan06.cn

Go:   os.Getwd()
来源：http://bb.9csxet.cn

Ruby: Dir.pwd
来源：http://pw.521024.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hd.panjiajie.cn

[M05] 设置退出码
来源：http://fb.huixinmuqiang.cn

Py:   sys.exit(1)
来源：http://cl.shtwfgs.cn

PHP:  exit(1);
来源：http://ox.nicolike.cn

JS:   process.exit(1)
来源：http://mb.9csxet.cn

TS:   process.exit(1)
来源：http://nc.yuntaijiaju.cn

Java: System.exit(1)
来源：http://dn.nicolike.cn

Go:   os.Exit(1)
来源：http://rv.newstarts.cn

Ruby: exit 1
来源：http://ti.bookmarksfly.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ht.newstarts.cn

[M06] 向标准错误输出
来源：http://cp.haigaiapp.cn

Py:   print("err", file=sys.stderr)
来源：http://qs.bjjhwx.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://es.shtwfgs.cn

JS:   console.error("err")
来源：http://dp.hnjuh.cn

TS:   console.error("err")
来源：http://pw.yuexingan06.cn

Java: System.err.println("err")
来源：http://ll.9csxet.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ts.panjiajie.cn

Ruby: warn "err"
来源：http://zf.haigaiapp.cn

C#:   Console.Error.WriteLine("err")
来源：http://vn.shtwfgs.cn

[M07] 判断是否为主入口
来源：http://wy.bjjhwx.cn

Py:   if __name__ == "__main__":
来源：http://ww.gzmigu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zd.newstarts.cn

JS:   require.main === module
来源：http://kn.newstarts.cn

TS:   require.main === module
来源：http://iu.szsharing.cn

Java: public static void main(String[] args)
来源：http://nb.yuntaijiaju.cn

Go:   func main()
来源：http://so.szxytkj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kp.nicolike.cn

C#:   static void Main(string[] args)
来源：http://ui.521024.cn

[M08] 获取系统与运行时信息
来源：http://fu.huanxung.cn

Py:   platform.system();  platform.python_version()
来源：http://xv.haigaiapp.cn

PHP:  PHP_OS;  phpversion();
来源：http://mk.gzmigu.cn

JS:   process.platform;  process.version
来源：http://lp.shxzskj.cn

TS:   process.platform;  process.version
来源：http://wd.huixinmuqiang.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jl.huixinmuqiang.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://sm.521024.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://eb.colortex.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://yc.huanxung.cn

================================================================================
来源：http://tq.huixinmuqiang.cn

N. 数据结构与算法
来源：http://hw.colortex.cn

================================================================================
来源：http://hp.chemitech.net.cn

[N01] 二分查找（有序数组）
来源：http://tr.shxzskj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kl.asd995.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://db.shxzskj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dt.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sq.jctech888.com.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ao.hnjuh.cn

Go:   sort.SearchInts(arr, x)
来源：http://qt.szsharing.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://md.lnxyls.cn


<!-- 参考信息 -->