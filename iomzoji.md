代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fq.colortex.cn

[J04] 时间戳与日期互转
来源：http://kg.gzmigu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://et.asd995.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://za.chemitech.net.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yd.hahajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vd.panjiajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fi.521024.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xa.huixiangedu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lj.jianghongdianzi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wp.nicolike.cn

[J05] 时间加减（加 7 天）
来源：http://uq.521024.cn

Py:   now + timedelta(days=7)
来源：http://hw.huanxung.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pf.lnxyls.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ce.huixinmuqiang.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wg.newstarts.cn

Java: LocalDate.now().plusDays(7)
来源：http://ss.yuexingan06.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ca.jianghongdianzi.cn

Ruby: Time.now + 7 * 86400
来源：http://xs.huanxung.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hg.asd995.cn

[J06] 计算两时间之差
来源：http://hm.szsharing.cn

Py:   (end - start).total_seconds()
来源：http://gf.huixinmuqiang.cn

PHP:  $end->diff($start)->days;
来源：http://fi.yuntaijiaju.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tv.muxihuayi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hq.gzmigu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xf.bookmarksfly.cn

Go:   end.Sub(start).Hours()
来源：http://an.jianghongdianzi.cn

Ruby: end - start                 # 返回秒数
来源：http://st.hahajie.cn

C#:   (end - start).TotalSeconds
来源：http://ye.jctech888.com.cn

[J07] 比较两个日期
来源：http://ht.newstarts.cn

Py:   d1 < d2;  d1 == d2
来源：http://my.newstarts.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jm.haigaiapp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ps.szxytkj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rb.haigaiapp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vj.yuexingan06.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rz.nicolike.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ar.521024.cn

C#:   d1 < d2;  d1 == d2
来源：http://qc.haigaiapp.cn

[J08] 提取年月日与星期
来源：http://xc.shxzukj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://uw.asd995.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tr.colortex.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ga.szsharing.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ia.huanxung.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mp.chemitech.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ny.yuntaijiaju.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vf.gzmigu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ix.nszjky.cn

[J09] 时区处理
来源：http://yn.lnxyls.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://is.yuexingan06.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mz.hnjuh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qr.muxihuayi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cx.newstarts.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dq.asd995.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kt.chemitech.net.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://sy.gzmigu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ri.huixiangedu.cn

[J10] 取今天 / 本月第一天
来源：http://nb.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ac.lnxyls.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://eg.muxihuayi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tr.nszjky.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qu.yuexingan06.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ny.hnjuh.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://oo.hnjuh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jc.shxzukj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ri.bookmarksfly.cn

================================================================================
来源：http://du.521024.cn

K. JSON 与序列化
来源：http://zo.hahajie.cn

================================================================================
来源：http://md.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://dk.yuexingan06.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mk.chemitech.net.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yv.wgjwhj.cn

JS:   JSON.stringify(obj)
来源：http://vh.jctech888.com.cn

TS:   JSON.stringify(obj)
来源：http://xo.yuexingan06.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gn.shxzskj.cn

Go:   json.Marshal(obj)
来源：http://nr.huanxung.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zf.huanxung.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hh.jctech888.com.cn

[K02] JSON 字符串转对象
来源：http://az.chemitech.net.cn

Py:   json.loads(s)
来源：http://nb.huixiangedu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mn.nszjky.cn

JS:   JSON.parse(s)
来源：http://sa.shtwfgs.cn

TS:   JSON.parse(s)
来源：http://nb.haigaiapp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yh.yuntaijiaju.cn

Go:   json.Unmarshal(data, &v)
来源：http://hq.yuexingan06.cn

Ruby: JSON.parse(s)
来源：http://lm.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cn.szsharing.cn

[K03] JSON 美化输出（带缩进）
来源：http://th.yuexingan06.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pl.chemitech.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ni.yuexingan06.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wr.lnxyls.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sk.jctech888.com.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sf.521024.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zl.jctech888.com.cn

Ruby: JSON.pretty_generate(obj)
来源：http://cn.asd995.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xs.shtwfgs.cn

[K04] 读取 JSON 文件
来源：http://gn.huixiangedu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jo.szxytkj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cl.bjjhwx.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ff.lnxyls.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://og.huixinmuqiang.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rj.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ue.yuexingan06.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vr.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://od.colortex.cn

[K05] 深拷贝对象
来源：http://vk.shxzukj.cn

Py:   copy.deepcopy(obj)
来源：http://lr.shxzukj.cn

PHP:  unserialize(serialize($obj));
来源：http://as.9csxet.cn

JS:   structuredClone(obj)
来源：http://xf.szsharing.cn

TS:   structuredClone(obj)
来源：http://dr.szxytkj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gc.panjiajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fc.jctech888.com.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ya.jianghongdianzi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dj.shtwfgs.cn

