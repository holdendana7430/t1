代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dy.gzmigu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fq.nszjky.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mo.jctech888.com.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ie.muxihuayi.cn

[J03] 字符串解析为日期
来源：http://mg.nszjky.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fi.szsharing.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sh.gzmigu.cn

JS:   new Date("2024-01-02")
来源：http://nz.521024.cn

TS:   new Date("2024-01-02")
来源：http://yp.nszjky.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rs.jianghongdianzi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vd.wgjwhj.cn

Ruby: Date.parse("2024-01-02")
来源：http://km.nszjky.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://os.muxihuayi.cn

[J04] 时间戳与日期互转
来源：http://ix.521024.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ua.chemitech.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ib.chemitech.net.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://by.nicolike.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cn.hahajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jf.panjiajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jq.nicolike.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zu.huanxung.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kp.colortex.cn

[J05] 时间加减（加 7 天）
来源：http://wu.shtwfgs.cn

Py:   now + timedelta(days=7)
来源：http://rw.yuexingan06.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xe.huixinmuqiang.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qy.muxihuayi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lg.newstarts.cn

Java: LocalDate.now().plusDays(7)
来源：http://nq.9csxet.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bc.szxytkj.cn

Ruby: Time.now + 7 * 86400
来源：http://mi.colortex.cn

C#:   DateTime.Now.AddDays(7)
来源：http://no.huanxung.cn

[J06] 计算两时间之差
来源：http://qa.nszjky.cn

Py:   (end - start).total_seconds()
来源：http://fm.szsharing.cn

PHP:  $end->diff($start)->days;
来源：http://ev.haigaiapp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vt.asd995.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jx.chemitech.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fa.hahajie.cn

Go:   end.Sub(start).Hours()
来源：http://po.bjjhwx.cn

Ruby: end - start                 # 返回秒数
来源：http://nd.shtwfgs.cn

C#:   (end - start).TotalSeconds
来源：http://to.shxzskj.cn

[J07] 比较两个日期
来源：http://vz.shxzskj.cn

Py:   d1 < d2;  d1 == d2
来源：http://ts.huixiangedu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://om.bookmarksfly.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hn.huanxung.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mk.shxzskj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rt.huanxung.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://et.wgjwhj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ml.huixinmuqiang.cn

C#:   d1 < d2;  d1 == d2
来源：http://fi.shxzukj.cn

[J08] 提取年月日与星期
来源：http://yk.huixiangedu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jr.shxzskj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://no.colortex.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rw.nicolike.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tn.colortex.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qh.wgjwhj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wk.nszjky.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yt.yuexingan06.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ge.colortex.cn

[J09] 时区处理
来源：http://rr.chemitech.net.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ap.huanxung.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nf.chemitech.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sc.jctech888.com.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tv.muxihuayi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wc.panjiajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gp.gzmigu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mv.shxzskj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vj.huanxung.cn

[J10] 取今天 / 本月第一天
来源：http://dv.9csxet.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zc.hnjuh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zz.jianghongdianzi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zm.muxihuayi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://os.muxihuayi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zo.muxihuayi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yy.huixiangedu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pf.huanxung.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bj.hahajie.cn

================================================================================
来源：http://sk.gzmigu.cn

K. JSON 与序列化
来源：http://od.szsharing.cn

================================================================================
来源：http://or.shxzskj.cn

[K01] 对象转 JSON 字符串
来源：http://gk.asd995.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gz.haigaiapp.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://me.521024.cn

JS:   JSON.stringify(obj)
来源：http://qk.nicolike.cn

TS:   JSON.stringify(obj)
来源：http://sf.hahajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nh.colortex.cn

Go:   json.Marshal(obj)
来源：http://rr.shxzskj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://sp.panjiajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fl.jianghongdianzi.cn

[K02] JSON 字符串转对象
来源：http://nt.nicolike.cn

Py:   json.loads(s)
来源：http://br.yuntaijiaju.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gl.colortex.cn

JS:   JSON.parse(s)
来源：http://pw.newstarts.cn

TS:   JSON.parse(s)
来源：http://gy.nszjky.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://di.jianghongdianzi.cn

Go:   json.Unmarshal(data, &v)
来源：http://rc.wgjwhj.cn

Ruby: JSON.parse(s)
来源：http://tl.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://et.nicolike.cn

[K03] JSON 美化输出（带缩进）
来源：http://ka.muxihuayi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ch.jctech888.com.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mc.gzmigu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://al.newstarts.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qo.muxihuayi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fb.9csxet.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ng.haigaiapp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vu.hahajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jb.shtwfgs.cn

[K04] 读取 JSON 文件
来源：http://al.newstarts.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tu.shtwfgs.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ku.hnjuh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://di.bookmarksfly.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sv.hahajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vd.hnjuh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wp.colortex.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ul.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rh.jianghongdianzi.cn

