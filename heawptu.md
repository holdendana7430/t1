代发 wailian999

Go:   time.Now()
来源：http://wl.asd995.cn

Ruby: Time.now
来源：http://if.newstarts.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vq.nszjky.cn

[J02] 格式化输出
来源：http://rf.wgjwhj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wm.shxzukj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pu.gzmigu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jz.haigaiapp.cn

TS:   d.toISOString()
来源：http://mf.shxzskj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yh.szsharing.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cl.gzmigu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cj.asd995.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mq.bjjhwx.cn

[J03] 字符串解析为日期
来源：http://jz.newstarts.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ff.wgjwhj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ot.asd995.cn

JS:   new Date("2024-01-02")
来源：http://pu.huixinmuqiang.cn

TS:   new Date("2024-01-02")
来源：http://zo.newstarts.cn

Java: LocalDate.parse("2024-01-02")
来源：http://sk.shxzskj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fk.shxzskj.cn

Ruby: Date.parse("2024-01-02")
来源：http://mo.szxytkj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ub.gzmigu.cn

[J04] 时间戳与日期互转
来源：http://lz.hahajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yr.muxihuayi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://he.chemitech.net.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://io.muxihuayi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://td.huixinmuqiang.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vg.wgjwhj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ty.bookmarksfly.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xs.haigaiapp.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pq.chemitech.net.cn

[J05] 时间加减（加 7 天）
来源：http://vf.521024.cn

Py:   now + timedelta(days=7)
来源：http://nf.chemitech.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://eb.huixinmuqiang.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cm.hnjuh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wc.gzmigu.cn

Java: LocalDate.now().plusDays(7)
来源：http://ij.gzmigu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qi.szsharing.cn

Ruby: Time.now + 7 * 86400
来源：http://aq.szxytkj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hw.jianghongdianzi.cn

[J06] 计算两时间之差
来源：http://jl.chemitech.net.cn

Py:   (end - start).total_seconds()
来源：http://yt.9csxet.cn

PHP:  $end->diff($start)->days;
来源：http://yc.lnxyls.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fb.jianghongdianzi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://le.asd995.cn

Java: Duration.between(start, end).toSeconds()
来源：http://aq.jianghongdianzi.cn

Go:   end.Sub(start).Hours()
来源：http://ay.9csxet.cn

Ruby: end - start                 # 返回秒数
来源：http://kj.huixinmuqiang.cn

C#:   (end - start).TotalSeconds
来源：http://sd.chemitech.net.cn

[J07] 比较两个日期
来源：http://te.jianghongdianzi.cn

Py:   d1 < d2;  d1 == d2
来源：http://gr.nszjky.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fn.haigaiapp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fn.jianghongdianzi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mm.shtwfgs.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mf.panjiajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://np.gzmigu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://yt.hahajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://se.nszjky.cn

[J08] 提取年月日与星期
来源：http://lh.9csxet.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://va.jianghongdianzi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ug.yuexingan06.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mk.asd995.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tx.szsharing.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qd.chemitech.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cx.lnxyls.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://iv.bjjhwx.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wj.jianghongdianzi.cn

[J09] 时区处理
来源：http://yr.9csxet.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hd.chemitech.net.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vf.hahajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qd.nicolike.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mm.shxzukj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vn.jianghongdianzi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jd.lnxyls.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qn.hahajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nh.colortex.cn

[J10] 取今天 / 本月第一天
来源：http://po.shxzukj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://iv.521024.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ho.lnxyls.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zh.asd995.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://eb.shxzukj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ct.521024.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pj.szsharing.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sw.huixiangedu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://br.huixiangedu.cn

================================================================================
来源：http://ro.nszjky.cn

K. JSON 与序列化
来源：http://dp.nicolike.cn

================================================================================
来源：http://qr.9csxet.cn

[K01] 对象转 JSON 字符串
来源：http://qz.bookmarksfly.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rc.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ff.hahajie.cn

JS:   JSON.stringify(obj)
来源：http://wd.yuexingan06.cn

TS:   JSON.stringify(obj)
来源：http://mn.colortex.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yx.hahajie.cn

Go:   json.Marshal(obj)
来源：http://xc.huanxung.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ki.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yj.bjjhwx.cn

[K02] JSON 字符串转对象
来源：http://vh.nicolike.cn

Py:   json.loads(s)
来源：http://xa.hnjuh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ck.jctech888.com.cn

JS:   JSON.parse(s)
来源：http://ig.huixinmuqiang.cn

TS:   JSON.parse(s)
来源：http://lr.huixiangedu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://es.shxzukj.cn

Go:   json.Unmarshal(data, &v)
来源：http://zm.521024.cn

Ruby: JSON.parse(s)
来源：http://zc.colortex.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lp.nicolike.cn

