代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qu.hnjuh.cn

[J04] 时间戳与日期互转
来源：http://nv.lnxyls.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uo.panjiajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xl.yuntaijiaju.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wh.szxytkj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://nc.shxzskj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ya.shtwfgs.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sp.lnxyls.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yj.haigaiapp.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qw.gzmigu.cn

[J05] 时间加减（加 7 天）
来源：http://so.shtwfgs.cn

Py:   now + timedelta(days=7)
来源：http://ie.shtwfgs.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://we.haigaiapp.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lw.huixiangedu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ob.szxytkj.cn

Java: LocalDate.now().plusDays(7)
来源：http://ce.haigaiapp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zw.wgjwhj.cn

Ruby: Time.now + 7 * 86400
来源：http://bn.bjjhwx.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ec.yuexingan06.cn

[J06] 计算两时间之差
来源：http://zk.jctech888.com.cn

Py:   (end - start).total_seconds()
来源：http://wl.colortex.cn

PHP:  $end->diff($start)->days;
来源：http://bx.9csxet.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nd.bjjhwx.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jv.szsharing.cn

Java: Duration.between(start, end).toSeconds()
来源：http://yv.bookmarksfly.cn

Go:   end.Sub(start).Hours()
来源：http://vz.yuexingan06.cn

Ruby: end - start                 # 返回秒数
来源：http://op.bookmarksfly.cn

C#:   (end - start).TotalSeconds
来源：http://ju.wgjwhj.cn

[J07] 比较两个日期
来源：http://ah.lnxyls.cn

Py:   d1 < d2;  d1 == d2
来源：http://ko.nicolike.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yg.huixinmuqiang.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kv.bjjhwx.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hy.lnxyls.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yd.hahajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kx.huixiangedu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ig.chemitech.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://uh.bjjhwx.cn

[J08] 提取年月日与星期
来源：http://dm.huixinmuqiang.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qn.huanxung.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ez.szsharing.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bi.huanxung.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vv.hahajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qn.shxzskj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nx.muxihuayi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kc.nicolike.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jf.shxzskj.cn

[J09] 时区处理
来源：http://qc.szsharing.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kk.hahajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zs.szsharing.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hj.szsharing.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ti.chemitech.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xm.lnxyls.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ns.521024.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://rw.jianghongdianzi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bb.asd995.cn

[J10] 取今天 / 本月第一天
来源：http://nz.shtwfgs.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jv.lnxyls.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xz.muxihuayi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bj.colortex.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iv.huanxung.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uq.szxytkj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bn.yuntaijiaju.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tx.yuexingan06.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vn.wgjwhj.cn

================================================================================
来源：http://oc.lnxyls.cn

K. JSON 与序列化
来源：http://au.shxzskj.cn

================================================================================
来源：http://ib.hnjuh.cn

[K01] 对象转 JSON 字符串
来源：http://yu.hnjuh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ba.bookmarksfly.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qq.yuexingan06.cn

JS:   JSON.stringify(obj)
来源：http://mc.huixiangedu.cn

TS:   JSON.stringify(obj)
来源：http://pp.huixinmuqiang.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jt.yuexingan06.cn

Go:   json.Marshal(obj)
来源：http://vo.lnxyls.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nc.szxytkj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qa.haigaiapp.cn

[K02] JSON 字符串转对象
来源：http://zr.jctech888.com.cn

Py:   json.loads(s)
来源：http://fi.panjiajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://va.lnxyls.cn

JS:   JSON.parse(s)
来源：http://mu.huixinmuqiang.cn

TS:   JSON.parse(s)
来源：http://zj.panjiajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vq.yuexingan06.cn

Go:   json.Unmarshal(data, &v)
来源：http://hs.szxytkj.cn

Ruby: JSON.parse(s)
来源：http://lg.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ol.muxihuayi.cn

[K03] JSON 美化输出（带缩进）
来源：http://dz.panjiajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xq.nszjky.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xm.asd995.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qk.shxzskj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nn.lnxyls.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bk.nicolike.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://py.colortex.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rf.hahajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ts.colortex.cn

[K04] 读取 JSON 文件
来源：http://lm.muxihuayi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hy.huixinmuqiang.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lw.wgjwhj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cn.huanxung.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rl.szxytkj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qp.asd995.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cd.hahajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dr.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rq.wgjwhj.cn

[K05] 深拷贝对象
来源：http://sh.muxihuayi.cn

Py:   copy.deepcopy(obj)
来源：http://tr.lnxyls.cn

PHP:  unserialize(serialize($obj));
来源：http://oo.521024.cn

JS:   structuredClone(obj)
来源：http://zj.haigaiapp.cn

TS:   structuredClone(obj)
来源：http://hn.shxzskj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://cl.newstarts.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hv.hahajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://by.asd995.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://uk.gzmigu.cn

