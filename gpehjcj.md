代发 wailian999

[J03] 字符串解析为日期
来源：http://oz.muxihuayi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bw.chemitech.net.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uj.szxytkj.cn

JS:   new Date("2024-01-02")
来源：http://np.yuntaijiaju.cn

TS:   new Date("2024-01-02")
来源：http://vv.nszjky.cn

Java: LocalDate.parse("2024-01-02")
来源：http://yw.521024.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xx.jianghongdianzi.cn

Ruby: Date.parse("2024-01-02")
来源：http://br.huixiangedu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://iu.lnxyls.cn

[J04] 时间戳与日期互转
来源：http://zl.szsharing.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bz.jctech888.com.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vc.nicolike.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pj.yuexingan06.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ua.colortex.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pr.huanxung.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ex.huanxung.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cp.asd995.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gb.jianghongdianzi.cn

[J05] 时间加减（加 7 天）
来源：http://gl.muxihuayi.cn

Py:   now + timedelta(days=7)
来源：http://lm.colortex.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xx.shxzukj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xo.bookmarksfly.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hg.asd995.cn

Java: LocalDate.now().plusDays(7)
来源：http://uz.shxzukj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yy.huixinmuqiang.cn

Ruby: Time.now + 7 * 86400
来源：http://uc.huanxung.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ey.bookmarksfly.cn

[J06] 计算两时间之差
来源：http://xv.yuexingan06.cn

Py:   (end - start).total_seconds()
来源：http://hf.colortex.cn

PHP:  $end->diff($start)->days;
来源：http://hx.nicolike.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://iw.wgjwhj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xt.szxytkj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ky.bjjhwx.cn

Go:   end.Sub(start).Hours()
来源：http://or.huixiangedu.cn

Ruby: end - start                 # 返回秒数
来源：http://dm.huanxung.cn

C#:   (end - start).TotalSeconds
来源：http://mr.521024.cn

[J07] 比较两个日期
来源：http://kg.wgjwhj.cn

Py:   d1 < d2;  d1 == d2
来源：http://hd.9csxet.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nt.haigaiapp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ue.chemitech.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://kk.asd995.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yu.colortex.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://br.colortex.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fc.colortex.cn

C#:   d1 < d2;  d1 == d2
来源：http://od.nicolike.cn

[J08] 提取年月日与星期
来源：http://ue.hahajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://oa.szsharing.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hh.chemitech.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ky.shxzukj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gr.shxzukj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rb.muxihuayi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vz.hahajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://my.newstarts.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vm.jianghongdianzi.cn

[J09] 时区处理
来源：http://pc.9csxet.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tl.muxihuayi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qt.szsharing.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yp.lnxyls.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rf.huixinmuqiang.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ng.jctech888.com.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fh.huanxung.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://es.bookmarksfly.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pe.nszjky.cn

[J10] 取今天 / 本月第一天
来源：http://th.gzmigu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://nd.chemitech.net.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cv.521024.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ld.colortex.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pe.lnxyls.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ou.huixinmuqiang.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hg.szsharing.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rz.bookmarksfly.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yl.gzmigu.cn

================================================================================
来源：http://dw.newstarts.cn

K. JSON 与序列化
来源：http://hx.hahajie.cn

================================================================================
来源：http://oy.yuexingan06.cn

[K01] 对象转 JSON 字符串
来源：http://tz.szsharing.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uj.szxytkj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ki.huixiangedu.cn

JS:   JSON.stringify(obj)
来源：http://cv.hahajie.cn

TS:   JSON.stringify(obj)
来源：http://jm.jctech888.com.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://br.chemitech.net.cn

Go:   json.Marshal(obj)
来源：http://yz.yuexingan06.cn

Ruby: obj.to_json                                     // require "json"
来源：http://yh.hahajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://iy.yuntaijiaju.cn

[K02] JSON 字符串转对象
来源：http://fs.szxytkj.cn

Py:   json.loads(s)
来源：http://lq.huanxung.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ds.jianghongdianzi.cn

JS:   JSON.parse(s)
来源：http://nk.bookmarksfly.cn

TS:   JSON.parse(s)
来源：http://fu.hnjuh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kz.newstarts.cn

Go:   json.Unmarshal(data, &v)
来源：http://zk.colortex.cn

Ruby: JSON.parse(s)
来源：http://fb.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tc.bjjhwx.cn

[K03] JSON 美化输出（带缩进）
来源：http://ba.szxytkj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nr.hnjuh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pb.panjiajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pc.szsharing.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xe.muxihuayi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kw.asd995.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gg.shtwfgs.cn

Ruby: JSON.pretty_generate(obj)
来源：http://cu.asd995.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://av.nicolike.cn

[K04] 读取 JSON 文件
来源：http://rn.gzmigu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kd.shtwfgs.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yz.jctech888.com.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wp.huanxung.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hy.lnxyls.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://as.szxytkj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://if.chemitech.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qk.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zu.colortex.cn

