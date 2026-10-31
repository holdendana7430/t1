代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lq.bjjhwx.cn

[J04] 时间戳与日期互转
来源：http://oh.bookmarksfly.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mk.gzmigu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nv.9csxet.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qp.bookmarksfly.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zy.521024.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ce.huanxung.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ee.hahajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ag.huanxung.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zh.colortex.cn

[J05] 时间加减（加 7 天）
来源：http://vk.haigaiapp.cn

Py:   now + timedelta(days=7)
来源：http://jo.chemitech.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xv.panjiajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ja.521024.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zx.huanxung.cn

Java: LocalDate.now().plusDays(7)
来源：http://fe.521024.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pr.bjjhwx.cn

Ruby: Time.now + 7 * 86400
来源：http://gj.chemitech.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zu.yuntaijiaju.cn

[J06] 计算两时间之差
来源：http://on.gzmigu.cn

Py:   (end - start).total_seconds()
来源：http://pu.nszjky.cn

PHP:  $end->diff($start)->days;
来源：http://eo.huixiangedu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://go.yuntaijiaju.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mu.9csxet.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jy.chemitech.net.cn

Go:   end.Sub(start).Hours()
来源：http://fp.yuntaijiaju.cn

Ruby: end - start                 # 返回秒数
来源：http://ow.jctech888.com.cn

C#:   (end - start).TotalSeconds
来源：http://gz.colortex.cn

[J07] 比较两个日期
来源：http://tv.haigaiapp.cn

Py:   d1 < d2;  d1 == d2
来源：http://vp.chemitech.net.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zq.huanxung.cn

JS:   d1.getTime() < d2.getTime()
来源：http://dp.huixinmuqiang.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fz.9csxet.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xa.jctech888.com.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vh.newstarts.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qi.nszjky.cn

C#:   d1 < d2;  d1 == d2
来源：http://jl.szxytkj.cn

[J08] 提取年月日与星期
来源：http://ng.shtwfgs.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ro.hnjuh.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://en.newstarts.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gt.shxzukj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hb.jctech888.com.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://to.shxzukj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://au.huanxung.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cz.huixinmuqiang.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ky.hahajie.cn

[J09] 时区处理
来源：http://ok.asd995.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rl.huixiangedu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://eu.hnjuh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bd.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ms.shtwfgs.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bw.lnxyls.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lf.muxihuayi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://kk.huanxung.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yc.shxzskj.cn

[J10] 取今天 / 本月第一天
来源：http://gw.hnjuh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xj.wgjwhj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pw.gzmigu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ka.hnjuh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://py.bjjhwx.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mc.muxihuayi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ur.colortex.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ih.jctech888.com.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://by.haigaiapp.cn

================================================================================
来源：http://up.asd995.cn

K. JSON 与序列化
来源：http://jg.huanxung.cn

================================================================================
来源：http://fv.haigaiapp.cn

[K01] 对象转 JSON 字符串
来源：http://jc.muxihuayi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mh.huanxung.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lt.shxzskj.cn

JS:   JSON.stringify(obj)
来源：http://as.huixiangedu.cn

TS:   JSON.stringify(obj)
来源：http://je.szsharing.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ix.jianghongdianzi.cn

Go:   json.Marshal(obj)
来源：http://ly.szxytkj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://yc.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://no.asd995.cn

[K02] JSON 字符串转对象
来源：http://py.jianghongdianzi.cn

Py:   json.loads(s)
来源：http://nk.hahajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ef.hnjuh.cn

JS:   JSON.parse(s)
来源：http://kc.9csxet.cn

TS:   JSON.parse(s)
来源：http://wz.nicolike.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nl.panjiajie.cn

Go:   json.Unmarshal(data, &v)
来源：http://tl.jctech888.com.cn

Ruby: JSON.parse(s)
来源：http://yt.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tz.nszjky.cn

[K03] JSON 美化输出（带缩进）
来源：http://lt.szxytkj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tq.haigaiapp.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hv.muxihuayi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jw.asd995.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gr.huanxung.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://br.lnxyls.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sk.jianghongdianzi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://lz.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uk.shxzukj.cn

[K04] 读取 JSON 文件
来源：http://my.nszjky.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nl.hahajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zy.yuntaijiaju.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://in.chemitech.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nc.colortex.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ij.9csxet.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kf.huixiangedu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://eq.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yb.yuntaijiaju.cn

[K05] 深拷贝对象
来源：http://od.chemitech.net.cn

Py:   copy.deepcopy(obj)
来源：http://rc.521024.cn

PHP:  unserialize(serialize($obj));
来源：http://ni.huanxung.cn

JS:   structuredClone(obj)
来源：http://fl.shtwfgs.cn

TS:   structuredClone(obj)
来源：http://im.hnjuh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bt.haigaiapp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hu.521024.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tt.bjjhwx.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yu.jianghongdianzi.cn