[K06] 解析 URL 查询串
来源：http://sc.haigaiapp.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vr.szsharing.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xd.jianghongdianzi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ik.shtwfgs.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wy.gzmigu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://he.9csxet.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cd.huixiangedu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cx.huixiangedu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dm.9csxet.cn

[K07] 进制转换
来源：http://dh.gzmigu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://os.shxzskj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kb.huixinmuqiang.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kw.nszjky.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ut.shxzskj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uq.hnjuh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tr.haigaiapp.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ho.szsharing.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ij.haigaiapp.cn

[K08] 二进制序列化（非 JSON）
来源：http://zw.colortex.cn

Py:   pickle.dumps(obj)
来源：http://zz.bjjhwx.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://qb.bjjhwx.cn

JS:   v8.serialize(obj)        // Node
来源：http://vd.hnjuh.cn

TS:   v8.serialize(obj)        // Node
来源：http://oa.yuntaijiaju.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ch.shtwfgs.cn

Go:   encoding/gob
来源：http://de.haigaiapp.cn

Ruby: Marshal.dump(obj)
来源：http://qx.lnxyls.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rm.newstarts.cn

================================================================================
来源：http://gy.yuexingan06.cn

L. 网络请求
来源：http://sd.jctech888.com.cn

================================================================================
来源：http://au.muxihuayi.cn

[L01] 发送 GET 请求
来源：http://fi.shxzskj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ah.colortex.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ve.jctech888.com.cn

JS:   await fetch(url)
来源：http://pe.yuntaijiaju.cn

TS:   await fetch(url)
来源：http://ps.yuntaijiaju.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vg.9csxet.cn

Go:   resp, err := http.Get(url)
来源：http://bo.newstarts.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ed.521024.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kl.hahajie.cn

[L02] 发送 POST JSON
来源：http://cz.gzmigu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rb.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jy.shtwfgs.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://er.shtwfgs.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oe.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sl.chemitech.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jz.newstarts.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://er.asd995.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ww.521024.cn

[L03] 设置自定义请求头
来源：http://gr.gzmigu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ui.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rs.huixiangedu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ju.newstarts.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://th.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ds.wgjwhj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pz.bookmarksfly.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wz.newstarts.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ek.szxytkj.cn

[L04] 设置超时
来源：http://mu.panjiajie.cn

Py:   requests.get(url, timeout=5)
来源：http://ul.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hn.hnjuh.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dm.panjiajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dg.huixiangedu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pv.nicolike.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zy.colortex.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://no.9csxet.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vn.haigaiapp.cn

[L05] 上传文件（multipart）
来源：http://za.yuntaijiaju.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sy.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sq.panjiajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dj.bjjhwx.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gp.jctech888.com.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dm.lnxyls.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ie.bookmarksfly.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ow.szxytkj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://km.szxytkj.cn

[L06] 解析响应为 JSON
来源：http://yy.colortex.cn

Py:   resp.json()
来源：http://ky.521024.cn

PHP:  json_decode($body, true);
来源：http://zw.nicolike.cn

JS:   await resp.json()
来源：http://qp.shtwfgs.cn

TS:   await resp.json()
来源：http://yo.jctech888.com.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ir.yuntaijiaju.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wf.szsharing.cn

Ruby: JSON.parse(resp.body)
来源：http://cg.gzmigu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fe.bjjhwx.cn

[L07] 处理 HTTP 状态码
来源：http://wv.hnjuh.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fq.shxzukj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yj.huixiangedu.cn

JS:   resp.ok;  resp.status
来源：http://lh.asd995.cn

TS:   resp.ok;  resp.status
来源：http://tt.colortex.cn

Java: resp.statusCode()
来源：http://ls.panjiajie.cn

Go:   resp.StatusCode
来源：http://qo.wgjwhj.cn

Ruby: resp.code.to_i
来源：http://az.haigaiapp.cn

C#:   (int)resp.StatusCode
来源：http://uf.chemitech.net.cn

[L08] 并发请求多个地址
来源：http://hd.haigaiapp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qk.bookmarksfly.cn

PHP:  curl_multi_init() 系列
来源：http://dm.huanxung.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://te.wgjwhj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://av.muxihuayi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hs.chemitech.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tk.yuntaijiaju.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mr.wgjwhj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qt.szsharing.cn

================================================================================
来源：http://bt.yuntaijiaju.cn

M. 命令行 / 进程 / 环境
来源：http://to.asd995.cn

================================================================================
来源：http://sw.gzmigu.cn

[M01] 读取命令行参数
来源：http://hw.yuexingan06.cn

Py:   sys.argv[1:]
来源：http://eb.newstarts.cn