[K03] JSON 美化输出（带缩进）
来源：http://do.jianghongdianzi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dl.nszjky.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dl.haigaiapp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ii.shxzskj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://lz.huixiangedu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wr.hnjuh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cc.shtwfgs.cn

Ruby: JSON.pretty_generate(obj)
来源：http://uv.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jd.nicolike.cn

[K04] 读取 JSON 文件
来源：http://rh.gzmigu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kz.yuexingan06.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ki.huixinmuqiang.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mk.shxzskj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vd.colortex.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ji.521024.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ij.panjiajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://sl.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qu.nszjky.cn

[K05] 深拷贝对象
来源：http://um.muxihuayi.cn

Py:   copy.deepcopy(obj)
来源：http://hc.nicolike.cn

PHP:  unserialize(serialize($obj));
来源：http://hy.haigaiapp.cn

JS:   structuredClone(obj)
来源：http://ds.muxihuayi.cn

TS:   structuredClone(obj)
来源：http://aq.yuntaijiaju.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wm.szxytkj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ce.chemitech.net.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ux.bjjhwx.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dn.hahajie.cn

[K06] 解析 URL 查询串
来源：http://uo.jianghongdianzi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://iv.panjiajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gt.521024.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://al.hnjuh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ys.panjiajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kg.yuexingan06.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wf.wgjwhj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ax.jianghongdianzi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://up.bjjhwx.cn

[K07] 进制转换
来源：http://zi.shtwfgs.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://of.shxzskj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qo.gzmigu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kl.lnxyls.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ii.huixiangedu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uf.bookmarksfly.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zz.yuexingan06.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rs.521024.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xx.newstarts.cn

[K08] 二进制序列化（非 JSON）
来源：http://sh.szxytkj.cn

Py:   pickle.dumps(obj)
来源：http://og.gzmigu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://uc.jctech888.com.cn

JS:   v8.serialize(obj)        // Node
来源：http://gb.521024.cn

TS:   v8.serialize(obj)        // Node
来源：http://cb.muxihuayi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qa.yuntaijiaju.cn

Go:   encoding/gob
来源：http://ic.wgjwhj.cn

Ruby: Marshal.dump(obj)
来源：http://qo.hahajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wt.szsharing.cn

================================================================================
来源：http://cg.yuexingan06.cn

L. 网络请求
来源：http://ed.9csxet.cn

================================================================================
来源：http://rc.szxytkj.cn

[L01] 发送 GET 请求
来源：http://an.huixinmuqiang.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lg.hnjuh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lq.chemitech.net.cn

JS:   await fetch(url)
来源：http://sy.colortex.cn

TS:   await fetch(url)
来源：http://ds.bjjhwx.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sq.jianghongdianzi.cn

Go:   resp, err := http.Get(url)
来源：http://kx.muxihuayi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xq.521024.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xu.bjjhwx.cn

[L02] 发送 POST JSON
来源：http://nt.szsharing.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zi.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ny.chemitech.net.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bw.nszjky.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oe.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cz.gzmigu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mt.9csxet.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kp.9csxet.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tk.huanxung.cn

[L03] 设置自定义请求头
来源：http://bk.colortex.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hi.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://la.wgjwhj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://va.shxzukj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ez.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xv.hahajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rk.9csxet.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sq.yuexingan06.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rk.panjiajie.cn

[L04] 设置超时
来源：http://yt.szsharing.cn

Py:   requests.get(url, timeout=5)
来源：http://rx.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cx.haigaiapp.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wu.wgjwhj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wl.shtwfgs.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rn.shxzskj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ss.jianghongdianzi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mr.huixinmuqiang.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zu.szxytkj.cn

[L05] 上传文件（multipart）
来源：http://kt.bjjhwx.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ll.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dn.521024.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://us.bjjhwx.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bc.shxzskj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ya.szsharing.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jc.521024.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vl.521024.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qi.shtwfgs.cn

[L06] 解析响应为 JSON
来源：http://nb.yuexingan06.cn

Py:   resp.json()
来源：http://rl.haigaiapp.cn

PHP:  json_decode($body, true);
来源：http://lz.hahajie.cn

JS:   await resp.json()
来源：http://iw.muxihuayi.cn

TS:   await resp.json()
来源：http://yk.9csxet.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ub.9csxet.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://js.huixiangedu.cn

Ruby: JSON.parse(resp.body)
来源：http://ut.asd995.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://un.hnjuh.cn

[L07] 处理 HTTP 状态码
来源：http://vu.nszjky.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jz.jctech888.com.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://me.colortex.cn

JS:   resp.ok;  resp.status
来源：http://rc.colortex.cn

TS:   resp.ok;  resp.status
来源：http://gv.wgjwhj.cn

Java: resp.statusCode()
来源：http://hc.chemitech.net.cn

