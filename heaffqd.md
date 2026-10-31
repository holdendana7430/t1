代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wj.jctech888.com.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jb.jianghongdianzi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ou.lnxyls.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uo.gzmigu.cn

[J03] 字符串解析为日期
来源：http://uf.huixinmuqiang.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pu.shxzukj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dh.hahajie.cn

JS:   new Date("2024-01-02")
来源：http://lu.yuexingan06.cn

TS:   new Date("2024-01-02")
来源：http://wv.newstarts.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xb.hahajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zc.yuntaijiaju.cn

Ruby: Date.parse("2024-01-02")
来源：http://mi.newstarts.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rt.yuexingan06.cn

[J04] 时间戳与日期互转
来源：http://gm.asd995.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tf.haigaiapp.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qt.yuntaijiaju.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kr.wgjwhj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bx.jianghongdianzi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xl.jctech888.com.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ki.gzmigu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kz.nicolike.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wv.bjjhwx.cn

[J05] 时间加减（加 7 天）
来源：http://yx.huanxung.cn

Py:   now + timedelta(days=7)
来源：http://kx.jianghongdianzi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rw.haigaiapp.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gx.nicolike.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uq.lnxyls.cn

Java: LocalDate.now().plusDays(7)
来源：http://cd.colortex.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rv.huixinmuqiang.cn

Ruby: Time.now + 7 * 86400
来源：http://ci.jianghongdianzi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://yj.jianghongdianzi.cn

[J06] 计算两时间之差
来源：http://eq.panjiajie.cn

Py:   (end - start).total_seconds()
来源：http://nv.huanxung.cn

PHP:  $end->diff($start)->days;
来源：http://ze.huixiangedu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bx.huixiangedu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ri.bookmarksfly.cn

Java: Duration.between(start, end).toSeconds()
来源：http://yt.lnxyls.cn

Go:   end.Sub(start).Hours()
来源：http://bn.hahajie.cn

Ruby: end - start                 # 返回秒数
来源：http://wb.shtwfgs.cn

C#:   (end - start).TotalSeconds
来源：http://tb.chemitech.net.cn

[J07] 比较两个日期
来源：http://dn.shxzukj.cn

Py:   d1 < d2;  d1 == d2
来源：http://mz.9csxet.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pb.huanxung.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ft.nicolike.cn

TS:   d1.getTime() < d2.getTime()
来源：http://es.szxytkj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ez.chemitech.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://oc.panjiajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hd.szxytkj.cn

C#:   d1 < d2;  d1 == d2
来源：http://tc.bjjhwx.cn

[J08] 提取年月日与星期
来源：http://zk.szxytkj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ll.lnxyls.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nw.hnjuh.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nt.huanxung.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ch.szxytkj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fn.szxytkj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xk.yuexingan06.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://iy.shtwfgs.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://py.szxytkj.cn

[J09] 时区处理
来源：http://gu.hnjuh.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nu.yuntaijiaju.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://np.chemitech.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ph.szsharing.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pp.muxihuayi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ax.huixinmuqiang.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ab.bookmarksfly.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wv.jianghongdianzi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ry.haigaiapp.cn

[J10] 取今天 / 本月第一天
来源：http://fn.bookmarksfly.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://oi.huixiangedu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tk.lnxyls.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ry.szxytkj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://el.521024.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qe.nszjky.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bj.521024.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ew.gzmigu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pz.lnxyls.cn

================================================================================
来源：http://ey.yuntaijiaju.cn

K. JSON 与序列化
来源：http://pp.szsharing.cn

================================================================================
来源：http://zs.wgjwhj.cn

[K01] 对象转 JSON 字符串
来源：http://ix.nszjky.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ww.szsharing.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lb.panjiajie.cn

JS:   JSON.stringify(obj)
来源：http://qw.nszjky.cn

TS:   JSON.stringify(obj)
来源：http://el.yuexingan06.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dy.jianghongdianzi.cn

Go:   json.Marshal(obj)
来源：http://aw.muxihuayi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ek.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bz.szxytkj.cn

[K02] JSON 字符串转对象
来源：http://jz.hahajie.cn

Py:   json.loads(s)
来源：http://al.panjiajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ua.shtwfgs.cn

JS:   JSON.parse(s)
来源：http://ri.haigaiapp.cn

TS:   JSON.parse(s)
来源：http://ht.hnjuh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kd.9csxet.cn

Go:   json.Unmarshal(data, &v)
来源：http://ex.hnjuh.cn

Ruby: JSON.parse(s)
来源：http://cx.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ne.shxzskj.cn

[K03] JSON 美化输出（带缩进）
来源：http://jl.yuexingan06.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://in.hahajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://aq.lnxyls.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xk.muxihuayi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://uq.newstarts.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hs.shxzukj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pr.szxytkj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jq.hnjuh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uc.szxytkj.cn

