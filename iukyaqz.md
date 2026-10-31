代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jp.9csxet.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lv.huixiangedu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ye.bookmarksfly.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tf.hnjuh.cn

[J03] 字符串解析为日期
来源：http://zp.chemitech.net.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uf.hahajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bv.szsharing.cn

JS:   new Date("2024-01-02")
来源：http://jb.bjjhwx.cn

TS:   new Date("2024-01-02")
来源：http://sb.shxzskj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://sh.yuntaijiaju.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vt.shxzskj.cn

Ruby: Date.parse("2024-01-02")
来源：http://de.haigaiapp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qo.shtwfgs.cn

[J04] 时间戳与日期互转
来源：http://aa.hahajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ck.bookmarksfly.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ie.muxihuayi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://le.521024.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ho.jctech888.com.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qx.wgjwhj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gj.haigaiapp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yu.chemitech.net.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vl.bjjhwx.cn

[J05] 时间加减（加 7 天）
来源：http://ow.521024.cn

Py:   now + timedelta(days=7)
来源：http://hg.haigaiapp.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bm.chemitech.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ba.chemitech.net.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xp.szsharing.cn

Java: LocalDate.now().plusDays(7)
来源：http://jp.9csxet.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ey.shtwfgs.cn

Ruby: Time.now + 7 * 86400
来源：http://rp.haigaiapp.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ss.hahajie.cn

[J06] 计算两时间之差
来源：http://ws.lnxyls.cn

Py:   (end - start).total_seconds()
来源：http://xd.shxzukj.cn

PHP:  $end->diff($start)->days;
来源：http://vo.nicolike.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://de.szsharing.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pk.shxzukj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zx.colortex.cn

Go:   end.Sub(start).Hours()
来源：http://vo.jctech888.com.cn

Ruby: end - start                 # 返回秒数
来源：http://kc.yuntaijiaju.cn

C#:   (end - start).TotalSeconds
来源：http://yq.colortex.cn

[J07] 比较两个日期
来源：http://fg.huixinmuqiang.cn

Py:   d1 < d2;  d1 == d2
来源：http://tx.nicolike.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vb.haigaiapp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vf.nszjky.cn

TS:   d1.getTime() < d2.getTime()
来源：http://lc.huixinmuqiang.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uw.huixiangedu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://oy.lnxyls.cn

Ruby: d1 < d2;  d1 == d2
来源：http://yh.muxihuayi.cn

C#:   d1 < d2;  d1 == d2
来源：http://im.nszjky.cn

[J08] 提取年月日与星期
来源：http://fw.huanxung.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cy.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ex.shtwfgs.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ej.bjjhwx.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tq.gzmigu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hl.nicolike.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ql.huixinmuqiang.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cl.bookmarksfly.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yr.chemitech.net.cn

[J09] 时区处理
来源：http://co.jianghongdianzi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gk.huanxung.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ef.panjiajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pe.shxzskj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ql.shtwfgs.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hx.nszjky.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qd.nszjky.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wh.asd995.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ro.jctech888.com.cn

[J10] 取今天 / 本月第一天
来源：http://uv.yuntaijiaju.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://qd.bookmarksfly.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ff.wgjwhj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gj.panjiajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cg.newstarts.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ug.yuexingan06.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://na.shtwfgs.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jf.huixinmuqiang.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ib.9csxet.cn

================================================================================
来源：http://ro.521024.cn

K. JSON 与序列化
来源：http://op.szsharing.cn

================================================================================
来源：http://ne.asd995.cn

[K01] 对象转 JSON 字符串
来源：http://zm.huixiangedu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://be.chemitech.net.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://es.huixinmuqiang.cn

JS:   JSON.stringify(obj)
来源：http://fq.chemitech.net.cn

TS:   JSON.stringify(obj)
来源：http://xh.panjiajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wx.panjiajie.cn

Go:   json.Marshal(obj)
来源：http://yd.haigaiapp.cn

Ruby: obj.to_json                                     // require "json"
来源：http://yw.shxzskj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://eo.huixinmuqiang.cn

[K02] JSON 字符串转对象
来源：http://qz.colortex.cn

Py:   json.loads(s)
来源：http://qp.shxzskj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gj.shxzskj.cn

JS:   JSON.parse(s)
来源：http://lo.panjiajie.cn

TS:   JSON.parse(s)
来源：http://ot.bookmarksfly.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hg.shtwfgs.cn

Go:   json.Unmarshal(data, &v)
来源：http://zj.muxihuayi.cn

Ruby: JSON.parse(s)
来源：http://ze.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kb.yuexingan06.cn

[K03] JSON 美化输出（带缩进）
来源：http://bb.szxytkj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lr.shxzukj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yy.nicolike.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bw.lnxyls.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fy.yuexingan06.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ga.szxytkj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qv.521024.cn

