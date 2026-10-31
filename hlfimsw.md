代发 wailian999

TS:   new Date("2024-01-02")
来源：http://qz.521024.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ox.huixiangedu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qy.asd995.cn

Ruby: Date.parse("2024-01-02")
来源：http://jz.gzmigu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ir.yuntaijiaju.cn

[J04] 时间戳与日期互转
来源：http://hg.521024.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uq.asd995.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ww.haigaiapp.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nu.haigaiapp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://nm.nicolike.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ld.colortex.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hh.yuntaijiaju.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cs.shtwfgs.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lb.shxzukj.cn

[J05] 时间加减（加 7 天）
来源：http://ol.asd995.cn

Py:   now + timedelta(days=7)
来源：http://ih.9csxet.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://tf.yuexingan06.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kf.asd995.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://se.nszjky.cn

Java: LocalDate.now().plusDays(7)
来源：http://gf.lnxyls.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jj.bookmarksfly.cn

Ruby: Time.now + 7 * 86400
来源：http://xk.hahajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://or.hahajie.cn

[J06] 计算两时间之差
来源：http://dr.bookmarksfly.cn

Py:   (end - start).total_seconds()
来源：http://vc.jctech888.com.cn

PHP:  $end->diff($start)->days;
来源：http://qj.colortex.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bb.nicolike.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rg.521024.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jf.haigaiapp.cn

Go:   end.Sub(start).Hours()
来源：http://fk.shxzukj.cn

Ruby: end - start                 # 返回秒数
来源：http://qb.jianghongdianzi.cn

C#:   (end - start).TotalSeconds
来源：http://yf.szsharing.cn

[J07] 比较两个日期
来源：http://aw.nicolike.cn

Py:   d1 < d2;  d1 == d2
来源：http://rb.newstarts.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xw.gzmigu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tn.bookmarksfly.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mi.szsharing.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cj.nicolike.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bi.jianghongdianzi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://uc.szxytkj.cn

C#:   d1 < d2;  d1 == d2
来源：http://ec.jctech888.com.cn

[J08] 提取年月日与星期
来源：http://bq.asd995.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qd.szxytkj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dq.shtwfgs.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vy.panjiajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bw.nszjky.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wo.jianghongdianzi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xi.muxihuayi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qo.wgjwhj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sa.wgjwhj.cn

[J09] 时区处理
来源：http://wd.lnxyls.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://go.colortex.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vj.yuexingan06.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wg.jianghongdianzi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ms.panjiajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pk.bookmarksfly.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jk.shtwfgs.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lh.asd995.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yt.yuntaijiaju.cn

[J10] 取今天 / 本月第一天
来源：http://xc.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fa.nszjky.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tq.hnjuh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nt.jctech888.com.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xt.huanxung.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cw.huanxung.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dk.colortex.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ts.huanxung.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kl.gzmigu.cn

================================================================================
来源：http://ks.asd995.cn

K. JSON 与序列化
来源：http://xa.yuntaijiaju.cn

================================================================================
来源：http://ha.jctech888.com.cn

[K01] 对象转 JSON 字符串
来源：http://kf.huixiangedu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vu.szsharing.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mt.shxzukj.cn

JS:   JSON.stringify(obj)
来源：http://yn.hnjuh.cn

TS:   JSON.stringify(obj)
来源：http://vo.szsharing.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://oi.chemitech.net.cn

Go:   json.Marshal(obj)
来源：http://me.jianghongdianzi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cy.colortex.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dh.shxzukj.cn

[K02] JSON 字符串转对象
来源：http://bx.gzmigu.cn

Py:   json.loads(s)
来源：http://sb.hahajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tr.521024.cn

JS:   JSON.parse(s)
来源：http://ky.yuntaijiaju.cn

TS:   JSON.parse(s)
来源：http://fb.9csxet.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nb.huixiangedu.cn

Go:   json.Unmarshal(data, &v)
来源：http://gs.shtwfgs.cn

Ruby: JSON.parse(s)
来源：http://md.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vl.hahajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://wj.521024.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tn.wgjwhj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://co.newstarts.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://mc.panjiajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xy.wgjwhj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ne.panjiajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rg.muxihuayi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://tp.521024.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wk.shtwfgs.cn

[K04] 读取 JSON 文件
来源：http://cc.yuexingan06.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dh.asd995.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fr.shxzukj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bh.bookmarksfly.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mv.szxytkj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vy.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://by.nicolike.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ia.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hq.huanxung.cn

[K05] 深拷贝对象
来源：http://zq.yuntaijiaju.cn

Py:   copy.deepcopy(obj)
来源：http://qi.shxzukj.cn

PHP:  unserialize(serialize($obj));
来源：http://gq.szsharing.cn

