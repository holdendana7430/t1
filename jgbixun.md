代发 wailian999

TS:   new Date("2024-01-02")
来源：http://ym.huanxung.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ou.muxihuayi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://me.9csxet.cn

Ruby: Date.parse("2024-01-02")
来源：http://ca.panjiajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kr.colortex.cn

[J04] 时间戳与日期互转
来源：http://ni.9csxet.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lo.shxzskj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jx.hahajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qt.yuntaijiaju.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://te.shtwfgs.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://no.bjjhwx.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ik.9csxet.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dd.szxytkj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qo.huixiangedu.cn

[J05] 时间加减（加 7 天）
来源：http://jq.hahajie.cn

Py:   now + timedelta(days=7)
来源：http://kp.nszjky.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yf.bjjhwx.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jq.lnxyls.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://oz.wgjwhj.cn

Java: LocalDate.now().plusDays(7)
来源：http://qj.shtwfgs.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wu.colortex.cn

Ruby: Time.now + 7 * 86400
来源：http://an.yuexingan06.cn

C#:   DateTime.Now.AddDays(7)
来源：http://fh.newstarts.cn

[J06] 计算两时间之差
来源：http://ku.asd995.cn

Py:   (end - start).total_seconds()
来源：http://vj.huixinmuqiang.cn

PHP:  $end->diff($start)->days;
来源：http://vo.panjiajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://iu.panjiajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cd.asd995.cn

Java: Duration.between(start, end).toSeconds()
来源：http://wy.szxytkj.cn

Go:   end.Sub(start).Hours()
来源：http://qz.colortex.cn

Ruby: end - start                 # 返回秒数
来源：http://gi.bjjhwx.cn

C#:   (end - start).TotalSeconds
来源：http://oy.panjiajie.cn

[J07] 比较两个日期
来源：http://kk.nszjky.cn

Py:   d1 < d2;  d1 == d2
来源：http://qx.hnjuh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ig.newstarts.cn

JS:   d1.getTime() < d2.getTime()
来源：http://dm.nicolike.cn

TS:   d1.getTime() < d2.getTime()
来源：http://na.nicolike.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dz.lnxyls.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://it.chemitech.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://im.jianghongdianzi.cn

C#:   d1 < d2;  d1 == d2
来源：http://qf.shxzukj.cn

[J08] 提取年月日与星期
来源：http://wm.muxihuayi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ye.9csxet.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rr.gzmigu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ys.huixiangedu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bj.shxzskj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sm.yuntaijiaju.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ib.huixinmuqiang.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xl.hahajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ho.hahajie.cn

[J09] 时区处理
来源：http://rx.newstarts.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nf.bjjhwx.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.szxytkj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rf.521024.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://md.haigaiapp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://so.nicolike.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://eq.jianghongdianzi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ba.panjiajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ro.szsharing.cn

[J10] 取今天 / 本月第一天
来源：http://sf.huanxung.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ew.newstarts.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kd.shtwfgs.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zd.chemitech.net.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nm.muxihuayi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ow.jctech888.com.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qe.huixiangedu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ve.newstarts.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mh.yuntaijiaju.cn

================================================================================
来源：http://xv.yuexingan06.cn

K. JSON 与序列化
来源：http://wi.jianghongdianzi.cn

================================================================================
来源：http://ua.521024.cn

[K01] 对象转 JSON 字符串
来源：http://zv.9csxet.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rb.shtwfgs.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://np.huixiangedu.cn

JS:   JSON.stringify(obj)
来源：http://mz.shxzskj.cn

TS:   JSON.stringify(obj)
来源：http://bj.shxzskj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ct.haigaiapp.cn

Go:   json.Marshal(obj)
来源：http://ib.szxytkj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://if.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://cm.bookmarksfly.cn

[K02] JSON 字符串转对象
来源：http://wl.huanxung.cn

Py:   json.loads(s)
来源：http://dv.colortex.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pz.jianghongdianzi.cn

JS:   JSON.parse(s)
来源：http://ok.szxytkj.cn

TS:   JSON.parse(s)
来源：http://hh.yuexingan06.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tg.bjjhwx.cn

Go:   json.Unmarshal(data, &v)
来源：http://zp.haigaiapp.cn

Ruby: JSON.parse(s)
来源：http://ay.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ua.shxzskj.cn

[K03] JSON 美化输出（带缩进）
来源：http://si.szxytkj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wh.asd995.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tt.shxzskj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hv.bjjhwx.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ul.bookmarksfly.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://le.gzmigu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dt.shxzskj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nh.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jq.nszjky.cn

[K04] 读取 JSON 文件
来源：http://ci.gzmigu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://eo.colortex.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nq.nicolike.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rj.521024.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mt.muxihuayi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zq.szxytkj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gu.asd995.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gn.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nv.huanxung.cn

[K05] 深拷贝对象
来源：http://gw.huixiangedu.cn

