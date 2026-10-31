代发 wailian999

Go:   time.Now()
来源：http://bc.szsharing.cn

Ruby: Time.now
来源：http://ip.huixiangedu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sx.jianghongdianzi.cn

[J02] 格式化输出
来源：http://gr.jianghongdianzi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xc.szsharing.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bl.hahajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fe.asd995.cn

TS:   d.toISOString()
来源：http://xq.hahajie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vg.shtwfgs.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hh.yuntaijiaju.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xd.haigaiapp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ez.szsharing.cn

[J03] 字符串解析为日期
来源：http://ml.gzmigu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gf.shtwfgs.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cx.521024.cn

JS:   new Date("2024-01-02")
来源：http://cj.hahajie.cn

TS:   new Date("2024-01-02")
来源：http://ti.9csxet.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jv.hnjuh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://eh.panjiajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://bu.9csxet.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ky.nicolike.cn

[J04] 时间戳与日期互转
来源：http://jb.hahajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cp.9csxet.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rb.haigaiapp.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ew.huixiangedu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://df.jctech888.com.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ib.bookmarksfly.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://or.huixinmuqiang.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://te.huixiangedu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ec.yuntaijiaju.cn

[J05] 时间加减（加 7 天）
来源：http://hf.muxihuayi.cn

Py:   now + timedelta(days=7)
来源：http://tf.bjjhwx.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vi.hnjuh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bw.bookmarksfly.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pu.muxihuayi.cn

Java: LocalDate.now().plusDays(7)
来源：http://ro.wgjwhj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gt.szxytkj.cn

Ruby: Time.now + 7 * 86400
来源：http://vs.gzmigu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://nw.chemitech.net.cn

[J06] 计算两时间之差
来源：http://wh.asd995.cn

Py:   (end - start).total_seconds()
来源：http://ul.yuexingan06.cn

PHP:  $end->diff($start)->days;
来源：http://ur.jctech888.com.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qp.chemitech.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://oy.panjiajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qb.colortex.cn

Go:   end.Sub(start).Hours()
来源：http://ot.yuexingan06.cn

Ruby: end - start                 # 返回秒数
来源：http://uq.wgjwhj.cn

C#:   (end - start).TotalSeconds
来源：http://ra.yuntaijiaju.cn

[J07] 比较两个日期
来源：http://gr.shtwfgs.cn

Py:   d1 < d2;  d1 == d2
来源：http://cz.shxzukj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rv.hnjuh.cn

JS:   d1.getTime() < d2.getTime()
来源：http://nd.muxihuayi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ai.shxzukj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zm.haigaiapp.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ar.jctech888.com.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wc.huixinmuqiang.cn

C#:   d1 < d2;  d1 == d2
来源：http://pk.colortex.cn

[J08] 提取年月日与星期
来源：http://fe.bjjhwx.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qy.huixiangedu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://po.shxzskj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xz.jctech888.com.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fb.lnxyls.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://je.szsharing.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://am.bookmarksfly.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cj.panjiajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sh.shxzskj.cn

[J09] 时区处理
来源：http://qd.yuntaijiaju.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rj.shtwfgs.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qc.huixiangedu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jk.hnjuh.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jp.shxzukj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kg.huixiangedu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jb.jianghongdianzi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ob.nicolike.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://st.wgjwhj.cn

[J10] 取今天 / 本月第一天
来源：http://fh.muxihuayi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zn.shtwfgs.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ng.colortex.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lt.muxihuayi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kq.gzmigu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uo.szxytkj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bg.hnjuh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zj.jctech888.com.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sh.wgjwhj.cn

================================================================================
来源：http://es.hnjuh.cn

K. JSON 与序列化
来源：http://ml.huixinmuqiang.cn

================================================================================
来源：http://an.huanxung.cn

[K01] 对象转 JSON 字符串
来源：http://xe.hnjuh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fy.szsharing.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pu.huixinmuqiang.cn

JS:   JSON.stringify(obj)
来源：http://pb.jctech888.com.cn

TS:   JSON.stringify(obj)
来源：http://if.yuntaijiaju.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://iw.huixiangedu.cn

Go:   json.Marshal(obj)
来源：http://zk.asd995.cn

Ruby: obj.to_json                                     // require "json"
来源：http://of.szxytkj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dy.hahajie.cn

[K02] JSON 字符串转对象
来源：http://vf.9csxet.cn

Py:   json.loads(s)
来源：http://gj.lnxyls.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vt.huixiangedu.cn

JS:   JSON.parse(s)
来源：http://xv.huanxung.cn

TS:   JSON.parse(s)
来源：http://yz.szsharing.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mn.szsharing.cn

Go:   json.Unmarshal(data, &v)
来源：http://pa.bookmarksfly.cn