[K06] 解析 URL 查询串
来源：http://ys.jctech888.com.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://na.bjjhwx.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://as.bjjhwx.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jj.bjjhwx.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wv.shtwfgs.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tq.bjjhwx.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rn.shtwfgs.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yn.shxzukj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sd.asd995.cn

[K07] 进制转换
来源：http://xr.nicolike.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://om.haigaiapp.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ka.shxzskj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ia.shtwfgs.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tx.9csxet.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lw.bookmarksfly.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sf.lnxyls.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://np.lnxyls.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pe.chemitech.net.cn

[K08] 二进制序列化（非 JSON）
来源：http://sv.szxytkj.cn

Py:   pickle.dumps(obj)
来源：http://tv.yuexingan06.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fj.jianghongdianzi.cn

JS:   v8.serialize(obj)        // Node
来源：http://qu.huanxung.cn

TS:   v8.serialize(obj)        // Node
来源：http://sg.shtwfgs.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tj.gzmigu.cn

Go:   encoding/gob
来源：http://ad.nszjky.cn

Ruby: Marshal.dump(obj)
来源：http://ab.szxytkj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fs.asd995.cn

================================================================================
来源：http://qx.gzmigu.cn

L. 网络请求
来源：http://mi.wgjwhj.cn

================================================================================
来源：http://ax.szsharing.cn

[L01] 发送 GET 请求
来源：http://lq.colortex.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ni.asd995.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bp.yuntaijiaju.cn

JS:   await fetch(url)
来源：http://yt.szxytkj.cn

TS:   await fetch(url)
来源：http://wp.shtwfgs.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vh.jctech888.com.cn

Go:   resp, err := http.Get(url)
来源：http://nc.muxihuayi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://en.gzmigu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://he.shxzukj.cn

[L02] 发送 POST JSON
来源：http://yz.shxzskj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://kg.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qg.huixiangedu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cf.colortex.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jk.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kz.colortex.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ki.panjiajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mw.shxzskj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://eo.yuexingan06.cn

[L03] 设置自定义请求头
来源：http://ux.muxihuayi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kg.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ar.yuexingan06.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yf.shxzukj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pv.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://md.huixiangedu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xd.521024.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ni.szsharing.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ra.szsharing.cn

[L04] 设置超时
来源：http://dt.bookmarksfly.cn

Py:   requests.get(url, timeout=5)
来源：http://av.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://im.haigaiapp.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lf.hnjuh.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ly.huixinmuqiang.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qx.jianghongdianzi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zi.yuexingan06.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ej.newstarts.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://or.shxzukj.cn

[L05] 上传文件（multipart）
来源：http://qe.yuntaijiaju.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mb.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mc.haigaiapp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lh.wgjwhj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cm.hahajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fg.bjjhwx.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hv.yuexingan06.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nd.bjjhwx.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ga.jianghongdianzi.cn

[L06] 解析响应为 JSON
来源：http://fe.hnjuh.cn

Py:   resp.json()
来源：http://dk.wgjwhj.cn

PHP:  json_decode($body, true);
来源：http://sv.huixiangedu.cn

JS:   await resp.json()
来源：http://gx.nszjky.cn

TS:   await resp.json()
来源：http://hg.hnjuh.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xp.newstarts.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kr.chemitech.net.cn

Ruby: JSON.parse(resp.body)
来源：http://em.huanxung.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ub.yuntaijiaju.cn

[L07] 处理 HTTP 状态码
来源：http://oc.bjjhwx.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://go.huixiangedu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hv.jianghongdianzi.cn

JS:   resp.ok;  resp.status
来源：http://qa.huixinmuqiang.cn

TS:   resp.ok;  resp.status
来源：http://gx.521024.cn

Java: resp.statusCode()
来源：http://nc.yuntaijiaju.cn

Go:   resp.StatusCode
来源：http://pv.wgjwhj.cn

Ruby: resp.code.to_i
来源：http://rd.wgjwhj.cn

C#:   (int)resp.StatusCode
来源：http://st.panjiajie.cn

[L08] 并发请求多个地址
来源：http://xr.bookmarksfly.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yc.huixiangedu.cn

PHP:  curl_multi_init() 系列
来源：http://tb.nszjky.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gp.shxzskj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tk.hnjuh.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xl.newstarts.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ti.wgjwhj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sv.colortex.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wi.jianghongdianzi.cn

================================================================================
来源：http://ty.nicolike.cn

M. 命令行 / 进程 / 环境
来源：http://vx.huixiangedu.cn

================================================================================
来源：http://zo.gzmigu.cn

[M01] 读取命令行参数
来源：http://kz.nszjky.cn

Py:   sys.argv[1:]
来源：http://wu.yuntaijiaju.cn

PHP:  $argv;  $argc;
来源：http://xo.szxytkj.cn