Go:   resp.StatusCode
来源：http://cs.gzmigu.cn

Ruby: resp.code.to_i
来源：http://ad.gzmigu.cn

C#:   (int)resp.StatusCode
来源：http://xw.bookmarksfly.cn

[L08] 并发请求多个地址
来源：http://wh.jctech888.com.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://id.shxzukj.cn

PHP:  curl_multi_init() 系列
来源：http://vq.bookmarksfly.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uo.wgjwhj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ds.huixinmuqiang.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wt.bjjhwx.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fq.huanxung.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ns.nicolike.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ro.colortex.cn

================================================================================
来源：http://nj.panjiajie.cn

M. 命令行 / 进程 / 环境
来源：http://mz.szxytkj.cn

================================================================================
来源：http://pu.muxihuayi.cn

[M01] 读取命令行参数
来源：http://my.bjjhwx.cn

Py:   sys.argv[1:]
来源：http://xp.shxzskj.cn

PHP:  $argv;  $argc;
来源：http://qb.yuexingan06.cn

JS:   process.argv.slice(2)
来源：http://xh.muxihuayi.cn

TS:   process.argv.slice(2)
来源：http://wk.9csxet.cn

Java: args 数组（main 方法参数）
来源：http://sd.hnjuh.cn

Go:   os.Args[1:]
来源：http://wf.jctech888.com.cn

Ruby: ARGV
来源：http://cs.szsharing.cn

C#:   args 数组（Main 方法参数）
来源：http://ri.gzmigu.cn

[M02] 读取环境变量
来源：http://sk.colortex.cn

Py:   os.environ.get("HOME")
来源：http://mk.muxihuayi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pb.haigaiapp.cn

JS:   process.env.HOME
来源：http://ef.wgjwhj.cn

TS:   process.env.HOME
来源：http://se.shtwfgs.cn

Java: System.getenv("HOME")
来源：http://yq.nicolike.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vg.bookmarksfly.cn

Ruby: ENV["HOME"]
来源：http://rp.hnjuh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oc.lnxyls.cn

[M03] 执行外部命令
来源：http://tb.nicolike.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://oy.nszjky.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://de.nicolike.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://yg.shxzskj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ta.colortex.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fe.newstarts.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://kb.chemitech.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vb.lnxyls.cn

C#:   Process.Start("ls", "-l");
来源：http://kf.huanxung.cn

[M04] 获取当前工作目录
来源：http://wy.jctech888.com.cn

Py:   os.getcwd()
来源：http://ib.gzmigu.cn

PHP:  getcwd();
来源：http://en.asd995.cn

JS:   process.cwd()
来源：http://eq.chemitech.net.cn

TS:   process.cwd()
来源：http://yv.muxihuayi.cn

Java: Path.of("").toAbsolutePath()
来源：http://xi.bjjhwx.cn

Go:   os.Getwd()
来源：http://em.huixiangedu.cn

Ruby: Dir.pwd
来源：http://zz.9csxet.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ux.huixiangedu.cn

[M05] 设置退出码
来源：http://uy.szsharing.cn

Py:   sys.exit(1)
来源：http://md.yuntaijiaju.cn

PHP:  exit(1);
来源：http://at.yuntaijiaju.cn

JS:   process.exit(1)
来源：http://wv.asd995.cn

TS:   process.exit(1)
来源：http://kr.521024.cn

Java: System.exit(1)
来源：http://gb.panjiajie.cn

Go:   os.Exit(1)
来源：http://mf.huanxung.cn

Ruby: exit 1
来源：http://hl.huanxung.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nw.bookmarksfly.cn

[M06] 向标准错误输出
来源：http://wz.yuexingan06.cn

Py:   print("err", file=sys.stderr)
来源：http://rj.szxytkj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ok.huanxung.cn

JS:   console.error("err")
来源：http://mw.nszjky.cn

TS:   console.error("err")
来源：http://uj.gzmigu.cn

Java: System.err.println("err")
来源：http://yk.huixiangedu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dt.huixiangedu.cn

Ruby: warn "err"
来源：http://jb.colortex.cn

C#:   Console.Error.WriteLine("err")
来源：http://gx.nicolike.cn

[M07] 判断是否为主入口
来源：http://nu.jianghongdianzi.cn

Py:   if __name__ == "__main__":
来源：http://kr.hnjuh.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ol.gzmigu.cn

JS:   require.main === module
来源：http://ie.asd995.cn

TS:   require.main === module
来源：http://lw.bjjhwx.cn

Java: public static void main(String[] args)
来源：http://ms.shxzukj.cn

Go:   func main()
来源：http://hk.hnjuh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qu.jianghongdianzi.cn

C#:   static void Main(string[] args)
来源：http://xj.yuntaijiaju.cn


<!-- 参考信息 -->