[K05] 深拷贝对象
来源：http://jg.bjjhwx.cn

Py:   copy.deepcopy(obj)
来源：http://ut.panjiajie.cn

PHP:  unserialize(serialize($obj));
来源：http://eo.panjiajie.cn

JS:   structuredClone(obj)
来源：http://cg.gzmigu.cn

TS:   structuredClone(obj)
来源：http://es.newstarts.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://id.colortex.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ic.newstarts.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dh.jianghongdianzi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://or.szxytkj.cn

[K06] 解析 URL 查询串
来源：http://ka.nicolike.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zn.yuexingan06.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ih.9csxet.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://al.yuntaijiaju.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fd.nicolike.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dj.huanxung.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bd.yuntaijiaju.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pi.haigaiapp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ph.shtwfgs.cn

[K07] 进制转换
来源：http://af.newstarts.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nx.szxytkj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ou.wgjwhj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rf.nszjky.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nk.shxzukj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xw.jianghongdianzi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gn.haigaiapp.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://im.haigaiapp.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ld.gzmigu.cn

[K08] 二进制序列化（非 JSON）
来源：http://zh.yuexingan06.cn

Py:   pickle.dumps(obj)
来源：http://nz.shtwfgs.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ck.shtwfgs.cn

JS:   v8.serialize(obj)        // Node
来源：http://hy.521024.cn

TS:   v8.serialize(obj)        // Node
来源：http://bm.haigaiapp.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hx.shxzskj.cn

Go:   encoding/gob
来源：http://oo.nicolike.cn

Ruby: Marshal.dump(obj)
来源：http://bj.shtwfgs.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ow.gzmigu.cn

================================================================================
来源：http://ah.huixinmuqiang.cn

L. 网络请求
来源：http://ik.521024.cn

================================================================================
来源：http://uj.jianghongdianzi.cn

[L01] 发送 GET 请求
来源：http://qu.huixinmuqiang.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ob.nszjky.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://iq.wgjwhj.cn

JS:   await fetch(url)
来源：http://lz.shtwfgs.cn

TS:   await fetch(url)
来源：http://ga.szsharing.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pz.wgjwhj.cn

Go:   resp, err := http.Get(url)
来源：http://fe.colortex.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wn.nszjky.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bz.wgjwhj.cn

[L02] 发送 POST JSON
来源：http://bt.shtwfgs.cn

Py:   requests.post(url, json={"a": 1})
来源：http://tu.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yy.asd995.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ql.lnxyls.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://un.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wm.shxzukj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wl.bookmarksfly.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wz.lnxyls.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rk.huixinmuqiang.cn

[L03] 设置自定义请求头
来源：http://aw.szsharing.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ae.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wm.huixinmuqiang.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jz.colortex.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://em.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ek.colortex.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ja.yuexingan06.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bd.szsharing.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://md.huixiangedu.cn

[L04] 设置超时
来源：http://cq.shtwfgs.cn

Py:   requests.get(url, timeout=5)
来源：http://qh.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wo.asd995.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qb.haigaiapp.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://va.yuexingan06.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gt.szsharing.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://so.shxzukj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rq.gzmigu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ka.shxzukj.cn

[L05] 上传文件（multipart）
来源：http://mw.muxihuayi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gm.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jx.shtwfgs.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ov.colortex.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vn.chemitech.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sf.hnjuh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ej.huixiangedu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ph.shxzskj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mk.521024.cn

[L06] 解析响应为 JSON
来源：http://lk.jctech888.com.cn

Py:   resp.json()
来源：http://rs.szxytkj.cn

PHP:  json_decode($body, true);
来源：http://bb.lnxyls.cn

JS:   await resp.json()
来源：http://rv.szsharing.cn

TS:   await resp.json()
来源：http://ro.hnjuh.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://an.yuntaijiaju.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lg.hnjuh.cn

Ruby: JSON.parse(resp.body)
来源：http://ej.bjjhwx.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pj.huixinmuqiang.cn

[L07] 处理 HTTP 状态码
来源：http://vu.hahajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mx.muxihuayi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nh.bjjhwx.cn

JS:   resp.ok;  resp.status
来源：http://rr.haigaiapp.cn

TS:   resp.ok;  resp.status
来源：http://au.bjjhwx.cn

Java: resp.statusCode()
来源：http://lq.huanxung.cn

Go:   resp.StatusCode
来源：http://fe.bjjhwx.cn

Ruby: resp.code.to_i
来源：http://pz.szsharing.cn

C#:   (int)resp.StatusCode
来源：http://zq.szxytkj.cn

[L08] 并发请求多个地址
来源：http://np.szsharing.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ax.huixiangedu.cn

PHP:  curl_multi_init() 系列
来源：http://oa.bjjhwx.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zw.huixiangedu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://on.jctech888.com.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tj.lnxyls.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://od.hnjuh.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://od.szsharing.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ye.bookmarksfly.cn