Ruby: JSON.parse(s)
来源：http://pi.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ah.yuntaijiaju.cn

[K03] JSON 美化输出（带缩进）
来源：http://vb.shxzskj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kq.521024.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ef.wgjwhj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dd.hnjuh.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://co.wgjwhj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lp.bookmarksfly.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://az.gzmigu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://he.nicolike.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dr.muxihuayi.cn

[K04] 读取 JSON 文件
来源：http://ql.colortex.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ys.jctech888.com.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ns.hnjuh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nn.haigaiapp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wi.hnjuh.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yo.nszjky.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wa.wgjwhj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://si.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ai.521024.cn

[K05] 深拷贝对象
来源：http://nt.haigaiapp.cn

Py:   copy.deepcopy(obj)
来源：http://jn.shtwfgs.cn

PHP:  unserialize(serialize($obj));
来源：http://us.yuexingan06.cn

JS:   structuredClone(obj)
来源：http://bp.bookmarksfly.cn

TS:   structuredClone(obj)
来源：http://yr.jianghongdianzi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://at.huixiangedu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://de.hnjuh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pj.szsharing.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rw.huixiangedu.cn

[K06] 解析 URL 查询串
来源：http://ld.521024.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ix.colortex.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://iv.szsharing.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wn.haigaiapp.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pu.huixinmuqiang.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://st.chemitech.net.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qy.shtwfgs.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jj.huanxung.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yo.szxytkj.cn

[K07] 进制转换
来源：http://rr.nicolike.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qx.bookmarksfly.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rw.huixinmuqiang.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zg.huanxung.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nz.shtwfgs.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uj.huixinmuqiang.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mj.wgjwhj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ws.jianghongdianzi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gv.yuexingan06.cn

[K08] 二进制序列化（非 JSON）
来源：http://jb.chemitech.net.cn

Py:   pickle.dumps(obj)
来源：http://il.yuntaijiaju.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zb.chemitech.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://xi.huanxung.cn

TS:   v8.serialize(obj)        // Node
来源：http://qz.hnjuh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hr.panjiajie.cn

Go:   encoding/gob
来源：http://rb.yuntaijiaju.cn

Ruby: Marshal.dump(obj)
来源：http://jp.huixinmuqiang.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://oz.colortex.cn

================================================================================
来源：http://ci.jctech888.com.cn

L. 网络请求
来源：http://wa.newstarts.cn

================================================================================
来源：http://bx.asd995.cn

[L01] 发送 GET 请求
来源：http://kv.gzmigu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tj.wgjwhj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hx.jianghongdianzi.cn

JS:   await fetch(url)
来源：http://ek.nszjky.cn

TS:   await fetch(url)
来源：http://cx.nicolike.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vr.muxihuayi.cn

Go:   resp, err := http.Get(url)
来源：http://bt.panjiajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ro.gzmigu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ah.asd995.cn

[L02] 发送 POST JSON
来源：http://ag.szxytkj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gq.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ok.hnjuh.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xj.lnxyls.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bb.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ma.shxzskj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qq.newstarts.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hh.colortex.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xu.9csxet.cn

[L03] 设置自定义请求头
来源：http://zv.muxihuayi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kb.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xo.hnjuh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dp.huixiangedu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eh.asd995.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ib.shxzukj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ro.chemitech.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vm.haigaiapp.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gv.nszjky.cn

[L04] 设置超时
来源：http://vw.nicolike.cn

Py:   requests.get(url, timeout=5)
来源：http://gt.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ln.muxihuayi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ha.colortex.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uo.lnxyls.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://le.newstarts.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dn.bjjhwx.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ft.colortex.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kp.gzmigu.cn

[L05] 上传文件（multipart）
来源：http://jk.muxihuayi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zk.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tr.nszjky.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://di.huanxung.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://of.hahajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kq.asd995.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gr.newstarts.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mf.yuntaijiaju.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://le.szsharing.cn

[L06] 解析响应为 JSON
来源：http://nu.hahajie.cn

Py:   resp.json()
来源：http://gv.hnjuh.cn

PHP:  json_decode($body, true);
来源：http://cf.nszjky.cn

JS:   await resp.json()
来源：http://qp.chemitech.net.cn

TS:   await resp.json()
来源：http://bv.yuntaijiaju.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zq.shxzskj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ny.muxihuayi.cn

Ruby: JSON.parse(resp.body)
来源：http://ts.muxihuayi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qb.newstarts.cn

[L07] 处理 HTTP 状态码
来源：http://mh.lnxyls.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dz.9csxet.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ar.hnjuh.cn

JS:   resp.ok;  resp.status
来源：http://or.wgjwhj.cn

TS:   resp.ok;  resp.status
来源：http://gi.muxihuayi.cn

Java: resp.statusCode()
来源：http://lc.newstarts.cn