Py:   copy.deepcopy(obj)
来源：http://ev.9csxet.cn

PHP:  unserialize(serialize($obj));
来源：http://an.newstarts.cn

JS:   structuredClone(obj)
来源：http://bj.nicolike.cn

TS:   structuredClone(obj)
来源：http://dh.huixinmuqiang.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rv.nicolike.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sv.asd995.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nu.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ck.newstarts.cn

[K06] 解析 URL 查询串
来源：http://dk.yuexingan06.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rg.shxzskj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yi.gzmigu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cl.asd995.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hh.huanxung.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gm.yuexingan06.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qg.bookmarksfly.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://js.huixiangedu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ik.szsharing.cn

[K07] 进制转换
来源：http://yd.shxzukj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hr.huanxung.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://on.newstarts.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mg.colortex.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dg.nicolike.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://my.shxzukj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kc.huixiangedu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vq.muxihuayi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ri.jianghongdianzi.cn

[K08] 二进制序列化（非 JSON）
来源：http://ke.colortex.cn

Py:   pickle.dumps(obj)
来源：http://mu.521024.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hn.9csxet.cn

JS:   v8.serialize(obj)        // Node
来源：http://xh.gzmigu.cn

TS:   v8.serialize(obj)        // Node
来源：http://kf.jctech888.com.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gc.jianghongdianzi.cn

Go:   encoding/gob
来源：http://fh.gzmigu.cn

Ruby: Marshal.dump(obj)
来源：http://lv.521024.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sy.colortex.cn

================================================================================
来源：http://zn.asd995.cn

L. 网络请求
来源：http://qb.gzmigu.cn

================================================================================
来源：http://uo.bookmarksfly.cn

[L01] 发送 GET 请求
来源：http://kr.9csxet.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://aj.shtwfgs.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fc.lnxyls.cn

JS:   await fetch(url)
来源：http://ng.haigaiapp.cn

TS:   await fetch(url)
来源：http://up.jctech888.com.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zg.newstarts.cn

Go:   resp, err := http.Get(url)
来源：http://bp.colortex.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://yn.panjiajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jq.panjiajie.cn

[L02] 发送 POST JSON
来源：http://dr.jianghongdianzi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pz.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dk.szsharing.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oo.haigaiapp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rn.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ca.muxihuayi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hj.colortex.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yw.shxzukj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://aa.gzmigu.cn

[L03] 设置自定义请求头
来源：http://ep.lnxyls.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ku.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rp.lnxyls.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uk.yuntaijiaju.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://km.asd995.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rh.lnxyls.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zt.9csxet.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xl.yuntaijiaju.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yw.szxytkj.cn

[L04] 设置超时
来源：http://zr.9csxet.cn

Py:   requests.get(url, timeout=5)
来源：http://aj.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gd.szxytkj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lv.nszjky.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ud.colortex.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ez.muxihuayi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cm.yuexingan06.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nd.colortex.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hx.jianghongdianzi.cn

[L05] 上传文件（multipart）
来源：http://jo.asd995.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://go.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pe.shxzskj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uk.chemitech.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qp.shxzukj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pe.szsharing.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cb.chemitech.net.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xa.huixinmuqiang.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kt.lnxyls.cn

[L06] 解析响应为 JSON
来源：http://zs.szxytkj.cn

Py:   resp.json()
来源：http://fj.gzmigu.cn

PHP:  json_decode($body, true);
来源：http://de.521024.cn

JS:   await resp.json()
来源：http://rm.wgjwhj.cn

TS:   await resp.json()
来源：http://am.bjjhwx.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bm.bookmarksfly.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bf.hahajie.cn

Ruby: JSON.parse(resp.body)
来源：http://wl.gzmigu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://um.jianghongdianzi.cn

[L07] 处理 HTTP 状态码
来源：http://kx.yuntaijiaju.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://iz.muxihuayi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nz.hnjuh.cn

JS:   resp.ok;  resp.status
来源：http://do.shxzukj.cn

TS:   resp.ok;  resp.status
来源：http://df.bjjhwx.cn

Java: resp.statusCode()
来源：http://pm.wgjwhj.cn

Go:   resp.StatusCode
来源：http://js.yuexingan06.cn

Ruby: resp.code.to_i
来源：http://vr.gzmigu.cn

C#:   (int)resp.StatusCode
来源：http://za.yuexingan06.cn

[L08] 并发请求多个地址
来源：http://td.521024.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wd.shxzukj.cn

PHP:  curl_multi_init() 系列
来源：http://ts.9csxet.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ks.asd995.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hv.9csxet.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dw.haigaiapp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gc.szsharing.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ju.panjiajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://if.bjjhwx.cn

================================================================================
来源：http://ws.lnxyls.cn

M. 命令行 / 进程 / 环境
来源：http://ld.colortex.cn

================================================================================
来源：http://cb.wgjwhj.cn

[M01] 读取命令行参数
来源：http://ng.lnxyls.cn

