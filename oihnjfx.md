代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hy.muxihuayi.cn

[J04] 时间戳与日期互转
来源：http://wm.szsharing.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dq.9csxet.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wm.bjjhwx.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xi.hahajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://sm.gzmigu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bf.shtwfgs.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://on.jianghongdianzi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hl.colortex.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ix.szxytkj.cn

[J05] 时间加减（加 7 天）
来源：http://mh.hnjuh.cn

Py:   now + timedelta(days=7)
来源：http://cw.yuntaijiaju.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://io.521024.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://df.bjjhwx.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://so.shxzukj.cn

Java: LocalDate.now().plusDays(7)
来源：http://fg.newstarts.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://va.wgjwhj.cn

Ruby: Time.now + 7 * 86400
来源：http://xr.chemitech.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ku.colortex.cn

[J06] 计算两时间之差
来源：http://ej.hahajie.cn

Py:   (end - start).total_seconds()
来源：http://vh.chemitech.net.cn

PHP:  $end->diff($start)->days;
来源：http://av.huixinmuqiang.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ta.jianghongdianzi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ff.jianghongdianzi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qj.jctech888.com.cn

Go:   end.Sub(start).Hours()
来源：http://mc.panjiajie.cn

Ruby: end - start                 # 返回秒数
来源：http://vx.huixinmuqiang.cn

C#:   (end - start).TotalSeconds
来源：http://hq.panjiajie.cn

[J07] 比较两个日期
来源：http://pq.huixinmuqiang.cn

Py:   d1 < d2;  d1 == d2
来源：http://mp.shxzskj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kk.shxzskj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bj.yuexingan06.cn

TS:   d1.getTime() < d2.getTime()
来源：http://om.521024.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wl.huixinmuqiang.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://oj.huixiangedu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gw.jctech888.com.cn

C#:   d1 < d2;  d1 == d2
来源：http://ts.jianghongdianzi.cn

[J08] 提取年月日与星期
来源：http://zg.jctech888.com.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wc.hnjuh.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://np.muxihuayi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rw.panjiajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dr.huixinmuqiang.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jd.chemitech.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jz.szxytkj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ah.9csxet.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fh.yuexingan06.cn

[J09] 时区处理
来源：http://jz.521024.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cx.asd995.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rv.huixiangedu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ps.szsharing.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nc.9csxet.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hf.newstarts.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lo.huixiangedu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://dh.haigaiapp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hv.lnxyls.cn

[J10] 取今天 / 本月第一天
来源：http://zk.gzmigu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xa.9csxet.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jz.nicolike.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tx.haigaiapp.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mb.yuntaijiaju.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sr.yuexingan06.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bs.nicolike.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uc.bjjhwx.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gd.bookmarksfly.cn

================================================================================
来源：http://wt.muxihuayi.cn

K. JSON 与序列化
来源：http://ew.chemitech.net.cn

================================================================================
来源：http://mj.hnjuh.cn

[K01] 对象转 JSON 字符串
来源：http://br.szxytkj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lr.muxihuayi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tn.jctech888.com.cn

JS:   JSON.stringify(obj)
来源：http://xt.newstarts.cn

TS:   JSON.stringify(obj)
来源：http://un.nszjky.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gv.yuexingan06.cn

Go:   json.Marshal(obj)
来源：http://jj.szxytkj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qj.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://mh.hnjuh.cn

[K02] JSON 字符串转对象
来源：http://md.shxzukj.cn

Py:   json.loads(s)
来源：http://rp.shtwfgs.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fk.lnxyls.cn

JS:   JSON.parse(s)
来源：http://vn.muxihuayi.cn

TS:   JSON.parse(s)
来源：http://ii.bjjhwx.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zv.huixiangedu.cn

Go:   json.Unmarshal(data, &v)
来源：http://ru.muxihuayi.cn

Ruby: JSON.parse(s)
来源：http://am.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ij.asd995.cn

[K03] JSON 美化输出（带缩进）
来源：http://mx.asd995.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ly.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vg.haigaiapp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://lx.newstarts.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ii.nicolike.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ue.huanxung.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kn.szsharing.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wg.nszjky.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ej.521024.cn

[K04] 读取 JSON 文件
来源：http://wb.asd995.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mx.9csxet.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rl.shtwfgs.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vs.yuntaijiaju.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qo.colortex.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mj.gzmigu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gc.wgjwhj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wm.asd995.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sd.panjiajie.cn

[K05] 深拷贝对象
来源：http://dz.lnxyls.cn

Py:   copy.deepcopy(obj)
来源：http://jo.jctech888.com.cn

PHP:  unserialize(serialize($obj));
来源：http://zx.colortex.cn

JS:   structuredClone(obj)
来源：http://vr.yuntaijiaju.cn