Ruby: JSON.pretty_generate(obj)
来源：http://uv.huanxung.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kw.huanxung.cn

[K04] 读取 JSON 文件
来源：http://gz.huixiangedu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tg.newstarts.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zn.lnxyls.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pj.yuexingan06.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://br.lnxyls.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jt.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bv.asd995.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ym.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ur.shxzukj.cn

[K05] 深拷贝对象
来源：http://er.huixinmuqiang.cn

Py:   copy.deepcopy(obj)
来源：http://tg.521024.cn

PHP:  unserialize(serialize($obj));
来源：http://ck.panjiajie.cn

JS:   structuredClone(obj)
来源：http://dm.shtwfgs.cn

TS:   structuredClone(obj)
来源：http://zi.chemitech.net.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wy.asd995.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gq.lnxyls.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jj.shtwfgs.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qk.huanxung.cn

[K06] 解析 URL 查询串
来源：http://bi.jianghongdianzi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zn.bjjhwx.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://uq.huixiangedu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nq.lnxyls.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iu.colortex.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sn.shtwfgs.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zt.chemitech.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hl.hahajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ke.muxihuayi.cn

[K07] 进制转换
来源：http://jz.huixiangedu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bn.bjjhwx.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://az.newstarts.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sk.muxihuayi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://km.yuntaijiaju.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hk.shtwfgs.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xe.muxihuayi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://st.colortex.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zt.nszjky.cn

[K08] 二进制序列化（非 JSON）
来源：http://xk.hahajie.cn

Py:   pickle.dumps(obj)
来源：http://gj.bjjhwx.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ob.jctech888.com.cn

JS:   v8.serialize(obj)        // Node
来源：http://jl.muxihuayi.cn

TS:   v8.serialize(obj)        // Node
来源：http://ht.huanxung.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tk.huixiangedu.cn

Go:   encoding/gob
来源：http://en.wgjwhj.cn

Ruby: Marshal.dump(obj)
来源：http://rl.shtwfgs.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://py.bjjhwx.cn

================================================================================
来源：http://av.asd995.cn

L. 网络请求
来源：http://py.lnxyls.cn

================================================================================
来源：http://ad.muxihuayi.cn

[L01] 发送 GET 请求
来源：http://rp.shtwfgs.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qs.nszjky.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qc.colortex.cn

JS:   await fetch(url)
来源：http://ws.shtwfgs.cn

TS:   await fetch(url)
来源：http://jw.wgjwhj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bb.nicolike.cn

Go:   resp, err := http.Get(url)
来源：http://ju.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pa.chemitech.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ia.chemitech.net.cn

[L02] 发送 POST JSON
来源：http://hu.muxihuayi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qj.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hn.hahajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kb.shxzukj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://as.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kc.shxzukj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sg.gzmigu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://he.szsharing.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vv.nszjky.cn

[L03] 设置自定义请求头
来源：http://gn.wgjwhj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zf.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sd.chemitech.net.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ju.yuexingan06.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ll.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qp.colortex.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fg.huanxung.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://iv.shxzskj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ma.colortex.cn

[L04] 设置超时
来源：http://sf.nszjky.cn

Py:   requests.get(url, timeout=5)
来源：http://ox.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mf.shxzukj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bn.huixinmuqiang.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oj.bookmarksfly.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://au.newstarts.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sk.shxzukj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mt.bookmarksfly.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://le.yuexingan06.cn

[L05] 上传文件（multipart）
来源：http://ua.chemitech.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jc.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gg.huixinmuqiang.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pm.szsharing.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lo.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://iu.hahajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://du.szxytkj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rl.shxzukj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xn.haigaiapp.cn

[L06] 解析响应为 JSON
来源：http://jj.asd995.cn

Py:   resp.json()
来源：http://uh.bjjhwx.cn

PHP:  json_decode($body, true);
来源：http://qs.wgjwhj.cn

JS:   await resp.json()
来源：http://nr.haigaiapp.cn

TS:   await resp.json()
来源：http://ev.wgjwhj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cd.shtwfgs.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uq.muxihuayi.cn

Ruby: JSON.parse(resp.body)
来源：http://xa.hnjuh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pa.shtwfgs.cn

[L07] 处理 HTTP 状态码
来源：http://xn.szxytkj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cg.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qw.asd995.cn

JS:   resp.ok;  resp.status
来源：http://vy.huixiangedu.cn

TS:   resp.ok;  resp.status
来源：http://tl.shxzukj.cn

Java: resp.statusCode()
来源：http://pu.hahajie.cn

Go:   resp.StatusCode
来源：http://eq.szxytkj.cn

Ruby: resp.code.to_i
来源：http://rx.bjjhwx.cn

C#:   (int)resp.StatusCode
来源：http://bu.gzmigu.cn

[L08] 并发请求多个地址
来源：http://zh.shxzukj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://me.shtwfgs.cn

