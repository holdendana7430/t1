代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gd.hnjuh.cn

[J04] 时间戳与日期互转
来源：http://rx.shxzskj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rl.bookmarksfly.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gl.muxihuayi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uq.9csxet.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wy.lnxyls.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sk.nicolike.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zr.panjiajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hy.yuexingan06.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lt.wgjwhj.cn

[J05] 时间加减（加 7 天）
来源：http://ss.521024.cn

Py:   now + timedelta(days=7)
来源：http://qp.shtwfgs.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://cu.nicolike.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://td.colortex.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wj.wgjwhj.cn

Java: LocalDate.now().plusDays(7)
来源：http://ch.jctech888.com.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jd.asd995.cn

Ruby: Time.now + 7 * 86400
来源：http://ac.huanxung.cn

C#:   DateTime.Now.AddDays(7)
来源：http://je.newstarts.cn

[J06] 计算两时间之差
来源：http://iw.lnxyls.cn

Py:   (end - start).total_seconds()
来源：http://ke.shxzukj.cn

PHP:  $end->diff($start)->days;
来源：http://yc.huixiangedu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ug.colortex.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eg.gzmigu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mj.hahajie.cn

Go:   end.Sub(start).Hours()
来源：http://bm.gzmigu.cn

Ruby: end - start                 # 返回秒数
来源：http://xg.gzmigu.cn

C#:   (end - start).TotalSeconds
来源：http://fp.yuexingan06.cn

[J07] 比较两个日期
来源：http://it.chemitech.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://al.szxytkj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xo.chemitech.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vu.nszjky.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hh.colortex.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bz.jianghongdianzi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://es.shxzskj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://os.nicolike.cn

C#:   d1 < d2;  d1 == d2
来源：http://mi.newstarts.cn

[J08] 提取年月日与星期
来源：http://lh.jianghongdianzi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ha.colortex.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ay.bjjhwx.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gt.colortex.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yf.szsharing.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hs.szsharing.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ql.lnxyls.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bl.hnjuh.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jf.lnxyls.cn

[J09] 时区处理
来源：http://ia.huixinmuqiang.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xf.bookmarksfly.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dm.shtwfgs.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mr.huixiangedu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fs.bjjhwx.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://on.chemitech.net.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ma.hnjuh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://le.szxytkj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dm.hahajie.cn

[J10] 取今天 / 本月第一天
来源：http://cq.shtwfgs.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://qx.colortex.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hc.jianghongdianzi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://el.wgjwhj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zl.521024.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wy.shxzukj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tw.bjjhwx.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lt.hahajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bl.nicolike.cn

================================================================================
来源：http://dc.hnjuh.cn

K. JSON 与序列化
来源：http://nq.chemitech.net.cn

================================================================================
来源：http://gq.nszjky.cn

[K01] 对象转 JSON 字符串
来源：http://hp.gzmigu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sx.gzmigu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xd.colortex.cn

JS:   JSON.stringify(obj)
来源：http://po.hnjuh.cn

TS:   JSON.stringify(obj)
来源：http://oc.huixinmuqiang.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ah.jctech888.com.cn

Go:   json.Marshal(obj)
来源：http://ap.hnjuh.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ge.shxzukj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xr.asd995.cn

[K02] JSON 字符串转对象
来源：http://bi.haigaiapp.cn

Py:   json.loads(s)
来源：http://fr.yuexingan06.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fp.9csxet.cn

JS:   JSON.parse(s)
来源：http://uq.nicolike.cn

TS:   JSON.parse(s)
来源：http://uc.szsharing.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lm.hnjuh.cn

Go:   json.Unmarshal(data, &v)
来源：http://fr.jianghongdianzi.cn

Ruby: JSON.parse(s)
来源：http://rm.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vh.yuexingan06.cn

[K03] JSON 美化输出（带缩进）
来源：http://fh.shtwfgs.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ic.gzmigu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ta.521024.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://se.panjiajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://no.bookmarksfly.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kw.gzmigu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lq.haigaiapp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dz.newstarts.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uy.asd995.cn

[K04] 读取 JSON 文件
来源：http://ni.wgjwhj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://de.asd995.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://au.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mk.muxihuayi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wg.nicolike.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ri.nszjky.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://if.huixiangedu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vo.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zp.huixiangedu.cn

[K05] 深拷贝对象
来源：http://wy.panjiajie.cn

Py:   copy.deepcopy(obj)
来源：http://gn.gzmigu.cn

PHP:  unserialize(serialize($obj));
来源：http://zg.shxzukj.cn

JS:   structuredClone(obj)
来源：http://qe.yuntaijiaju.cn

TS:   structuredClone(obj)
来源：http://kq.huixinmuqiang.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://cw.gzmigu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qw.nszjky.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mr.chemitech.net.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ld.hahajie.cn