================================================================================
来源：http://sg.shtwfgs.cn

M. 命令行 / 进程 / 环境
来源：http://ls.hnjuh.cn

================================================================================
来源：http://gc.wgjwhj.cn

[M01] 读取命令行参数
来源：http://ry.nszjky.cn

Py:   sys.argv[1:]
来源：http://yr.521024.cn

PHP:  $argv;  $argc;
来源：http://te.9csxet.cn

JS:   process.argv.slice(2)
来源：http://mc.huixinmuqiang.cn

TS:   process.argv.slice(2)
来源：http://uy.hnjuh.cn

Java: args 数组（main 方法参数）
来源：http://md.haigaiapp.cn

Go:   os.Args[1:]
来源：http://pn.colortex.cn

Ruby: ARGV
来源：http://pj.shxzskj.cn

C#:   args 数组（Main 方法参数）
来源：http://nz.szsharing.cn

[M02] 读取环境变量
来源：http://fv.nicolike.cn

Py:   os.environ.get("HOME")
来源：http://fh.jctech888.com.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://te.yuexingan06.cn

JS:   process.env.HOME
来源：http://jx.yuntaijiaju.cn

TS:   process.env.HOME
来源：http://ut.lnxyls.cn

Java: System.getenv("HOME")
来源：http://lc.newstarts.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mk.szsharing.cn

Ruby: ENV["HOME"]
来源：http://ja.hnjuh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rc.szxytkj.cn

[M03] 执行外部命令
来源：http://cx.jianghongdianzi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://un.hahajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zd.panjiajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://le.bjjhwx.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://eq.muxihuayi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ad.asd995.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vc.colortex.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bb.bookmarksfly.cn

C#:   Process.Start("ls", "-l");
来源：http://zc.yuntaijiaju.cn

[M04] 获取当前工作目录
来源：http://lc.haigaiapp.cn

Py:   os.getcwd()
来源：http://fd.gzmigu.cn

PHP:  getcwd();
来源：http://ew.huixinmuqiang.cn

JS:   process.cwd()
来源：http://lg.muxihuayi.cn

TS:   process.cwd()
来源：http://fp.haigaiapp.cn

Java: Path.of("").toAbsolutePath()
来源：http://lk.szsharing.cn

Go:   os.Getwd()
来源：http://fu.nszjky.cn

Ruby: Dir.pwd
来源：http://hn.bjjhwx.cn

C#:   Directory.GetCurrentDirectory()
来源：http://fx.muxihuayi.cn

[M05] 设置退出码
来源：http://ae.shxzskj.cn

Py:   sys.exit(1)
来源：http://zl.hnjuh.cn

PHP:  exit(1);
来源：http://fu.huixinmuqiang.cn

JS:   process.exit(1)
来源：http://td.colortex.cn

TS:   process.exit(1)
来源：http://rl.asd995.cn

Java: System.exit(1)
来源：http://gz.huixinmuqiang.cn

Go:   os.Exit(1)
来源：http://xh.chemitech.net.cn

Ruby: exit 1
来源：http://ri.bookmarksfly.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://io.newstarts.cn

[M06] 向标准错误输出
来源：http://qh.haigaiapp.cn

Py:   print("err", file=sys.stderr)
来源：http://hu.panjiajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pw.huixiangedu.cn

JS:   console.error("err")
来源：http://ir.shtwfgs.cn

TS:   console.error("err")
来源：http://zj.huixinmuqiang.cn

Java: System.err.println("err")
来源：http://by.wgjwhj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ah.szxytkj.cn

Ruby: warn "err"
来源：http://qb.lnxyls.cn

C#:   Console.Error.WriteLine("err")
来源：http://xc.bjjhwx.cn

[M07] 判断是否为主入口
来源：http://pw.haigaiapp.cn

Py:   if __name__ == "__main__":
来源：http://au.nicolike.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dd.shxzukj.cn

JS:   require.main === module
来源：http://sk.szxytkj.cn

TS:   require.main === module
来源：http://dy.huixiangedu.cn

Java: public static void main(String[] args)
来源：http://jr.hahajie.cn

Go:   func main()
来源：http://pd.hahajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://eg.shxzukj.cn

C#:   static void Main(string[] args)
来源：http://ii.asd995.cn

[M08] 获取系统与运行时信息
来源：http://yr.jianghongdianzi.cn

Py:   platform.system();  platform.python_version()
来源：http://tj.lnxyls.cn

PHP:  PHP_OS;  phpversion();
来源：http://hj.9csxet.cn

JS:   process.platform;  process.version
来源：http://sy.lnxyls.cn

TS:   process.platform;  process.version
来源：http://iz.wgjwhj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uk.yuntaijiaju.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vy.szxytkj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pv.bjjhwx.cn


<!-- 参考信息 -->