PHP:  $argv;  $argc;
来源：http://hw.huixinmuqiang.cn

JS:   process.argv.slice(2)
来源：http://pl.shxzskj.cn

TS:   process.argv.slice(2)
来源：http://ic.szsharing.cn

Java: args 数组（main 方法参数）
来源：http://hk.hahajie.cn

Go:   os.Args[1:]
来源：http://cl.panjiajie.cn

Ruby: ARGV
来源：http://ht.szsharing.cn

C#:   args 数组（Main 方法参数）
来源：http://ry.newstarts.cn

[M02] 读取环境变量
来源：http://zu.bjjhwx.cn

Py:   os.environ.get("HOME")
来源：http://by.panjiajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vs.lnxyls.cn

JS:   process.env.HOME
来源：http://ym.colortex.cn

TS:   process.env.HOME
来源：http://pr.shxzukj.cn

Java: System.getenv("HOME")
来源：http://uw.wgjwhj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xr.shxzskj.cn

Ruby: ENV["HOME"]
来源：http://ck.hnjuh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qo.jctech888.com.cn

[M03] 执行外部命令
来源：http://xs.lnxyls.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ri.chemitech.net.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zx.colortex.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pj.huanxung.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://lt.shtwfgs.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uf.bookmarksfly.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://sw.shtwfgs.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tn.bjjhwx.cn

C#:   Process.Start("ls", "-l");
来源：http://gi.hnjuh.cn

[M04] 获取当前工作目录
来源：http://rw.gzmigu.cn

Py:   os.getcwd()
来源：http://ra.hnjuh.cn

PHP:  getcwd();
来源：http://mp.bookmarksfly.cn

JS:   process.cwd()
来源：http://qf.wgjwhj.cn

TS:   process.cwd()
来源：http://ta.shxzukj.cn

Java: Path.of("").toAbsolutePath()
来源：http://tp.huanxung.cn

Go:   os.Getwd()
来源：http://yf.muxihuayi.cn

Ruby: Dir.pwd
来源：http://wq.muxihuayi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zo.szxytkj.cn

[M05] 设置退出码
来源：http://wt.huixinmuqiang.cn

Py:   sys.exit(1)
来源：http://wc.hnjuh.cn

PHP:  exit(1);
来源：http://ql.hnjuh.cn

JS:   process.exit(1)
来源：http://gx.newstarts.cn

TS:   process.exit(1)
来源：http://vi.huanxung.cn

Java: System.exit(1)
来源：http://dr.chemitech.net.cn

Go:   os.Exit(1)
来源：http://eh.huanxung.cn

Ruby: exit 1
来源：http://hk.yuntaijiaju.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qh.jctech888.com.cn

[M06] 向标准错误输出
来源：http://ai.gzmigu.cn

Py:   print("err", file=sys.stderr)
来源：http://zb.asd995.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cn.shxzukj.cn

JS:   console.error("err")
来源：http://vv.521024.cn

TS:   console.error("err")
来源：http://jn.gzmigu.cn

Java: System.err.println("err")
来源：http://sx.newstarts.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tw.shxzskj.cn

Ruby: warn "err"
来源：http://fn.huixiangedu.cn

C#:   Console.Error.WriteLine("err")
来源：http://dj.521024.cn

[M07] 判断是否为主入口
来源：http://qp.nicolike.cn

Py:   if __name__ == "__main__":
来源：http://qm.521024.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ez.colortex.cn

JS:   require.main === module
来源：http://re.szxytkj.cn

TS:   require.main === module
来源：http://pc.muxihuayi.cn

Java: public static void main(String[] args)
来源：http://gj.nicolike.cn

Go:   func main()
来源：http://fh.yuexingan06.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ws.muxihuayi.cn

C#:   static void Main(string[] args)
来源：http://yy.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://cs.jianghongdianzi.cn

Py:   platform.system();  platform.python_version()
来源：http://tp.nicolike.cn

PHP:  PHP_OS;  phpversion();
来源：http://wi.shxzukj.cn

JS:   process.platform;  process.version
来源：http://we.shxzukj.cn

TS:   process.platform;  process.version
来源：http://xr.jianghongdianzi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jx.szxytkj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ve.hahajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://um.lnxyls.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ls.jctech888.com.cn

================================================================================
来源：http://zz.nszjky.cn

N. 数据结构与算法
来源：http://pn.huixinmuqiang.cn

================================================================================
来源：http://hu.muxihuayi.cn

[N01] 二分查找（有序数组）
来源：http://sl.huanxung.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bt.colortex.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nq.wgjwhj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mx.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ul.szxytkj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xj.chemitech.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://jr.bjjhwx.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qg.hahajie.cn


<!-- 参考信息 -->