[K06] 解析 URL 查询串
来源：http://yy.wgjwhj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fd.hahajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pi.asd995.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zb.huixiangedu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vc.jianghongdianzi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wp.panjiajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://id.9csxet.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fz.lnxyls.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xa.yuexingan06.cn

[K07] 进制转换
来源：http://mc.jianghongdianzi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tr.asd995.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lf.yuntaijiaju.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rj.nszjky.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://de.9csxet.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mr.jianghongdianzi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jd.nicolike.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fo.yuntaijiaju.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qw.colortex.cn

[K08] 二进制序列化（非 JSON）
来源：http://jt.huanxung.cn

Py:   pickle.dumps(obj)
来源：http://nr.jianghongdianzi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://qt.colortex.cn

JS:   v8.serialize(obj)        // Node
来源：http://kb.jianghongdianzi.cn

TS:   v8.serialize(obj)        // Node
来源：http://xl.yuexingan06.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ot.jctech888.com.cn

Go:   encoding/gob
来源：http://mc.9csxet.cn

Ruby: Marshal.dump(obj)
来源：http://ru.521024.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yt.jianghongdianzi.cn

================================================================================
来源：http://xw.bjjhwx.cn

L. 网络请求
来源：http://me.shxzukj.cn

================================================================================
来源：http://ww.wgjwhj.cn

[L01] 发送 GET 请求
来源：http://vy.yuntaijiaju.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ue.lnxyls.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dv.newstarts.cn

JS:   await fetch(url)
来源：http://bm.yuntaijiaju.cn

TS:   await fetch(url)
来源：http://hf.wgjwhj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hs.bjjhwx.cn

Go:   resp, err := http.Get(url)
来源：http://wp.muxihuayi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xb.shxzukj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vj.huixiangedu.cn

[L02] 发送 POST JSON
来源：http://dk.huanxung.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vv.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ur.hnjuh.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ep.gzmigu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sb.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ey.yuexingan06.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hf.gzmigu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lz.wgjwhj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tq.szsharing.cn

[L03] 设置自定义请求头
来源：http://ln.haigaiapp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hk.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yv.szxytkj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ms.yuexingan06.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hf.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yn.shxzskj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hi.yuexingan06.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tk.bookmarksfly.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://aw.yuntaijiaju.cn

[L04] 设置超时
来源：http://ez.lnxyls.cn

Py:   requests.get(url, timeout=5)
来源：http://gd.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ld.yuexingan06.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ds.huanxung.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xw.gzmigu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://oj.wgjwhj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bm.lnxyls.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ps.asd995.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rw.colortex.cn

[L05] 上传文件（multipart）
来源：http://wu.nicolike.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://av.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ym.muxihuayi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mn.asd995.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xc.szxytkj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gj.shxzskj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vg.huanxung.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://te.huixiangedu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uj.panjiajie.cn

[L06] 解析响应为 JSON
来源：http://cx.shtwfgs.cn

Py:   resp.json()
来源：http://qe.huixiangedu.cn

PHP:  json_decode($body, true);
来源：http://dk.muxihuayi.cn

JS:   await resp.json()
来源：http://zc.9csxet.cn

TS:   await resp.json()
来源：http://iv.hnjuh.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mz.yuexingan06.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hv.lnxyls.cn

Ruby: JSON.parse(resp.body)
来源：http://ga.chemitech.net.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sm.bookmarksfly.cn

[L07] 处理 HTTP 状态码
来源：http://lj.hahajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hm.shxzukj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fp.bookmarksfly.cn

JS:   resp.ok;  resp.status
来源：http://ta.hnjuh.cn

TS:   resp.ok;  resp.status
来源：http://nr.bjjhwx.cn

Java: resp.statusCode()
来源：http://pb.colortex.cn

Go:   resp.StatusCode
来源：http://vu.bookmarksfly.cn

Ruby: resp.code.to_i
来源：http://jk.huixiangedu.cn

C#:   (int)resp.StatusCode
来源：http://rr.9csxet.cn

[L08] 并发请求多个地址
来源：http://bw.colortex.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fg.bjjhwx.cn

PHP:  curl_multi_init() 系列
来源：http://mu.hnjuh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nt.muxihuayi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uq.hnjuh.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mo.hahajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ag.shxzskj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sr.shxzskj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vc.newstarts.cn

================================================================================
来源：http://ji.nicolike.cn

M. 命令行 / 进程 / 环境
来源：http://pi.hnjuh.cn

================================================================================
来源：http://bz.hnjuh.cn

[M01] 读取命令行参数
来源：http://kh.newstarts.cn

Py:   sys.argv[1:]
来源：http://vg.yuexingan06.cn

PHP:  $argv;  $argc;
来源：http://ks.shtwfgs.cn