[K06] 解析 URL 查询串
来源：http://jp.521024.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kx.bjjhwx.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vp.huixiangedu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ni.asd995.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oc.521024.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://st.huixinmuqiang.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://eq.colortex.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qt.colortex.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zy.wgjwhj.cn

[K07] 进制转换
来源：http://oi.szsharing.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ms.wgjwhj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gh.hnjuh.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wv.huixinmuqiang.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kn.chemitech.net.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hr.hnjuh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kh.huixiangedu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vi.muxihuayi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://di.wgjwhj.cn

[K08] 二进制序列化（非 JSON）
来源：http://pu.jctech888.com.cn

Py:   pickle.dumps(obj)
来源：http://ii.shxzskj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xj.huanxung.cn

JS:   v8.serialize(obj)        // Node
来源：http://ni.bookmarksfly.cn

TS:   v8.serialize(obj)        // Node
来源：http://gd.yuexingan06.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sm.gzmigu.cn

Go:   encoding/gob
来源：http://kj.521024.cn

Ruby: Marshal.dump(obj)
来源：http://dg.colortex.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ob.nszjky.cn

================================================================================
来源：http://tk.asd995.cn

L. 网络请求
来源：http://lb.nicolike.cn

================================================================================
来源：http://gh.lnxyls.cn

[L01] 发送 GET 请求
来源：http://ao.jctech888.com.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bg.bookmarksfly.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bx.huixinmuqiang.cn

JS:   await fetch(url)
来源：http://ki.huixiangedu.cn

TS:   await fetch(url)
来源：http://jd.nicolike.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vp.shxzskj.cn

Go:   resp, err := http.Get(url)
来源：http://os.hahajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ru.newstarts.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ir.lnxyls.cn

[L02] 发送 POST JSON
来源：http://cz.521024.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rz.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cd.yuntaijiaju.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dh.chemitech.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://di.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vp.szxytkj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lq.yuntaijiaju.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xs.colortex.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qz.gzmigu.cn

[L03] 设置自定义请求头
来源：http://mh.muxihuayi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lv.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wj.chemitech.net.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kx.colortex.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wg.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gj.wgjwhj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://io.huixiangedu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rq.colortex.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ow.shxzukj.cn

[L04] 设置超时
来源：http://zv.9csxet.cn

Py:   requests.get(url, timeout=5)
来源：http://ee.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cy.yuexingan06.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wv.bookmarksfly.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vu.yuexingan06.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jd.szsharing.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zt.521024.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zk.gzmigu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xt.szsharing.cn

[L05] 上传文件（multipart）
来源：http://of.yuntaijiaju.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://oy.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://em.muxihuayi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://td.yuntaijiaju.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pu.haigaiapp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hm.jctech888.com.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rv.newstarts.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.panjiajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bm.szxytkj.cn

[L06] 解析响应为 JSON
来源：http://wt.hnjuh.cn

Py:   resp.json()
来源：http://qk.haigaiapp.cn

PHP:  json_decode($body, true);
来源：http://jk.nszjky.cn

JS:   await resp.json()
来源：http://dz.chemitech.net.cn

TS:   await resp.json()
来源：http://qv.jianghongdianzi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oa.szxytkj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cs.nicolike.cn

Ruby: JSON.parse(resp.body)
来源：http://lk.muxihuayi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ly.nicolike.cn

[L07] 处理 HTTP 状态码
来源：http://uh.9csxet.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uj.nszjky.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fu.hnjuh.cn

JS:   resp.ok;  resp.status
来源：http://en.newstarts.cn

TS:   resp.ok;  resp.status
来源：http://yw.yuexingan06.cn

Java: resp.statusCode()
来源：http://cg.colortex.cn

Go:   resp.StatusCode
来源：http://ha.nszjky.cn

Ruby: resp.code.to_i
来源：http://oc.szxytkj.cn

C#:   (int)resp.StatusCode
来源：http://nq.shxzskj.cn

[L08] 并发请求多个地址
来源：http://pa.nszjky.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ef.szxytkj.cn

PHP:  curl_multi_init() 系列
来源：http://wv.hahajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hn.huixiangedu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vi.hnjuh.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ma.hahajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xm.shtwfgs.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bb.chemitech.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://oa.nszjky.cn

================================================================================
来源：http://pa.chemitech.net.cn

M. 命令行 / 进程 / 环境
来源：http://fp.huixinmuqiang.cn

================================================================================
来源：http://sg.shxzskj.cn

[M01] 读取命令行参数
来源：http://st.haigaiapp.cn

Py:   sys.argv[1:]
来源：http://ye.szxytkj.cn

PHP:  $argv;  $argc;
来源：http://cz.hnjuh.cn

JS:   process.argv.slice(2)
来源：http://yo.shxzukj.cn