TS:   structuredClone(obj)
来源：http://dj.shxzskj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://is.huanxung.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gj.colortex.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ex.jianghongdianzi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://de.panjiajie.cn

[K06] 解析 URL 查询串
来源：http://lj.yuexingan06.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ig.jctech888.com.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gd.colortex.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cr.gzmigu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bl.wgjwhj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xg.haigaiapp.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://nf.wgjwhj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rx.huixinmuqiang.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://el.asd995.cn

[K07] 进制转换
来源：http://nh.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://if.nicolike.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gk.521024.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://br.shxzskj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yl.huixiangedu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lv.hnjuh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lv.shxzukj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tp.shxzskj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nx.wgjwhj.cn

[K08] 二进制序列化（非 JSON）
来源：http://lf.yuntaijiaju.cn

Py:   pickle.dumps(obj)
来源：http://vg.jianghongdianzi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zv.hahajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://bx.lnxyls.cn

TS:   v8.serialize(obj)        // Node
来源：http://vi.huixiangedu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://up.chemitech.net.cn

Go:   encoding/gob
来源：http://ld.muxihuayi.cn

Ruby: Marshal.dump(obj)
来源：http://tl.panjiajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uv.huixinmuqiang.cn

================================================================================
来源：http://lm.shxzukj.cn

L. 网络请求
来源：http://mz.muxihuayi.cn

================================================================================
来源：http://iv.nszjky.cn

[L01] 发送 GET 请求
来源：http://vz.gzmigu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qq.jianghongdianzi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ns.9csxet.cn

JS:   await fetch(url)
来源：http://in.chemitech.net.cn

TS:   await fetch(url)
来源：http://ip.muxihuayi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yv.colortex.cn

Go:   resp, err := http.Get(url)
来源：http://vx.colortex.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://kb.asd995.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wa.521024.cn

[L02] 发送 POST JSON
来源：http://gy.bookmarksfly.cn

Py:   requests.post(url, json={"a": 1})
来源：http://oa.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wp.newstarts.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cu.nicolike.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jh.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sn.newstarts.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://co.shtwfgs.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kd.lnxyls.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mj.hahajie.cn

[L03] 设置自定义请求头
来源：http://jo.newstarts.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jw.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mf.hnjuh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sh.bjjhwx.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pu.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://le.hnjuh.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ac.lnxyls.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kk.bookmarksfly.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://on.lnxyls.cn

[L04] 设置超时
来源：http://fg.huixiangedu.cn

Py:   requests.get(url, timeout=5)
来源：http://vx.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ht.yuexingan06.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ws.shxzskj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ug.shxzskj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jg.panjiajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fi.shxzskj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://px.wgjwhj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ft.muxihuayi.cn

[L05] 上传文件（multipart）
来源：http://ml.shxzskj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qz.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bt.jianghongdianzi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gj.nicolike.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://aj.nicolike.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wv.panjiajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kt.hahajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gn.shtwfgs.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fx.hnjuh.cn

[L06] 解析响应为 JSON
来源：http://ot.lnxyls.cn

Py:   resp.json()
来源：http://cd.colortex.cn

PHP:  json_decode($body, true);
来源：http://vi.shxzskj.cn

JS:   await resp.json()
来源：http://vi.shxzskj.cn

TS:   await resp.json()
来源：http://hn.bookmarksfly.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ai.shtwfgs.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jn.nicolike.cn

Ruby: JSON.parse(resp.body)
来源：http://dw.muxihuayi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tp.huixinmuqiang.cn

[L07] 处理 HTTP 状态码
来源：http://kl.9csxet.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ov.huanxung.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kw.yuexingan06.cn

JS:   resp.ok;  resp.status
来源：http://cp.muxihuayi.cn

TS:   resp.ok;  resp.status
来源：http://qb.wgjwhj.cn

Java: resp.statusCode()
来源：http://ff.newstarts.cn

Go:   resp.StatusCode
来源：http://sd.lnxyls.cn

Ruby: resp.code.to_i
来源：http://qk.shtwfgs.cn

C#:   (int)resp.StatusCode
来源：http://yh.521024.cn

[L08] 并发请求多个地址
来源：http://yh.wgjwhj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://iy.bookmarksfly.cn

PHP:  curl_multi_init() 系列
来源：http://dt.asd995.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://in.szxytkj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://et.bjjhwx.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fw.hnjuh.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pi.yuntaijiaju.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sn.jctech888.com.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lj.shxzukj.cn

================================================================================
来源：http://fn.huixiangedu.cn

M. 命令行 / 进程 / 环境
来源：http://mp.lnxyls.cn

================================================================================
来源：http://ll.bjjhwx.cn

[M01] 读取命令行参数
来源：http://xr.yuntaijiaju.cn

Py:   sys.argv[1:]
来源：http://sq.yuntaijiaju.cn