PHP:  curl_multi_init() 系列
来源：http://ty.shxzskj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://px.521024.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://od.szxytkj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ha.muxihuayi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bl.jianghongdianzi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jz.bjjhwx.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://og.shxzukj.cn

================================================================================
来源：http://tq.szxytkj.cn

M. 命令行 / 进程 / 环境
来源：http://nh.9csxet.cn

================================================================================
来源：http://va.jianghongdianzi.cn

[M01] 读取命令行参数
来源：http://jb.shxzskj.cn

Py:   sys.argv[1:]
来源：http://ho.chemitech.net.cn

PHP:  $argv;  $argc;
来源：http://dp.huixinmuqiang.cn

JS:   process.argv.slice(2)
来源：http://fj.colortex.cn

TS:   process.argv.slice(2)
来源：http://ki.hnjuh.cn

Java: args 数组（main 方法参数）
来源：http://am.hnjuh.cn

Go:   os.Args[1:]
来源：http://tl.muxihuayi.cn

Ruby: ARGV
来源：http://uv.9csxet.cn

C#:   args 数组（Main 方法参数）
来源：http://en.colortex.cn

[M02] 读取环境变量
来源：http://qn.nszjky.cn

Py:   os.environ.get("HOME")
来源：http://kq.huixinmuqiang.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jj.asd995.cn

JS:   process.env.HOME
来源：http://sp.panjiajie.cn

TS:   process.env.HOME
来源：http://ju.wgjwhj.cn

Java: System.getenv("HOME")
来源：http://zp.jianghongdianzi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ei.chemitech.net.cn

Ruby: ENV["HOME"]
来源：http://yy.wgjwhj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tn.chemitech.net.cn

[M03] 执行外部命令
来源：http://gs.colortex.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ye.jctech888.com.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wd.asd995.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zb.hnjuh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ip.chemitech.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xd.asd995.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://bw.jctech888.com.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tu.hnjuh.cn

C#:   Process.Start("ls", "-l");
来源：http://nz.9csxet.cn

[M04] 获取当前工作目录
来源：http://bs.shxzskj.cn

Py:   os.getcwd()
来源：http://pj.wgjwhj.cn

PHP:  getcwd();
来源：http://ec.jianghongdianzi.cn

JS:   process.cwd()
来源：http://gm.chemitech.net.cn

TS:   process.cwd()
来源：http://qj.hnjuh.cn

Java: Path.of("").toAbsolutePath()
来源：http://fz.gzmigu.cn

Go:   os.Getwd()
来源：http://bc.gzmigu.cn

Ruby: Dir.pwd
来源：http://ai.jctech888.com.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ie.szsharing.cn

[M05] 设置退出码
来源：http://bi.wgjwhj.cn

Py:   sys.exit(1)
来源：http://te.haigaiapp.cn

PHP:  exit(1);
来源：http://mo.521024.cn

JS:   process.exit(1)
来源：http://nb.szxytkj.cn

TS:   process.exit(1)
来源：http://zp.panjiajie.cn

Java: System.exit(1)
来源：http://bh.nicolike.cn

Go:   os.Exit(1)
来源：http://nt.nszjky.cn

Ruby: exit 1
来源：http://rv.huanxung.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xt.newstarts.cn

[M06] 向标准错误输出
来源：http://no.nszjky.cn

Py:   print("err", file=sys.stderr)
来源：http://ob.jctech888.com.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tg.bookmarksfly.cn

JS:   console.error("err")
来源：http://aj.bookmarksfly.cn

TS:   console.error("err")
来源：http://pu.yuntaijiaju.cn

Java: System.err.println("err")
来源：http://go.panjiajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ek.gzmigu.cn

Ruby: warn "err"
来源：http://of.bjjhwx.cn

C#:   Console.Error.WriteLine("err")
来源：http://oi.panjiajie.cn

[M07] 判断是否为主入口
来源：http://ph.huanxung.cn

Py:   if __name__ == "__main__":
来源：http://jp.yuntaijiaju.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dx.lnxyls.cn

JS:   require.main === module
来源：http://xg.jctech888.com.cn

TS:   require.main === module
来源：http://uv.bjjhwx.cn

Java: public static void main(String[] args)
来源：http://bu.nicolike.cn

Go:   func main()
来源：http://xq.jctech888.com.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nq.bjjhwx.cn

C#:   static void Main(string[] args)
来源：http://oo.shxzukj.cn

[M08] 获取系统与运行时信息
来源：http://jt.hahajie.cn

Py:   platform.system();  platform.python_version()
来源：http://cv.colortex.cn

PHP:  PHP_OS;  phpversion();
来源：http://tc.chemitech.net.cn

JS:   process.platform;  process.version
来源：http://ts.colortex.cn

TS:   process.platform;  process.version
来源：http://jj.bookmarksfly.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lc.lnxyls.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://in.chemitech.net.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tz.hnjuh.cn


<!-- 参考信息 -->