JS:   structuredClone(obj)
来源：http://dm.szxytkj.cn

TS:   structuredClone(obj)
来源：http://uu.521024.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ol.jianghongdianzi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bh.nszjky.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rm.521024.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://nb.huixiangedu.cn

[K06] 解析 URL 查询串
来源：http://ft.hnjuh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yj.nicolike.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yx.huanxung.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jy.yuexingan06.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ne.bjjhwx.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pz.9csxet.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rc.haigaiapp.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jc.haigaiapp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nn.panjiajie.cn

[K07] 进制转换
来源：http://nj.jianghongdianzi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xn.szsharing.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mw.521024.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cf.shxzukj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tv.shtwfgs.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hb.bjjhwx.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bt.shxzskj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xu.jianghongdianzi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://oq.haigaiapp.cn

[K08] 二进制序列化（非 JSON）
来源：http://ms.nicolike.cn

Py:   pickle.dumps(obj)
来源：http://ug.szsharing.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nq.asd995.cn

JS:   v8.serialize(obj)        // Node
来源：http://jz.chemitech.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://iu.newstarts.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kj.muxihuayi.cn

Go:   encoding/gob
来源：http://mn.wgjwhj.cn

Ruby: Marshal.dump(obj)
来源：http://yt.yuexingan06.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dk.shxzukj.cn

================================================================================
来源：http://nl.colortex.cn

L. 网络请求
来源：http://dm.bjjhwx.cn

================================================================================
来源：http://dr.nszjky.cn

[L01] 发送 GET 请求
来源：http://kv.szxytkj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lp.colortex.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xh.shxzskj.cn

JS:   await fetch(url)
来源：http://by.wgjwhj.cn

TS:   await fetch(url)
来源：http://dn.panjiajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ei.bookmarksfly.cn

Go:   resp, err := http.Get(url)
来源：http://ce.hahajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hq.muxihuayi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tl.szsharing.cn

[L02] 发送 POST JSON
来源：http://di.panjiajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ww.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ck.bookmarksfly.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nr.colortex.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://if.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xb.bookmarksfly.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://py.jianghongdianzi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ya.gzmigu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://su.muxihuayi.cn

[L03] 设置自定义请求头
来源：http://nm.gzmigu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://be.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wo.jctech888.com.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qa.shxzukj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vi.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://an.gzmigu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yl.521024.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sp.colortex.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bt.bjjhwx.cn

[L04] 设置超时
来源：http://eq.jctech888.com.cn

Py:   requests.get(url, timeout=5)
来源：http://er.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cn.szsharing.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ao.asd995.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sj.hahajie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qq.szxytkj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dm.wgjwhj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://da.shxzskj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ue.gzmigu.cn

[L05] 上传文件（multipart）
来源：http://uw.hnjuh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jq.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dl.nicolike.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nl.nszjky.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ch.bookmarksfly.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gg.yuntaijiaju.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nx.hnjuh.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bz.9csxet.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sw.asd995.cn

[L06] 解析响应为 JSON
来源：http://un.shxzskj.cn

Py:   resp.json()
来源：http://ud.bookmarksfly.cn

PHP:  json_decode($body, true);
来源：http://zv.bookmarksfly.cn

JS:   await resp.json()
来源：http://de.huixinmuqiang.cn

TS:   await resp.json()
来源：http://ei.lnxyls.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xn.chemitech.net.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jj.hahajie.cn

Ruby: JSON.parse(resp.body)
来源：http://de.wgjwhj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://oo.bjjhwx.cn

[L07] 处理 HTTP 状态码
来源：http://ak.panjiajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://eg.gzmigu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hp.hnjuh.cn

JS:   resp.ok;  resp.status
来源：http://jm.yuntaijiaju.cn

TS:   resp.ok;  resp.status
来源：http://gi.bjjhwx.cn

Java: resp.statusCode()
来源：http://fq.huixinmuqiang.cn

Go:   resp.StatusCode
来源：http://lu.muxihuayi.cn

Ruby: resp.code.to_i
来源：http://qz.gzmigu.cn

C#:   (int)resp.StatusCode
来源：http://do.9csxet.cn

[L08] 并发请求多个地址
来源：http://cj.muxihuayi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tf.huixiangedu.cn

PHP:  curl_multi_init() 系列
来源：http://vf.9csxet.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xg.yuexingan06.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ap.wgjwhj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://by.bookmarksfly.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cv.wgjwhj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lr.chemitech.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hb.yuexingan06.cn

================================================================================
来源：http://vf.shxzukj.cn

M. 命令行 / 进程 / 环境
来源：http://qh.shxzukj.cn

================================================================================
来源：http://oy.szxytkj.cn

[M01] 读取命令行参数
来源：http://jh.nicolike.cn