PHP:  $argv;  $argc;
来源：http://xc.haigaiapp.cn

JS:   process.argv.slice(2)
来源：http://hz.nicolike.cn

TS:   process.argv.slice(2)
来源：http://eh.521024.cn

Java: args 数组（main 方法参数）
来源：http://je.shxzskj.cn

Go:   os.Args[1:]
来源：http://to.huixiangedu.cn

Ruby: ARGV
来源：http://dl.jianghongdianzi.cn

C#:   args 数组（Main 方法参数）
来源：http://eg.haigaiapp.cn

[M02] 读取环境变量
来源：http://oo.hahajie.cn

Py:   os.environ.get("HOME")
来源：http://wv.gzmigu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pz.hahajie.cn

JS:   process.env.HOME
来源：http://lt.jctech888.com.cn

TS:   process.env.HOME
来源：http://st.huanxung.cn

Java: System.getenv("HOME")
来源：http://tx.shtwfgs.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ia.hahajie.cn

Ruby: ENV["HOME"]
来源：http://iu.bookmarksfly.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ts.szsharing.cn

[M03] 执行外部命令
来源：http://ba.nicolike.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jo.lnxyls.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xp.muxihuayi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://uu.newstarts.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ws.jianghongdianzi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://af.bjjhwx.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ae.jctech888.com.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rc.szxytkj.cn

C#:   Process.Start("ls", "-l");
来源：http://qv.hahajie.cn

[M04] 获取当前工作目录
来源：http://he.shxzukj.cn

Py:   os.getcwd()
来源：http://fl.asd995.cn

PHP:  getcwd();
来源：http://my.gzmigu.cn

JS:   process.cwd()
来源：http://eb.szxytkj.cn

TS:   process.cwd()
来源：http://hs.shxzukj.cn

Java: Path.of("").toAbsolutePath()
来源：http://ij.shtwfgs.cn

Go:   os.Getwd()
来源：http://eo.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://fh.yuntaijiaju.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jianghongdianzi.cn

[M05] 设置退出码
来源：http://vx.gzmigu.cn

Py:   sys.exit(1)
来源：http://nx.9csxet.cn

PHP:  exit(1);
来源：http://gr.szxytkj.cn

JS:   process.exit(1)
来源：http://vl.huixiangedu.cn

TS:   process.exit(1)
来源：http://lx.panjiajie.cn

Java: System.exit(1)
来源：http://vi.szxytkj.cn

Go:   os.Exit(1)
来源：http://tc.haigaiapp.cn

Ruby: exit 1
来源：http://fo.szsharing.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qk.huixiangedu.cn

[M06] 向标准错误输出
来源：http://ls.colortex.cn

Py:   print("err", file=sys.stderr)
来源：http://kf.wgjwhj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bv.lnxyls.cn

JS:   console.error("err")
来源：http://mm.chemitech.net.cn

TS:   console.error("err")
来源：http://lx.newstarts.cn

Java: System.err.println("err")
来源：http://ic.shxzskj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kz.jctech888.com.cn

Ruby: warn "err"
来源：http://zg.szxytkj.cn

C#:   Console.Error.WriteLine("err")
来源：http://dh.huixinmuqiang.cn

[M07] 判断是否为主入口
来源：http://pc.wgjwhj.cn

Py:   if __name__ == "__main__":
来源：http://iq.bjjhwx.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://sw.jctech888.com.cn

JS:   require.main === module
来源：http://xt.szxytkj.cn

TS:   require.main === module
来源：http://ja.nicolike.cn

Java: public static void main(String[] args)
来源：http://tz.nicolike.cn

Go:   func main()
来源：http://ei.shxzskj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xf.huixiangedu.cn

C#:   static void Main(string[] args)
来源：http://iz.huanxung.cn

[M08] 获取系统与运行时信息
来源：http://vs.shxzukj.cn

Py:   platform.system();  platform.python_version()
来源：http://gw.lnxyls.cn

PHP:  PHP_OS;  phpversion();
来源：http://se.huanxung.cn

JS:   process.platform;  process.version
来源：http://gb.yuntaijiaju.cn

TS:   process.platform;  process.version
来源：http://ds.gzmigu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wm.szxytkj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://by.lnxyls.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://oz.gzmigu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://oy.wgjwhj.cn

================================================================================
来源：http://bz.shxzukj.cn

N. 数据结构与算法
来源：http://rp.newstarts.cn

================================================================================
来源：http://no.panjiajie.cn

[N01] 二分查找（有序数组）
来源：http://dh.gzmigu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gx.huanxung.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rp.panjiajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bz.shxzskj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dl.haigaiapp.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ng.huixinmuqiang.cn

Go:   sort.SearchInts(arr, x)
来源：http://jv.yuexingan06.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://co.huanxung.cn


<!-- 参考信息 -->