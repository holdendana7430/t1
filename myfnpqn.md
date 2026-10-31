代发 wailian999

TS:   new Date("2024-01-02")
来源：http://yq.muxihuayi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cc.9csxet.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://da.haigaiapp.cn

Ruby: Date.parse("2024-01-02")
来源：http://gt.huixinmuqiang.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ys.szxytkj.cn

[J04] 时间戳与日期互转
来源：http://ax.wgjwhj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dh.9csxet.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://il.gzmigu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zp.szxytkj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://iy.shtwfgs.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://si.shxzukj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jh.gzmigu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xo.shxzukj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://oq.huanxung.cn

[J05] 时间加减（加 7 天）
来源：http://jy.9csxet.cn

Py:   now + timedelta(days=7)
来源：http://rr.yuexingan06.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bh.colortex.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lz.521024.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gc.shtwfgs.cn

Java: LocalDate.now().plusDays(7)
来源：http://lt.lnxyls.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://te.huixiangedu.cn

Ruby: Time.now + 7 * 86400
来源：http://ra.lnxyls.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bk.jianghongdianzi.cn

[J06] 计算两时间之差
来源：http://aa.yuexingan06.cn

Py:   (end - start).total_seconds()
来源：http://ky.lnxyls.cn

PHP:  $end->diff($start)->days;
来源：http://wy.hahajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qs.shxzskj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cr.521024.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ug.chemitech.net.cn

Go:   end.Sub(start).Hours()
来源：http://ia.hahajie.cn

Ruby: end - start                 # 返回秒数
来源：http://vf.newstarts.cn

C#:   (end - start).TotalSeconds
来源：http://ns.huanxung.cn

[J07] 比较两个日期
来源：http://nb.huixinmuqiang.cn

Py:   d1 < d2;  d1 == d2
来源：http://ua.jianghongdianzi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qr.lnxyls.cn

JS:   d1.getTime() < d2.getTime()
来源：http://nk.huixinmuqiang.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gd.shtwfgs.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uq.shxzskj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://up.huixiangedu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lz.szsharing.cn

C#:   d1 < d2;  d1 == d2
来源：http://vl.shtwfgs.cn

[J08] 提取年月日与星期
来源：http://zf.haigaiapp.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yq.bookmarksfly.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ki.hahajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gi.nicolike.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ge.nszjky.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ep.asd995.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rs.gzmigu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nt.lnxyls.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://st.jianghongdianzi.cn

[J09] 时区处理
来源：http://dv.huanxung.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ps.szsharing.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mi.panjiajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xx.jianghongdianzi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yc.panjiajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yo.huanxung.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vj.521024.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xy.shxzskj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nu.shtwfgs.cn

[J10] 取今天 / 本月第一天
来源：http://av.haigaiapp.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wd.huixinmuqiang.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jt.yuexingan06.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://po.shxzskj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ab.shxzskj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jf.huixiangedu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zr.haigaiapp.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tk.lnxyls.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qa.szsharing.cn

================================================================================
来源：http://kn.jianghongdianzi.cn

K. JSON 与序列化
来源：http://uy.yuntaijiaju.cn

================================================================================
来源：http://ze.hnjuh.cn

[K01] 对象转 JSON 字符串
来源：http://lw.hnjuh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nw.shxzukj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cw.jctech888.com.cn

JS:   JSON.stringify(obj)
来源：http://bd.yuntaijiaju.cn

TS:   JSON.stringify(obj)
来源：http://wx.yuexingan06.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xi.bookmarksfly.cn

Go:   json.Marshal(obj)
来源：http://ub.nicolike.cn

Ruby: obj.to_json                                     // require "json"
来源：http://uv.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hg.szsharing.cn

[K02] JSON 字符串转对象
来源：http://kc.panjiajie.cn

Py:   json.loads(s)
来源：http://et.nszjky.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gp.wgjwhj.cn

JS:   JSON.parse(s)
来源：http://qz.lnxyls.cn

TS:   JSON.parse(s)
来源：http://xq.shxzukj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fz.bookmarksfly.cn

Go:   json.Unmarshal(data, &v)
来源：http://bn.yuexingan06.cn

Ruby: JSON.parse(s)
来源：http://cc.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lh.nszjky.cn

[K03] JSON 美化输出（带缩进）
来源：http://rt.szxytkj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sw.panjiajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qd.521024.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gn.panjiajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xf.shtwfgs.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sf.newstarts.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://po.lnxyls.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zz.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bm.muxihuayi.cn

[K04] 读取 JSON 文件
来源：http://mb.shxzukj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rz.huixinmuqiang.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kl.521024.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uh.shxzukj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vz.huixinmuqiang.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ug.nszjky.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ii.huanxung.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vs.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://np.lnxyls.cn

[K05] 深拷贝对象
来源：http://go.haigaiapp.cn