Py:   sys.argv[1:]
来源：http://fd.szsharing.cn

PHP:  $argv;  $argc;
来源：http://qd.9csxet.cn

JS:   process.argv.slice(2)
来源：http://ur.hnjuh.cn

TS:   process.argv.slice(2)
来源：http://px.yuexingan06.cn

Java: args 数组（main 方法参数）
来源：http://is.bjjhwx.cn

Go:   os.Args[1:]
来源：http://bd.hahajie.cn

Ruby: ARGV
来源：http://hu.bjjhwx.cn

C#:   args 数组（Main 方法参数）
来源：http://xz.colortex.cn

[M02] 读取环境变量
来源：http://mk.szsharing.cn

Py:   os.environ.get("HOME")
来源：http://vf.huixiangedu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ff.yuexingan06.cn

JS:   process.env.HOME
来源：http://el.jctech888.com.cn

TS:   process.env.HOME
来源：http://ti.colortex.cn

Java: System.getenv("HOME")
来源：http://fy.shtwfgs.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vh.yuexingan06.cn

Ruby: ENV["HOME"]
来源：http://di.colortex.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yk.lnxyls.cn

[M03] 执行外部命令
来源：http://wg.shxzukj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://aj.gzmigu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cn.shxzukj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://uj.jctech888.com.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mo.wgjwhj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nw.9csxet.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gi.bjjhwx.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tb.gzmigu.cn

C#:   Process.Start("ls", "-l");
来源：http://th.haigaiapp.cn

[M04] 获取当前工作目录
来源：http://de.haigaiapp.cn

Py:   os.getcwd()
来源：http://rg.9csxet.cn

PHP:  getcwd();
来源：http://gn.wgjwhj.cn

JS:   process.cwd()
来源：http://qf.chemitech.net.cn

TS:   process.cwd()
来源：http://fw.9csxet.cn

Java: Path.of("").toAbsolutePath()
来源：http://vg.nicolike.cn

Go:   os.Getwd()
来源：http://mr.yuexingan06.cn

Ruby: Dir.pwd
来源：http://ec.yuexingan06.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rn.yuexingan06.cn

[M05] 设置退出码
来源：http://ya.yuexingan06.cn

Py:   sys.exit(1)
来源：http://bu.chemitech.net.cn

PHP:  exit(1);
来源：http://pe.yuexingan06.cn

JS:   process.exit(1)
来源：http://rl.gzmigu.cn

TS:   process.exit(1)
来源：http://hn.shxzukj.cn

Java: System.exit(1)
来源：http://jw.bookmarksfly.cn

Go:   os.Exit(1)
来源：http://dg.haigaiapp.cn

Ruby: exit 1
来源：http://zz.bookmarksfly.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xo.huixinmuqiang.cn

[M06] 向标准错误输出
来源：http://yj.lnxyls.cn

Py:   print("err", file=sys.stderr)
来源：http://vp.shxzukj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://md.hahajie.cn

JS:   console.error("err")
来源：http://ql.huanxung.cn

TS:   console.error("err")
来源：http://iz.hahajie.cn

Java: System.err.println("err")
来源：http://og.szxytkj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://il.yuntaijiaju.cn

Ruby: warn "err"
来源：http://zq.9csxet.cn

C#:   Console.Error.WriteLine("err")
来源：http://fk.9csxet.cn

[M07] 判断是否为主入口
来源：http://ym.huanxung.cn

Py:   if __name__ == "__main__":
来源：http://wq.panjiajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xx.gzmigu.cn

JS:   require.main === module
来源：http://tp.szxytkj.cn

TS:   require.main === module
来源：http://az.9csxet.cn

Java: public static void main(String[] args)
来源：http://gk.9csxet.cn

Go:   func main()
来源：http://fh.bookmarksfly.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gd.bookmarksfly.cn

C#:   static void Main(string[] args)
来源：http://ke.lnxyls.cn

[M08] 获取系统与运行时信息
来源：http://mz.huanxung.cn

Py:   platform.system();  platform.python_version()
来源：http://no.bjjhwx.cn

PHP:  PHP_OS;  phpversion();
来源：http://kj.chemitech.net.cn

JS:   process.platform;  process.version
来源：http://aa.colortex.cn

TS:   process.platform;  process.version
来源：http://rw.9csxet.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wk.bjjhwx.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qd.colortex.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qw.nicolike.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://lo.jianghongdianzi.cn

================================================================================
来源：http://of.haigaiapp.cn

N. 数据结构与算法
来源：http://nl.bookmarksfly.cn

================================================================================
来源：http://hs.newstarts.cn

[N01] 二分查找（有序数组）
来源：http://gb.yuexingan06.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yv.huixinmuqiang.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wg.colortex.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://us.colortex.cn


<!-- 参考信息 -->