TS:   process.argv.slice(2)
来源：http://jn.yuntaijiaju.cn

Java: args 数组（main 方法参数）
来源：http://fd.haigaiapp.cn

Go:   os.Args[1:]
来源：http://ao.colortex.cn

Ruby: ARGV
来源：http://yr.muxihuayi.cn

C#:   args 数组（Main 方法参数）
来源：http://rb.muxihuayi.cn

[M02] 读取环境变量
来源：http://lh.nicolike.cn

Py:   os.environ.get("HOME")
来源：http://ue.hnjuh.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://we.gzmigu.cn

JS:   process.env.HOME
来源：http://yd.nicolike.cn

TS:   process.env.HOME
来源：http://gd.jianghongdianzi.cn

Java: System.getenv("HOME")
来源：http://td.shxzskj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ut.wgjwhj.cn

Ruby: ENV["HOME"]
来源：http://nw.shtwfgs.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bz.shtwfgs.cn

[M03] 执行外部命令
来源：http://dc.haigaiapp.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nm.haigaiapp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://og.bjjhwx.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://sy.asd995.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qn.asd995.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://by.asd995.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://sv.shxzskj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://cp.lnxyls.cn

C#:   Process.Start("ls", "-l");
来源：http://uo.bjjhwx.cn

[M04] 获取当前工作目录
来源：http://cs.chemitech.net.cn

Py:   os.getcwd()
来源：http://mu.jctech888.com.cn

PHP:  getcwd();
来源：http://xy.chemitech.net.cn

JS:   process.cwd()
来源：http://ru.nszjky.cn

TS:   process.cwd()
来源：http://wq.colortex.cn

Java: Path.of("").toAbsolutePath()
来源：http://lp.bjjhwx.cn

Go:   os.Getwd()
来源：http://uz.muxihuayi.cn

Ruby: Dir.pwd
来源：http://ew.haigaiapp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://cc.lnxyls.cn

[M05] 设置退出码
来源：http://jr.chemitech.net.cn

Py:   sys.exit(1)
来源：http://fc.bjjhwx.cn

PHP:  exit(1);
来源：http://gm.nszjky.cn

JS:   process.exit(1)
来源：http://ig.hahajie.cn

TS:   process.exit(1)
来源：http://mj.chemitech.net.cn

Java: System.exit(1)
来源：http://gv.haigaiapp.cn

Go:   os.Exit(1)
来源：http://uc.shxzukj.cn

Ruby: exit 1
来源：http://ml.shxzukj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ah.asd995.cn

[M06] 向标准错误输出
来源：http://ux.yuntaijiaju.cn

Py:   print("err", file=sys.stderr)
来源：http://vx.muxihuayi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tu.asd995.cn

JS:   console.error("err")
来源：http://dh.chemitech.net.cn

TS:   console.error("err")
来源：http://jp.asd995.cn

Java: System.err.println("err")
来源：http://xn.huixiangedu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nq.521024.cn

Ruby: warn "err"
来源：http://gb.huanxung.cn

C#:   Console.Error.WriteLine("err")
来源：http://fh.asd995.cn

[M07] 判断是否为主入口
来源：http://is.yuexingan06.cn

Py:   if __name__ == "__main__":
来源：http://zt.shtwfgs.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cn.chemitech.net.cn

JS:   require.main === module
来源：http://cz.huixinmuqiang.cn

TS:   require.main === module
来源：http://ye.newstarts.cn

Java: public static void main(String[] args)
来源：http://vf.hahajie.cn

Go:   func main()
来源：http://hb.chemitech.net.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nr.shxzukj.cn

C#:   static void Main(string[] args)
来源：http://qf.521024.cn

[M08] 获取系统与运行时信息
来源：http://cj.colortex.cn

Py:   platform.system();  platform.python_version()
来源：http://ht.huixiangedu.cn

PHP:  PHP_OS;  phpversion();
来源：http://ga.bjjhwx.cn

JS:   process.platform;  process.version
来源：http://rx.nicolike.cn

TS:   process.platform;  process.version
来源：http://vk.shxzukj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ra.yuntaijiaju.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://jq.panjiajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://iq.shxzukj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://cj.hnjuh.cn

================================================================================
来源：http://em.nicolike.cn

N. 数据结构与算法
来源：http://jh.huixiangedu.cn

================================================================================
来源：http://qj.huixinmuqiang.cn

[N01] 二分查找（有序数组）
来源：http://ui.yuexingan06.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gd.asd995.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gp.huixiangedu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ay.huanxung.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fj.szsharing.cn

Java: Arrays.binarySearch(arr, x)
来源：http://oh.nicolike.cn

Go:   sort.SearchInts(arr, x)
来源：http://fe.chemitech.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://js.huixinmuqiang.cn


<!-- 参考信息 -->