Py:   copy.deepcopy(obj)
来源：http://lq.hnjuh.cn

PHP:  unserialize(serialize($obj));
来源：http://qm.jianghongdianzi.cn

JS:   structuredClone(obj)
来源：http://hm.wgjwhj.cn

TS:   structuredClone(obj)
来源：http://ri.nszjky.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gj.huixiangedu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zr.gzmigu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kc.muxihuayi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yn.haigaiapp.cn

[K06] 解析 URL 查询串
来源：http://uz.hahajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tv.shtwfgs.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xw.asd995.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ir.nicolike.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tm.szsharing.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gs.colortex.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sw.szxytkj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cn.colortex.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qy.nicolike.cn

[K07] 进制转换
来源：http://vu.shxzukj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gm.yuexingan06.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hp.hahajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qu.huixiangedu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fn.hahajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://po.9csxet.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nn.muxihuayi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pw.muxihuayi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yf.panjiajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://vi.shxzskj.cn

Py:   pickle.dumps(obj)
来源：http://dl.szsharing.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ly.szsharing.cn

JS:   v8.serialize(obj)        // Node
来源：http://yd.huixinmuqiang.cn

TS:   v8.serialize(obj)        // Node
来源：http://yl.haigaiapp.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xa.colortex.cn

Go:   encoding/gob
来源：http://xb.huixinmuqiang.cn

Ruby: Marshal.dump(obj)
来源：http://hs.shxzukj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://oj.shxzukj.cn

================================================================================
来源：http://dm.shxzukj.cn

L. 网络请求
来源：http://oi.chemitech.net.cn

================================================================================
来源：http://fy.521024.cn

[L01] 发送 GET 请求
来源：http://zv.newstarts.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wg.wgjwhj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://aj.wgjwhj.cn

JS:   await fetch(url)
来源：http://at.jctech888.com.cn

TS:   await fetch(url)
来源：http://rf.shxzukj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kt.nszjky.cn

Go:   resp, err := http.Get(url)
来源：http://cr.9csxet.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://vz.asd995.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nw.nszjky.cn

[L02] 发送 POST JSON
来源：http://zb.bjjhwx.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nr.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://th.asd995.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kk.huixiangedu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://of.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ev.panjiajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wa.shxzukj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ac.muxihuayi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ui.9csxet.cn

[L03] 设置自定义请求头
来源：http://sk.szsharing.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xx.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zh.nszjky.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mq.nszjky.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mh.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://he.hahajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cl.nszjky.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bj.jctech888.com.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cc.hahajie.cn

[L04] 设置超时
来源：http://ht.huixinmuqiang.cn

Py:   requests.get(url, timeout=5)
来源：http://fz.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dq.nicolike.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nu.huanxung.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ak.jctech888.com.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fy.hahajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ss.szsharing.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ua.jctech888.com.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fc.shtwfgs.cn

[L05] 上传文件（multipart）
来源：http://va.szxytkj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qz.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hh.huanxung.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mc.hnjuh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://va.newstarts.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pk.jctech888.com.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://aq.hahajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gl.szsharing.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://un.521024.cn

[L06] 解析响应为 JSON
来源：http://up.gzmigu.cn

Py:   resp.json()
来源：http://wc.newstarts.cn

PHP:  json_decode($body, true);
来源：http://re.yuexingan06.cn

JS:   await resp.json()
来源：http://ke.huixinmuqiang.cn

TS:   await resp.json()
来源：http://nl.colortex.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://aw.jctech888.com.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rw.haigaiapp.cn

Ruby: JSON.parse(resp.body)
来源：http://zj.huixinmuqiang.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jr.521024.cn

[L07] 处理 HTTP 状态码
来源：http://bc.shxzukj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ef.jianghongdianzi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uu.colortex.cn

JS:   resp.ok;  resp.status
来源：http://zn.bookmarksfly.cn

TS:   resp.ok;  resp.status
来源：http://zw.bookmarksfly.cn

Java: resp.statusCode()
来源：http://jx.9csxet.cn

Go:   resp.StatusCode
来源：http://vy.yuexingan06.cn

Ruby: resp.code.to_i
来源：http://bs.lnxyls.cn

C#:   (int)resp.StatusCode
来源：http://fi.shtwfgs.cn

[L08] 并发请求多个地址
来源：http://yb.yuntaijiaju.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pe.muxihuayi.cn

PHP:  curl_multi_init() 系列
来源：http://nt.huixiangedu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jn.shxzukj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ei.huixiangedu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ny.shtwfgs.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ko.9csxet.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cr.colortex.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zq.hnjuh.cn

================================================================================
来源：http://lg.jctech888.com.cn

M. 命令行 / 进程 / 环境
来源：http://gz.gzmigu.cn

================================================================================
来源：http://xl.huanxung.cn