[K04] 读取 JSON 文件
来源：http://pr.lnxyls.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://si.lnxyls.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nh.wgjwhj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ja.panjiajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://na.haigaiapp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://os.bookmarksfly.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nh.yuexingan06.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xv.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mn.nicolike.cn

[K05] 深拷贝对象
来源：http://jo.huixinmuqiang.cn

Py:   copy.deepcopy(obj)
来源：http://al.asd995.cn

PHP:  unserialize(serialize($obj));
来源：http://yr.shtwfgs.cn

JS:   structuredClone(obj)
来源：http://kd.521024.cn

TS:   structuredClone(obj)
来源：http://io.nicolike.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://lq.muxihuayi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cn.nicolike.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://js.hnjuh.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rw.szxytkj.cn

[K06] 解析 URL 查询串
来源：http://wm.nszjky.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uo.chemitech.net.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pb.huixinmuqiang.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://th.hahajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ve.yuntaijiaju.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ap.521024.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bs.wgjwhj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dr.szsharing.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uu.szsharing.cn

[K07] 进制转换
来源：http://fs.bjjhwx.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fj.panjiajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yu.colortex.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ey.szxytkj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yr.huixinmuqiang.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jk.huanxung.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jd.newstarts.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://us.chemitech.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sg.haigaiapp.cn

[K08] 二进制序列化（非 JSON）
来源：http://zq.9csxet.cn

Py:   pickle.dumps(obj)
来源：http://va.lnxyls.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xw.huixiangedu.cn

JS:   v8.serialize(obj)        // Node
来源：http://ur.huixiangedu.cn

TS:   v8.serialize(obj)        // Node
来源：http://sg.chemitech.net.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qm.521024.cn

Go:   encoding/gob
来源：http://vt.bjjhwx.cn

Ruby: Marshal.dump(obj)
来源：http://kq.yuexingan06.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lz.szsharing.cn

================================================================================
来源：http://wv.newstarts.cn

L. 网络请求
来源：http://ci.szxytkj.cn

================================================================================
来源：http://xu.panjiajie.cn

[L01] 发送 GET 请求
来源：http://hd.asd995.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://oy.nszjky.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yo.haigaiapp.cn

JS:   await fetch(url)
来源：http://zu.panjiajie.cn

TS:   await fetch(url)
来源：http://fz.lnxyls.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zg.muxihuayi.cn

Go:   resp, err := http.Get(url)
来源：http://ol.bjjhwx.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fo.asd995.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cx.colortex.cn

[L02] 发送 POST JSON
来源：http://ck.nicolike.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wy.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pt.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qm.shxzskj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wp.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wn.jctech888.com.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gh.bookmarksfly.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fm.huixinmuqiang.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vs.muxihuayi.cn

[L03] 设置自定义请求头
来源：http://xo.bjjhwx.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hb.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pw.szsharing.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ow.jctech888.com.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jg.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rm.yuexingan06.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qz.huanxung.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gm.shtwfgs.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://oe.huixinmuqiang.cn

[L04] 设置超时
来源：http://ta.hahajie.cn

Py:   requests.get(url, timeout=5)
来源：http://wv.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hc.hahajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://my.bookmarksfly.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fz.9csxet.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zh.szxytkj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wc.shtwfgs.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ia.szxytkj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cd.szsharing.cn

[L05] 上传文件（multipart）
来源：http://um.huanxung.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fb.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yr.bookmarksfly.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pz.hahajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ax.jianghongdianzi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mz.521024.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://io.bookmarksfly.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kp.huixinmuqiang.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dg.haigaiapp.cn

[L06] 解析响应为 JSON
来源：http://lj.hahajie.cn

Py:   resp.json()
来源：http://wy.huixiangedu.cn

PHP:  json_decode($body, true);
来源：http://sa.jianghongdianzi.cn

JS:   await resp.json()
来源：http://rw.chemitech.net.cn

TS:   await resp.json()
来源：http://oi.9csxet.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ax.hnjuh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ny.bjjhwx.cn

Ruby: JSON.parse(resp.body)
来源：http://ym.panjiajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fw.newstarts.cn

[L07] 处理 HTTP 状态码
来源：http://zb.shxzskj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kj.huixinmuqiang.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ot.bjjhwx.cn

JS:   resp.ok;  resp.status
来源：http://ee.bjjhwx.cn

TS:   resp.ok;  resp.status
来源：http://vc.haigaiapp.cn

Java: resp.statusCode()
来源：http://wb.hahajie.cn

Go:   resp.StatusCode
来源：http://rk.newstarts.cn

Ruby: resp.code.to_i
来源：http://pe.nszjky.cn

C#:   (int)resp.StatusCode
来源：http://ck.jianghongdianzi.cn

[L08] 并发请求多个地址
来源：http://hz.bjjhwx.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gf.haigaiapp.cn

PHP:  curl_multi_init() 系列
来源：http://ww.szsharing.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mg.shxzukj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uc.gzmigu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ss.jctech888.com.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://iq.panjiajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hs.jianghongdianzi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://od.9csxet.cn