JS:   process.argv.slice(2)
来源：http://ix.huixiangedu.cn

TS:   process.argv.slice(2)
来源：http://lm.nszjky.cn

Java: args 数组（main 方法参数）
来源：http://ha.shxzukj.cn

Go:   os.Args[1:]
来源：http://jj.lnxyls.cn

Ruby: ARGV
来源：http://zq.gzmigu.cn

C#:   args 数组（Main 方法参数）
来源：http://nd.shxzskj.cn

[M02] 读取环境变量
来源：http://kq.gzmigu.cn

Py:   os.environ.get("HOME")
来源：http://ko.jianghongdianzi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ga.yuntaijiaju.cn

JS:   process.env.HOME
来源：http://wo.asd995.cn

TS:   process.env.HOME
来源：http://sn.shxzukj.cn

Java: System.getenv("HOME")
来源：http://gx.haigaiapp.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kh.hnjuh.cn

Ruby: ENV["HOME"]
来源：http://dd.hahajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qp.wgjwhj.cn

[M03] 执行外部命令
来源：http://xf.shxzskj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zk.bookmarksfly.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ih.yuexingan06.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ol.shxzukj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fu.nszjky.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jk.huixinmuqiang.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://rk.shtwfgs.cn

Ruby: system("ls -l");  `ls -l`
来源：http://oy.szxytkj.cn

C#:   Process.Start("ls", "-l");
来源：http://wn.szxytkj.cn

[M04] 获取当前工作目录
来源：http://rz.hahajie.cn

Py:   os.getcwd()
来源：http://dr.szxytkj.cn

PHP:  getcwd();
来源：http://oz.lnxyls.cn

JS:   process.cwd()
来源：http://zk.521024.cn

TS:   process.cwd()
来源：http://ny.panjiajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://nx.jctech888.com.cn

Go:   os.Getwd()
来源：http://sf.lnxyls.cn

Ruby: Dir.pwd
来源：http://nn.9csxet.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yp.lnxyls.cn

[M05] 设置退出码
来源：http://jm.yuexingan06.cn

Py:   sys.exit(1)
来源：http://ve.521024.cn

PHP:  exit(1);
来源：http://jo.bookmarksfly.cn

JS:   process.exit(1)
来源：http://hc.jianghongdianzi.cn

TS:   process.exit(1)
来源：http://no.huixinmuqiang.cn

Java: System.exit(1)
来源：http://jg.bookmarksfly.cn

Go:   os.Exit(1)
来源：http://nd.yuexingan06.cn

Ruby: exit 1
来源：http://ap.bjjhwx.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sg.colortex.cn

[M06] 向标准错误输出
来源：http://pb.bookmarksfly.cn

Py:   print("err", file=sys.stderr)
来源：http://eb.shxzukj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://oc.nszjky.cn

JS:   console.error("err")
来源：http://el.bjjhwx.cn

TS:   console.error("err")
来源：http://ro.asd995.cn

Java: System.err.println("err")
来源：http://zt.jctech888.com.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cq.nicolike.cn

Ruby: warn "err"
来源：http://zl.wgjwhj.cn

C#:   Console.Error.WriteLine("err")
来源：http://be.yuexingan06.cn

[M07] 判断是否为主入口
来源：http://hs.asd995.cn

Py:   if __name__ == "__main__":
来源：http://ph.panjiajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ap.asd995.cn

JS:   require.main === module
来源：http://jy.wgjwhj.cn

TS:   require.main === module
来源：http://kc.yuntaijiaju.cn

Java: public static void main(String[] args)
来源：http://my.newstarts.cn

Go:   func main()
来源：http://ge.asd995.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bw.haigaiapp.cn

C#:   static void Main(string[] args)
来源：http://mt.szsharing.cn

[M08] 获取系统与运行时信息
来源：http://qg.bjjhwx.cn

Py:   platform.system();  platform.python_version()
来源：http://im.shxzukj.cn

PHP:  PHP_OS;  phpversion();
来源：http://xw.szxytkj.cn

JS:   process.platform;  process.version
来源：http://uv.asd995.cn

TS:   process.platform;  process.version
来源：http://th.haigaiapp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vi.huanxung.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://iu.jctech888.com.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hs.lnxyls.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://up.asd995.cn

================================================================================
来源：http://dp.lnxyls.cn

N. 数据结构与算法
来源：http://fb.lnxyls.cn

================================================================================
来源：http://jc.muxihuayi.cn

[N01] 二分查找（有序数组）
来源：http://do.haigaiapp.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hm.muxihuayi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tw.jianghongdianzi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gj.newstarts.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cy.colortex.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jx.haigaiapp.cn

Go:   sort.SearchInts(arr, x)
来源：http://ux.shtwfgs.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ug.shtwfgs.cn


<!-- 参考信息 -->