[M01] 读取命令行参数
来源：http://zo.huixinmuqiang.cn

Py:   sys.argv[1:]
来源：http://dy.szsharing.cn

PHP:  $argv;  $argc;
来源：http://xw.szxytkj.cn

JS:   process.argv.slice(2)
来源：http://re.hahajie.cn

TS:   process.argv.slice(2)
来源：http://gl.nicolike.cn

Java: args 数组（main 方法参数）
来源：http://xc.jctech888.com.cn

Go:   os.Args[1:]
来源：http://sd.lnxyls.cn

Ruby: ARGV
来源：http://ni.yuntaijiaju.cn

C#:   args 数组（Main 方法参数）
来源：http://mb.shxzskj.cn

[M02] 读取环境变量
来源：http://dk.huixiangedu.cn

Py:   os.environ.get("HOME")
来源：http://gy.nicolike.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mz.jctech888.com.cn

JS:   process.env.HOME
来源：http://sv.hnjuh.cn

TS:   process.env.HOME
来源：http://kq.gzmigu.cn

Java: System.getenv("HOME")
来源：http://yx.asd995.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xl.wgjwhj.cn

Ruby: ENV["HOME"]
来源：http://xm.521024.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hn.wgjwhj.cn

[M03] 执行外部命令
来源：http://yf.nszjky.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vn.521024.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hq.huixinmuqiang.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hs.bjjhwx.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ss.panjiajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wn.yuntaijiaju.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://tc.haigaiapp.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ae.shtwfgs.cn

C#:   Process.Start("ls", "-l");
来源：http://sn.huixinmuqiang.cn

[M04] 获取当前工作目录
来源：http://ep.panjiajie.cn

Py:   os.getcwd()
来源：http://da.gzmigu.cn

PHP:  getcwd();
来源：http://eg.colortex.cn

JS:   process.cwd()
来源：http://rg.shxzukj.cn

TS:   process.cwd()
来源：http://wi.9csxet.cn

Java: Path.of("").toAbsolutePath()
来源：http://zi.shxzukj.cn

Go:   os.Getwd()
来源：http://fj.gzmigu.cn

Ruby: Dir.pwd
来源：http://tb.muxihuayi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ss.hnjuh.cn

[M05] 设置退出码
来源：http://qr.jctech888.com.cn

Py:   sys.exit(1)
来源：http://dn.jctech888.com.cn

PHP:  exit(1);
来源：http://at.lnxyls.cn

JS:   process.exit(1)
来源：http://xl.yuntaijiaju.cn

TS:   process.exit(1)
来源：http://kj.shxzukj.cn

Java: System.exit(1)
来源：http://zd.bookmarksfly.cn

Go:   os.Exit(1)
来源：http://za.huixinmuqiang.cn

Ruby: exit 1
来源：http://il.shxzukj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yj.shxzukj.cn

[M06] 向标准错误输出
来源：http://iw.lnxyls.cn

Py:   print("err", file=sys.stderr)
来源：http://un.jianghongdianzi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://sb.hnjuh.cn

JS:   console.error("err")
来源：http://np.hnjuh.cn

TS:   console.error("err")
来源：http://va.shxzskj.cn

Java: System.err.println("err")
来源：http://tt.gzmigu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ug.bjjhwx.cn

Ruby: warn "err"
来源：http://th.hahajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://cw.asd995.cn

[M07] 判断是否为主入口
来源：http://nn.jianghongdianzi.cn

Py:   if __name__ == "__main__":
来源：http://ox.huixiangedu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gy.shxzukj.cn

JS:   require.main === module
来源：http://dl.szxytkj.cn

TS:   require.main === module
来源：http://tr.yuntaijiaju.cn

Java: public static void main(String[] args)
来源：http://gl.szxytkj.cn

Go:   func main()
来源：http://fx.muxihuayi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zc.nicolike.cn

C#:   static void Main(string[] args)
来源：http://tz.hahajie.cn

[M08] 获取系统与运行时信息
来源：http://ix.colortex.cn

Py:   platform.system();  platform.python_version()
来源：http://vn.521024.cn

PHP:  PHP_OS;  phpversion();
来源：http://ay.bjjhwx.cn

JS:   process.platform;  process.version
来源：http://im.nicolike.cn

TS:   process.platform;  process.version
来源：http://fi.huanxung.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lu.huanxung.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://jo.asd995.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fa.lnxyls.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gm.colortex.cn

================================================================================
来源：http://dl.jctech888.com.cn

N. 数据结构与算法
来源：http://ne.colortex.cn

================================================================================
来源：http://dx.lnxyls.cn

[N01] 二分查找（有序数组）
来源：http://fj.9csxet.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ef.szxytkj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rz.bjjhwx.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ei.szxytkj.cn


<!-- 参考信息 -->