JS:   process.argv.slice(2)
来源：http://ee.yuexingan06.cn

TS:   process.argv.slice(2)
来源：http://yd.chemitech.net.cn

Java: args 数组（main 方法参数）
来源：http://yi.nszjky.cn

Go:   os.Args[1:]
来源：http://ur.huanxung.cn

Ruby: ARGV
来源：http://xl.nszjky.cn

C#:   args 数组（Main 方法参数）
来源：http://bt.shxzukj.cn

[M02] 读取环境变量
来源：http://eg.chemitech.net.cn

Py:   os.environ.get("HOME")
来源：http://ps.shxzukj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vc.panjiajie.cn

JS:   process.env.HOME
来源：http://cs.szsharing.cn

TS:   process.env.HOME
来源：http://jc.haigaiapp.cn

Java: System.getenv("HOME")
来源：http://pi.yuntaijiaju.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yd.shxzskj.cn

Ruby: ENV["HOME"]
来源：http://ae.huanxung.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tl.muxihuayi.cn

[M03] 执行外部命令
来源：http://re.shtwfgs.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gv.szsharing.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lc.shxzskj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nw.szxytkj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jk.panjiajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uu.9csxet.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hr.nszjky.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pa.huanxung.cn

C#:   Process.Start("ls", "-l");
来源：http://fw.huixiangedu.cn

[M04] 获取当前工作目录
来源：http://xn.shtwfgs.cn

Py:   os.getcwd()
来源：http://bt.huixiangedu.cn

PHP:  getcwd();
来源：http://cs.szsharing.cn

JS:   process.cwd()
来源：http://yx.nicolike.cn

TS:   process.cwd()
来源：http://wn.bookmarksfly.cn

Java: Path.of("").toAbsolutePath()
来源：http://dj.jctech888.com.cn

Go:   os.Getwd()
来源：http://ld.nszjky.cn

Ruby: Dir.pwd
来源：http://fe.lnxyls.cn

C#:   Directory.GetCurrentDirectory()
来源：http://bd.shxzukj.cn

[M05] 设置退出码
来源：http://ph.jctech888.com.cn

Py:   sys.exit(1)
来源：http://bv.colortex.cn

PHP:  exit(1);
来源：http://ez.9csxet.cn

JS:   process.exit(1)
来源：http://fv.muxihuayi.cn

TS:   process.exit(1)
来源：http://vk.asd995.cn

Java: System.exit(1)
来源：http://wl.huixinmuqiang.cn

Go:   os.Exit(1)
来源：http://fo.szxytkj.cn

Ruby: exit 1
来源：http://xk.szxytkj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nj.huanxung.cn

[M06] 向标准错误输出
来源：http://mx.nicolike.cn

Py:   print("err", file=sys.stderr)
来源：http://om.wgjwhj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qz.szsharing.cn

JS:   console.error("err")
来源：http://nu.asd995.cn

TS:   console.error("err")
来源：http://wa.huanxung.cn

Java: System.err.println("err")
来源：http://zg.9csxet.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rz.szsharing.cn

Ruby: warn "err"
来源：http://ob.colortex.cn

C#:   Console.Error.WriteLine("err")
来源：http://tx.szxytkj.cn

[M07] 判断是否为主入口
来源：http://cv.wgjwhj.cn

Py:   if __name__ == "__main__":
来源：http://gw.9csxet.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gq.hnjuh.cn

JS:   require.main === module
来源：http://zw.asd995.cn

TS:   require.main === module
来源：http://lz.shxzukj.cn

Java: public static void main(String[] args)
来源：http://ju.jctech888.com.cn

Go:   func main()
来源：http://an.bookmarksfly.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ls.bjjhwx.cn

C#:   static void Main(string[] args)
来源：http://ei.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://rc.hahajie.cn

Py:   platform.system();  platform.python_version()
来源：http://jq.panjiajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://qh.shtwfgs.cn

JS:   process.platform;  process.version
来源：http://lm.huanxung.cn

TS:   process.platform;  process.version
来源：http://ho.szxytkj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wz.szxytkj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zj.newstarts.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xo.newstarts.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bu.521024.cn

================================================================================
来源：http://ir.yuntaijiaju.cn

N. 数据结构与算法
来源：http://vk.gzmigu.cn

================================================================================
来源：http://yg.lnxyls.cn

[N01] 二分查找（有序数组）
来源：http://ha.9csxet.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vg.huixiangedu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jy.muxihuayi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hf.huixinmuqiang.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ks.yuntaijiaju.cn

Java: Arrays.binarySearch(arr, x)
来源：http://tk.bookmarksfly.cn

Go:   sort.SearchInts(arr, x)
来源：http://tq.huixinmuqiang.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jr.haigaiapp.cn


<!-- 参考信息 -->