Go:   resp.StatusCode
来源：http://rc.szsharing.cn

Ruby: resp.code.to_i
来源：http://it.shxzukj.cn

C#:   (int)resp.StatusCode
来源：http://xa.jianghongdianzi.cn

[L08] 并发请求多个地址
来源：http://wd.asd995.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cc.szsharing.cn

PHP:  curl_multi_init() 系列
来源：http://bh.bjjhwx.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://co.jianghongdianzi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://me.jctech888.com.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dv.gzmigu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://af.huixinmuqiang.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vu.9csxet.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dy.huanxung.cn

================================================================================
来源：http://ou.wgjwhj.cn

M. 命令行 / 进程 / 环境
来源：http://ex.szxytkj.cn

================================================================================
来源：http://ec.huixiangedu.cn

[M01] 读取命令行参数
来源：http://lq.shtwfgs.cn

Py:   sys.argv[1:]
来源：http://ty.shtwfgs.cn

PHP:  $argv;  $argc;
来源：http://nk.shxzskj.cn

JS:   process.argv.slice(2)
来源：http://ig.huixinmuqiang.cn

TS:   process.argv.slice(2)
来源：http://ac.colortex.cn

Java: args 数组（main 方法参数）
来源：http://ws.chemitech.net.cn

Go:   os.Args[1:]
来源：http://tg.huixiangedu.cn

Ruby: ARGV
来源：http://oc.bjjhwx.cn

C#:   args 数组（Main 方法参数）
来源：http://qt.shtwfgs.cn

[M02] 读取环境变量
来源：http://yv.huixiangedu.cn

Py:   os.environ.get("HOME")
来源：http://hk.huixiangedu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ri.muxihuayi.cn

JS:   process.env.HOME
来源：http://lm.9csxet.cn

TS:   process.env.HOME
来源：http://vi.jctech888.com.cn

Java: System.getenv("HOME")
来源：http://ks.shxzskj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ba.shtwfgs.cn

Ruby: ENV["HOME"]
来源：http://kh.newstarts.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fy.szsharing.cn

[M03] 执行外部命令
来源：http://bp.asd995.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://go.colortex.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rr.muxihuayi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ju.newstarts.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://kx.hnjuh.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ew.shtwfgs.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wq.shxzukj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yh.hahajie.cn

C#:   Process.Start("ls", "-l");
来源：http://lf.yuntaijiaju.cn

[M04] 获取当前工作目录
来源：http://qn.chemitech.net.cn

Py:   os.getcwd()
来源：http://ob.colortex.cn

PHP:  getcwd();
来源：http://vp.yuexingan06.cn

JS:   process.cwd()
来源：http://vy.hahajie.cn

TS:   process.cwd()
来源：http://ka.panjiajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://tg.hnjuh.cn

Go:   os.Getwd()
来源：http://pv.haigaiapp.cn

Ruby: Dir.pwd
来源：http://ri.nicolike.cn

C#:   Directory.GetCurrentDirectory()
来源：http://al.haigaiapp.cn

[M05] 设置退出码
来源：http://tz.szsharing.cn

Py:   sys.exit(1)
来源：http://qq.bookmarksfly.cn

PHP:  exit(1);
来源：http://eu.colortex.cn

JS:   process.exit(1)
来源：http://jq.yuexingan06.cn

TS:   process.exit(1)
来源：http://ve.bjjhwx.cn

Java: System.exit(1)
来源：http://fl.yuexingan06.cn

Go:   os.Exit(1)
来源：http://wo.lnxyls.cn

Ruby: exit 1
来源：http://ci.bookmarksfly.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tz.yuexingan06.cn

[M06] 向标准错误输出
来源：http://ha.lnxyls.cn

Py:   print("err", file=sys.stderr)
来源：http://vz.huanxung.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qh.yuntaijiaju.cn

JS:   console.error("err")
来源：http://tv.bookmarksfly.cn

TS:   console.error("err")
来源：http://lf.hahajie.cn

Java: System.err.println("err")
来源：http://ke.shxzskj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rq.haigaiapp.cn

Ruby: warn "err"
来源：http://lk.shxzskj.cn

C#:   Console.Error.WriteLine("err")
来源：http://en.szsharing.cn

[M07] 判断是否为主入口
来源：http://ln.shxzskj.cn

Py:   if __name__ == "__main__":
来源：http://hi.shxzukj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jl.muxihuayi.cn

JS:   require.main === module
来源：http://jf.newstarts.cn

TS:   require.main === module
来源：http://il.jianghongdianzi.cn

Java: public static void main(String[] args)
来源：http://uy.panjiajie.cn

Go:   func main()
来源：http://od.hnjuh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pe.colortex.cn

C#:   static void Main(string[] args)
来源：http://eh.jianghongdianzi.cn


<!-- 参考信息 -->