Py:   sys.argv[1:]
来源：http://ae.colortex.cn

PHP:  $argv;  $argc;
来源：http://xa.yuntaijiaju.cn

JS:   process.argv.slice(2)
来源：http://fr.jianghongdianzi.cn

TS:   process.argv.slice(2)
来源：http://ul.huanxung.cn

Java: args 数组（main 方法参数）
来源：http://cg.hahajie.cn

Go:   os.Args[1:]
来源：http://gp.yuexingan06.cn

Ruby: ARGV
来源：http://yp.muxihuayi.cn

C#:   args 数组（Main 方法参数）
来源：http://ab.nicolike.cn

[M02] 读取环境变量
来源：http://xm.asd995.cn

Py:   os.environ.get("HOME")
来源：http://ew.szxytkj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jp.hahajie.cn

JS:   process.env.HOME
来源：http://bb.gzmigu.cn

TS:   process.env.HOME
来源：http://cu.huanxung.cn

Java: System.getenv("HOME")
来源：http://dl.asd995.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://me.szsharing.cn

Ruby: ENV["HOME"]
来源：http://bz.asd995.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nj.muxihuayi.cn

[M03] 执行外部命令
来源：http://ak.nszjky.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qh.haigaiapp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pf.lnxyls.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://sf.muxihuayi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://kf.nszjky.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gm.hahajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hy.chemitech.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ei.shtwfgs.cn

C#:   Process.Start("ls", "-l");
来源：http://cc.gzmigu.cn

[M04] 获取当前工作目录
来源：http://zk.asd995.cn

Py:   os.getcwd()
来源：http://yu.lnxyls.cn

PHP:  getcwd();
来源：http://iw.hnjuh.cn

JS:   process.cwd()
来源：http://ml.szsharing.cn

TS:   process.cwd()
来源：http://oj.yuexingan06.cn

Java: Path.of("").toAbsolutePath()
来源：http://tt.szsharing.cn

Go:   os.Getwd()
来源：http://ub.wgjwhj.cn

Ruby: Dir.pwd
来源：http://gw.jctech888.com.cn

C#:   Directory.GetCurrentDirectory()
来源：http://li.haigaiapp.cn

[M05] 设置退出码
来源：http://sg.shxzukj.cn

Py:   sys.exit(1)
来源：http://pk.shxzskj.cn

PHP:  exit(1);
来源：http://pz.huanxung.cn

JS:   process.exit(1)
来源：http://bc.bookmarksfly.cn

TS:   process.exit(1)
来源：http://tf.shxzukj.cn

Java: System.exit(1)
来源：http://hm.shxzskj.cn

Go:   os.Exit(1)
来源：http://dq.jctech888.com.cn

Ruby: exit 1
来源：http://dc.huixinmuqiang.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wx.haigaiapp.cn

[M06] 向标准错误输出
来源：http://lk.huixinmuqiang.cn

Py:   print("err", file=sys.stderr)
来源：http://uk.panjiajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pp.9csxet.cn

JS:   console.error("err")
来源：http://ve.lnxyls.cn

TS:   console.error("err")
来源：http://sl.shxzukj.cn

Java: System.err.println("err")
来源：http://pf.chemitech.net.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tz.muxihuayi.cn

Ruby: warn "err"
来源：http://on.jianghongdianzi.cn

C#:   Console.Error.WriteLine("err")
来源：http://bd.nszjky.cn

[M07] 判断是否为主入口
来源：http://az.panjiajie.cn

Py:   if __name__ == "__main__":
来源：http://tf.gzmigu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mw.panjiajie.cn

JS:   require.main === module
来源：http://ij.nicolike.cn

TS:   require.main === module
来源：http://mw.newstarts.cn

Java: public static void main(String[] args)
来源：http://wb.gzmigu.cn

Go:   func main()
来源：http://hx.jianghongdianzi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://de.shxzskj.cn

C#:   static void Main(string[] args)
来源：http://gv.yuntaijiaju.cn

[M08] 获取系统与运行时信息
来源：http://ev.colortex.cn

Py:   platform.system();  platform.python_version()
来源：http://jl.haigaiapp.cn

PHP:  PHP_OS;  phpversion();
来源：http://ar.asd995.cn

JS:   process.platform;  process.version
来源：http://dh.szxytkj.cn

TS:   process.platform;  process.version
来源：http://xy.asd995.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yi.asd995.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wk.chemitech.net.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uv.jianghongdianzi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://hn.huanxung.cn

================================================================================
来源：http://fz.nszjky.cn

N. 数据结构与算法
来源：http://ht.wgjwhj.cn

================================================================================
来源：http://gl.yuntaijiaju.cn

[N01] 二分查找（有序数组）
来源：http://ev.yuexingan06.cn

Py:   bisect.bisect_left(arr, x)
来源：http://me.chemitech.net.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ed.gzmigu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ir.huixiangedu.cn


<!-- 参考信息 -->