================================================================================
来源：http://gt.9csxet.cn

M. 命令行 / 进程 / 环境
来源：http://tt.521024.cn

================================================================================
来源：http://ld.nicolike.cn

[M01] 读取命令行参数
来源：http://th.huixinmuqiang.cn

Py:   sys.argv[1:]
来源：http://im.jctech888.com.cn

PHP:  $argv;  $argc;
来源：http://hk.nszjky.cn

JS:   process.argv.slice(2)
来源：http://nf.yuexingan06.cn

TS:   process.argv.slice(2)
来源：http://ql.yuntaijiaju.cn

Java: args 数组（main 方法参数）
来源：http://nn.chemitech.net.cn

Go:   os.Args[1:]
来源：http://fr.haigaiapp.cn

Ruby: ARGV
来源：http://xc.nszjky.cn

C#:   args 数组（Main 方法参数）
来源：http://vx.bjjhwx.cn

[M02] 读取环境变量
来源：http://xp.haigaiapp.cn

Py:   os.environ.get("HOME")
来源：http://fh.jctech888.com.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tp.9csxet.cn

JS:   process.env.HOME
来源：http://zh.bjjhwx.cn

TS:   process.env.HOME
来源：http://wc.huixinmuqiang.cn

Java: System.getenv("HOME")
来源：http://oh.9csxet.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xh.yuntaijiaju.cn

Ruby: ENV["HOME"]
来源：http://qg.wgjwhj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kg.colortex.cn

[M03] 执行外部命令
来源：http://zd.yuntaijiaju.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://sc.gzmigu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tc.asd995.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://oh.muxihuayi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yi.jianghongdianzi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hw.yuntaijiaju.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ry.lnxyls.cn

Ruby: system("ls -l");  `ls -l`
来源：http://sd.nszjky.cn

C#:   Process.Start("ls", "-l");
来源：http://on.szxytkj.cn

[M04] 获取当前工作目录
来源：http://lr.panjiajie.cn

Py:   os.getcwd()
来源：http://dx.chemitech.net.cn

PHP:  getcwd();
来源：http://xb.gzmigu.cn

JS:   process.cwd()
来源：http://gm.gzmigu.cn

TS:   process.cwd()
来源：http://de.9csxet.cn

Java: Path.of("").toAbsolutePath()
来源：http://wm.jianghongdianzi.cn

Go:   os.Getwd()
来源：http://qb.muxihuayi.cn

Ruby: Dir.pwd
来源：http://fj.nszjky.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jo.chemitech.net.cn

[M05] 设置退出码
来源：http://uf.huixiangedu.cn

Py:   sys.exit(1)
来源：http://nt.newstarts.cn

PHP:  exit(1);
来源：http://ih.bookmarksfly.cn

JS:   process.exit(1)
来源：http://rf.bookmarksfly.cn

TS:   process.exit(1)
来源：http://ki.shtwfgs.cn

Java: System.exit(1)
来源：http://or.9csxet.cn

Go:   os.Exit(1)
来源：http://we.9csxet.cn

Ruby: exit 1
来源：http://hm.huanxung.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nu.bjjhwx.cn

[M06] 向标准错误输出
来源：http://pj.jianghongdianzi.cn

Py:   print("err", file=sys.stderr)
来源：http://pa.panjiajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xa.huixiangedu.cn

JS:   console.error("err")
来源：http://ek.nicolike.cn

TS:   console.error("err")
来源：http://lo.gzmigu.cn

Java: System.err.println("err")
来源：http://zo.yuntaijiaju.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://la.yuntaijiaju.cn

Ruby: warn "err"
来源：http://go.yuntaijiaju.cn

C#:   Console.Error.WriteLine("err")
来源：http://ra.szsharing.cn

[M07] 判断是否为主入口
来源：http://ep.bookmarksfly.cn

Py:   if __name__ == "__main__":
来源：http://gh.szxytkj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nq.wgjwhj.cn

JS:   require.main === module
来源：http://gl.panjiajie.cn

TS:   require.main === module
来源：http://bq.jianghongdianzi.cn

Java: public static void main(String[] args)
来源：http://zh.szsharing.cn

Go:   func main()
来源：http://be.hahajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://eq.muxihuayi.cn

C#:   static void Main(string[] args)
来源：http://gx.bookmarksfly.cn

[M08] 获取系统与运行时信息
来源：http://xk.521024.cn

Py:   platform.system();  platform.python_version()
来源：http://hg.521024.cn

PHP:  PHP_OS;  phpversion();
来源：http://as.bookmarksfly.cn

JS:   process.platform;  process.version
来源：http://gz.colortex.cn

TS:   process.platform;  process.version
来源：http://zd.hnjuh.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bc.jianghongdianzi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://sd.colortex.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://su.yuntaijiaju.cn


<!-- 参考信息 -->