[K05] 深拷贝对象
来源：http://xo.yuntaijiaju.cn

Py:   copy.deepcopy(obj)
来源：http://xf.panjiajie.cn

PHP:  unserialize(serialize($obj));
来源：http://fj.shxzukj.cn

JS:   structuredClone(obj)
来源：http://rz.huixiangedu.cn

TS:   structuredClone(obj)
来源：http://ri.shxzskj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qh.lnxyls.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rw.bjjhwx.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tc.haigaiapp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://im.jctech888.com.cn

[K06] 解析 URL 查询串
来源：http://on.huanxung.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jv.muxihuayi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dk.hnjuh.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ar.hnjuh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gf.yuntaijiaju.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uc.szsharing.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://os.wgjwhj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dy.colortex.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qa.yuntaijiaju.cn

[K07] 进制转换
来源：http://fy.nicolike.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ab.hnjuh.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qt.muxihuayi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wz.bjjhwx.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.bookmarksfly.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://li.bookmarksfly.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ii.shtwfgs.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fv.9csxet.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://go.yuntaijiaju.cn

[K08] 二进制序列化（非 JSON）
来源：http://bb.yuntaijiaju.cn

Py:   pickle.dumps(obj)
来源：http://in.wgjwhj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fu.shtwfgs.cn

JS:   v8.serialize(obj)        // Node
来源：http://nw.shxzskj.cn

TS:   v8.serialize(obj)        // Node
来源：http://az.shtwfgs.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sm.colortex.cn

Go:   encoding/gob
来源：http://ye.yuexingan06.cn

Ruby: Marshal.dump(obj)
来源：http://ff.hahajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fo.shxzskj.cn

================================================================================
来源：http://vb.shtwfgs.cn

L. 网络请求
来源：http://jf.yuntaijiaju.cn

================================================================================
来源：http://tq.asd995.cn

[L01] 发送 GET 请求
来源：http://on.lnxyls.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mb.hahajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://by.huanxung.cn

JS:   await fetch(url)
来源：http://qx.muxihuayi.cn

TS:   await fetch(url)
来源：http://ai.huixiangedu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mk.hnjuh.cn

Go:   resp, err := http.Get(url)
来源：http://pv.nszjky.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rr.wgjwhj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pl.521024.cn

[L02] 发送 POST JSON
来源：http://tb.9csxet.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qd.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qp.bjjhwx.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xq.bjjhwx.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xu.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uq.asd995.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://st.jctech888.com.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tn.nicolike.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lw.hnjuh.cn

[L03] 设置自定义请求头
来源：http://cy.chemitech.net.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dn.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://po.huixinmuqiang.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ww.szxytkj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jr.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://te.panjiajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tg.gzmigu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://oh.wgjwhj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tb.jianghongdianzi.cn

[L04] 设置超时
来源：http://hu.asd995.cn

Py:   requests.get(url, timeout=5)
来源：http://dq.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dc.shxzskj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ia.huanxung.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sd.newstarts.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://io.huixiangedu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bz.bjjhwx.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yx.shxzukj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gz.bookmarksfly.cn

[L05] 上传文件（multipart）
来源：http://cy.bookmarksfly.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uk.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ed.shtwfgs.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gw.521024.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bw.huixiangedu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ll.9csxet.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ne.newstarts.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qz.lnxyls.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ht.yuntaijiaju.cn

[L06] 解析响应为 JSON
来源：http://ed.shtwfgs.cn

Py:   resp.json()
来源：http://ai.huanxung.cn

PHP:  json_decode($body, true);
来源：http://na.huanxung.cn

JS:   await resp.json()
来源：http://yr.bjjhwx.cn

TS:   await resp.json()
来源：http://aq.huanxung.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://la.colortex.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ey.bjjhwx.cn

Ruby: JSON.parse(resp.body)
来源：http://xf.jianghongdianzi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hg.bjjhwx.cn

[L07] 处理 HTTP 状态码
来源：http://ip.colortex.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://go.huanxung.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://op.chemitech.net.cn

JS:   resp.ok;  resp.status
来源：http://uf.huixinmuqiang.cn

TS:   resp.ok;  resp.status
来源：http://sh.bjjhwx.cn

Java: resp.statusCode()
来源：http://kk.bjjhwx.cn

Go:   resp.StatusCode
来源：http://vq.9csxet.cn

Ruby: resp.code.to_i
来源：http://cf.jianghongdianzi.cn

C#:   (int)resp.StatusCode
来源：http://zb.bookmarksfly.cn

[L08] 并发请求多个地址
来源：http://vp.muxihuayi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ap.muxihuayi.cn

PHP:  curl_multi_init() 系列
来源：http://ez.jctech888.com.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ne.huixinmuqiang.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pe.asd995.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://df.chemitech.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tm.panjiajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mf.huanxung.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pd.panjiajie.cn

================================================================================
来源：http://aw.panjiajie.cn

M. 命令行 / 进程 / 环境
来源：http://tg.huixinmuqiang.cn

================================================================================
来源：http://ls.yuexingan06.cn

[M01] 读取命令行参数
来源：http://mz.bjjhwx.cn

Py:   sys.argv[1:]
来源：http://km.asd995.cn

PHP:  $argv;  $argc;
来源：http://kj.huixinmuqiang.cn

JS:   process.argv.slice(2)
来源：http://kh.szsharing.cn

TS:   process.argv.slice(2)
来源：http://uz.nszjky.cn

Java: args 数组（main 方法参数）
来源：http://sf.colortex.cn

Go:   os.Args[1:]
来源：http://vf.yuntaijiaju.cn

Ruby: ARGV
来源：http://sb.haigaiapp.cn

C#:   args 数组（Main 方法参数）
来源：http://hf.asd995.cn

[M02] 读取环境变量
来源：http://lv.nicolike.cn

Py:   os.environ.get("HOME")
来源：http://fp.muxihuayi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mr.colortex.cn

JS:   process.env.HOME
来源：http://pr.muxihuayi.cn

TS:   process.env.HOME
来源：http://qc.huixinmuqiang.cn

Java: System.getenv("HOME")
来源：http://ng.gzmigu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qf.wgjwhj.cn

Ruby: ENV["HOME"]
来源：http://qt.jianghongdianzi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zt.bookmarksfly.cn

[M03] 执行外部命令
来源：http://gg.9csxet.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://iw.haigaiapp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://up.huixinmuqiang.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dy.panjiajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ok.521024.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tl.wgjwhj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gd.wgjwhj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://dg.huixinmuqiang.cn

C#:   Process.Start("ls", "-l");
来源：http://xv.szxytkj.cn

[M04] 获取当前工作目录
来源：http://zo.colortex.cn

Py:   os.getcwd()
来源：http://ts.jianghongdianzi.cn

PHP:  getcwd();
来源：http://fr.szxytkj.cn

JS:   process.cwd()
来源：http://rd.wgjwhj.cn

TS:   process.cwd()
来源：http://ym.wgjwhj.cn

Java: Path.of("").toAbsolutePath()
来源：http://ns.lnxyls.cn

Go:   os.Getwd()
来源：http://gy.panjiajie.cn

Ruby: Dir.pwd
来源：http://pa.9csxet.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ab.muxihuayi.cn

[M05] 设置退出码
来源：http://uq.haigaiapp.cn

Py:   sys.exit(1)
来源：http://pr.shtwfgs.cn

PHP:  exit(1);
来源：http://hj.yuntaijiaju.cn

JS:   process.exit(1)
来源：http://mv.muxihuayi.cn

TS:   process.exit(1)
来源：http://nz.haigaiapp.cn

Java: System.exit(1)
来源：http://cz.nszjky.cn

Go:   os.Exit(1)
来源：http://vn.shxzukj.cn

Ruby: exit 1
来源：http://yj.huanxung.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zf.muxihuayi.cn

[M06] 向标准错误输出
来源：http://pa.szxytkj.cn

Py:   print("err", file=sys.stderr)
来源：http://ac.szsharing.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xz.shxzskj.cn

JS:   console.error("err")
来源：http://nx.huixinmuqiang.cn

TS:   console.error("err")
来源：http://im.huanxung.cn

Java: System.err.println("err")
来源：http://os.huanxung.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mg.jctech888.com.cn

Ruby: warn "err"
来源：http://la.bookmarksfly.cn

C#:   Console.Error.WriteLine("err")
来源：http://df.bookmarksfly.cn

[M07] 判断是否为主入口
来源：http://bf.huanxung.cn

Py:   if __name__ == "__main__":
来源：http://qe.hahajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ph.huixinmuqiang.cn

JS:   require.main === module
来源：http://ib.haigaiapp.cn

TS:   require.main === module
来源：http://zf.wgjwhj.cn

Java: public static void main(String[] args)
来源：http://al.yuexingan06.cn

Go:   func main()
来源：http://bp.shxzukj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bb.hnjuh.cn

C#:   static void Main(string[] args)
来源：http://gl.hahajie.cn

[M08] 获取系统与运行时信息
来源：http://zv.521024.cn

Py:   platform.system();  platform.python_version()
来源：http://tu.jctech888.com.cn

PHP:  PHP_OS;  phpversion();
来源：http://nv.nicolike.cn

JS:   process.platform;  process.version
来源：http://gb.colortex.cn

TS:   process.platform;  process.version
来源：http://gt.huixiangedu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://in.haigaiapp.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ah.asd995.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dw.muxihuayi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://uw.yuntaijiaju.cn

================================================================================
来源：http://bl.yuexingan06.cn

N. 数据结构与算法
来源：http://nn.jctech888.com.cn

================================================================================
来源：http://hl.panjiajie.cn


<!-- 参考信息 -->