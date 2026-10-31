代发 wailian999

Go:   time.Now()
来源：http://bm.szxytkj.cn

Ruby: Time.now
来源：http://rl.yuexingan06.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lc.nszjky.cn

[J02] 格式化输出
来源：http://an.nicolike.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qa.haigaiapp.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kx.yuntaijiaju.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mm.szsharing.cn

TS:   d.toISOString()
来源：http://sw.huixiangedu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ug.shtwfgs.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://aa.huanxung.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mv.hnjuh.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://re.lnxyls.cn

[J03] 字符串解析为日期
来源：http://ue.bjjhwx.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rv.bjjhwx.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xr.gzmigu.cn

JS:   new Date("2024-01-02")
来源：http://qv.shtwfgs.cn

TS:   new Date("2024-01-02")
来源：http://hl.wgjwhj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://tq.jctech888.com.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sb.newstarts.cn

Ruby: Date.parse("2024-01-02")
来源：http://yz.shtwfgs.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kh.yuntaijiaju.cn

[J04] 时间戳与日期互转
来源：http://bp.bookmarksfly.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qx.gzmigu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wl.shxzukj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://oa.yuntaijiaju.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ta.huanxung.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lj.newstarts.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://iy.chemitech.net.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yz.panjiajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://oc.asd995.cn

[J05] 时间加减（加 7 天）
来源：http://ax.gzmigu.cn

Py:   now + timedelta(days=7)
来源：http://dk.lnxyls.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ii.yuntaijiaju.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ls.shxzskj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hp.hahajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://zz.lnxyls.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qk.shxzukj.cn

Ruby: Time.now + 7 * 86400
来源：http://qt.szxytkj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://uu.jianghongdianzi.cn

[J06] 计算两时间之差
来源：http://ik.hahajie.cn

Py:   (end - start).total_seconds()
来源：http://io.colortex.cn

PHP:  $end->diff($start)->days;
来源：http://us.shxzukj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uv.newstarts.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xa.nicolike.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zb.521024.cn

Go:   end.Sub(start).Hours()
来源：http://lf.huanxung.cn

Ruby: end - start                 # 返回秒数
来源：http://ih.huixiangedu.cn

C#:   (end - start).TotalSeconds
来源：http://ez.chemitech.net.cn

[J07] 比较两个日期
来源：http://fo.nicolike.cn

Py:   d1 < d2;  d1 == d2
来源：http://fy.521024.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xv.lnxyls.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xg.asd995.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qx.szxytkj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dg.nszjky.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jm.521024.cn

Ruby: d1 < d2;  d1 == d2
来源：http://rj.shtwfgs.cn

C#:   d1 < d2;  d1 == d2
来源：http://gy.gzmigu.cn

[J08] 提取年月日与星期
来源：http://gt.bookmarksfly.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ev.wgjwhj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wy.wgjwhj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fs.shxzukj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lc.bjjhwx.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kf.newstarts.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pm.hahajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cg.newstarts.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qt.shxzskj.cn

[J09] 时区处理
来源：http://yw.bookmarksfly.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yh.hahajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://es.nicolike.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pt.huixinmuqiang.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qn.lnxyls.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hw.hahajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sg.huanxung.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://oy.szxytkj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://at.muxihuayi.cn

[J10] 取今天 / 本月第一天
来源：http://pq.bookmarksfly.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://yh.huanxung.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qo.wgjwhj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kc.huixiangedu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xa.jctech888.com.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yt.wgjwhj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nz.yuexingan06.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ot.shtwfgs.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rp.jctech888.com.cn

================================================================================
来源：http://he.gzmigu.cn

K. JSON 与序列化
来源：http://rn.lnxyls.cn

================================================================================
来源：http://bi.hahajie.cn

[K01] 对象转 JSON 字符串
来源：http://ix.newstarts.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rn.hahajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yc.panjiajie.cn

JS:   JSON.stringify(obj)
来源：http://if.newstarts.cn

TS:   JSON.stringify(obj)
来源：http://xr.shtwfgs.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hv.chemitech.net.cn

Go:   json.Marshal(obj)
来源：http://jc.huixinmuqiang.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ks.shxzskj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lj.shtwfgs.cn

[K02] JSON 字符串转对象
来源：http://jo.yuexingan06.cn

Py:   json.loads(s)
来源：http://bt.yuexingan06.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jm.muxihuayi.cn

JS:   JSON.parse(s)
来源：http://uk.shtwfgs.cn

TS:   JSON.parse(s)
来源：http://zm.haigaiapp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zv.huanxung.cn

Go:   json.Unmarshal(data, &v)
来源：http://gd.newstarts.cn

Ruby: JSON.parse(s)
来源：http://er.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xm.szsharing.cn

[K03] JSON 美化输出（带缩进）
来源：http://js.newstarts.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xc.asd995.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bv.yuntaijiaju.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://tg.nicolike.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bc.newstarts.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pk.haigaiapp.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qm.jctech888.com.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ez.521024.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xo.521024.cn

[K04] 读取 JSON 文件
来源：http://oo.hahajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lm.huixiangedu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ih.bjjhwx.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://or.bjjhwx.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tk.yuexingan06.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sh.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://os.bjjhwx.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fo.asd995.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rt.shtwfgs.cn

[K05] 深拷贝对象
来源：http://fy.521024.cn

Py:   copy.deepcopy(obj)
来源：http://eh.bjjhwx.cn

PHP:  unserialize(serialize($obj));
来源：http://kh.newstarts.cn

JS:   structuredClone(obj)
来源：http://db.jianghongdianzi.cn

TS:   structuredClone(obj)
来源：http://vn.bookmarksfly.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rd.bjjhwx.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ux.asd995.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ec.wgjwhj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://bj.hahajie.cn

[K06] 解析 URL 查询串
来源：http://ks.huanxung.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://is.nszjky.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://oy.huanxung.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ow.shtwfgs.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eh.shtwfgs.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ca.bjjhwx.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qu.muxihuayi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cc.hahajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pf.gzmigu.cn

[K07] 进制转换
来源：http://uw.newstarts.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ph.huixiangedu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mk.haigaiapp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mz.wgjwhj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tu.muxihuayi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fs.haigaiapp.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wj.hnjuh.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://va.asd995.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yg.bjjhwx.cn

[K08] 二进制序列化（非 JSON）
来源：http://xe.hahajie.cn

Py:   pickle.dumps(obj)
来源：http://wr.jianghongdianzi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://eo.jctech888.com.cn

JS:   v8.serialize(obj)        // Node
来源：http://nf.9csxet.cn

TS:   v8.serialize(obj)        // Node
来源：http://bn.colortex.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ls.szsharing.cn

Go:   encoding/gob
来源：http://ms.wgjwhj.cn

Ruby: Marshal.dump(obj)
来源：http://ap.jianghongdianzi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ic.szxytkj.cn

================================================================================
来源：http://kp.nszjky.cn

L. 网络请求
来源：http://kc.szxytkj.cn

================================================================================
来源：http://zo.shtwfgs.cn

[L01] 发送 GET 请求
来源：http://ke.9csxet.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rk.asd995.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zo.9csxet.cn

JS:   await fetch(url)
来源：http://sr.szxytkj.cn

TS:   await fetch(url)
来源：http://qp.hnjuh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fw.huixiangedu.cn

Go:   resp, err := http.Get(url)
来源：http://rq.hahajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://nr.szsharing.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qb.lnxyls.cn

[L02] 发送 POST JSON
来源：http://hh.shxzskj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xb.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ed.colortex.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yo.bookmarksfly.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kh.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qu.szxytkj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://og.nszjky.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://us.gzmigu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xq.yuexingan06.cn

[L03] 设置自定义请求头
来源：http://ob.huixiangedu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pf.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tq.szxytkj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ox.hnjuh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yp.521024.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yn.panjiajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mn.jctech888.com.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gm.hnjuh.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yn.wgjwhj.cn

[L04] 设置超时
来源：http://cg.gzmigu.cn

Py:   requests.get(url, timeout=5)
来源：http://kz.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cy.newstarts.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ro.szsharing.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qe.9csxet.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ef.nicolike.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ih.yuntaijiaju.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ex.haigaiapp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kg.shxzukj.cn

[L05] 上传文件（multipart）
来源：http://cs.yuexingan06.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ff.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ot.yuntaijiaju.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vv.chemitech.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xo.szxytkj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://px.huanxung.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mo.jianghongdianzi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://oh.huanxung.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mx.huanxung.cn

[L06] 解析响应为 JSON
来源：http://xh.shxzukj.cn

Py:   resp.json()
来源：http://vh.shxzukj.cn

PHP:  json_decode($body, true);
来源：http://nh.panjiajie.cn

JS:   await resp.json()
来源：http://vz.haigaiapp.cn

TS:   await resp.json()
来源：http://dw.521024.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ob.jctech888.com.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kp.hahajie.cn

Ruby: JSON.parse(resp.body)
来源：http://ht.newstarts.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://et.9csxet.cn

[L07] 处理 HTTP 状态码
来源：http://hk.szsharing.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://th.jianghongdianzi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wd.szxytkj.cn

JS:   resp.ok;  resp.status
来源：http://xi.haigaiapp.cn

TS:   resp.ok;  resp.status
来源：http://qj.shxzukj.cn

Java: resp.statusCode()
来源：http://ji.yuntaijiaju.cn

Go:   resp.StatusCode
来源：http://ph.nszjky.cn

Ruby: resp.code.to_i
来源：http://ni.colortex.cn

C#:   (int)resp.StatusCode
来源：http://ru.panjiajie.cn

[L08] 并发请求多个地址
来源：http://df.wgjwhj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qi.gzmigu.cn

PHP:  curl_multi_init() 系列
来源：http://ud.hnjuh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tl.szxytkj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wd.shtwfgs.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mi.szsharing.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pz.bjjhwx.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bq.wgjwhj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hk.yuntaijiaju.cn

================================================================================
来源：http://nh.shxzskj.cn

M. 命令行 / 进程 / 环境
来源：http://jq.hahajie.cn

================================================================================
来源：http://et.bjjhwx.cn

[M01] 读取命令行参数
来源：http://vj.huanxung.cn

Py:   sys.argv[1:]
来源：http://uf.gzmigu.cn

PHP:  $argv;  $argc;
来源：http://tz.521024.cn

JS:   process.argv.slice(2)
来源：http://tf.hnjuh.cn

TS:   process.argv.slice(2)
来源：http://kn.asd995.cn

Java: args 数组（main 方法参数）
来源：http://cw.colortex.cn

Go:   os.Args[1:]
来源：http://ta.yuexingan06.cn

Ruby: ARGV
来源：http://iq.muxihuayi.cn

C#:   args 数组（Main 方法参数）
来源：http://qe.jianghongdianzi.cn

[M02] 读取环境变量
来源：http://hm.nszjky.cn

Py:   os.environ.get("HOME")
来源：http://tn.jctech888.com.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cv.haigaiapp.cn

JS:   process.env.HOME
来源：http://ar.szxytkj.cn

TS:   process.env.HOME
来源：http://sk.yuexingan06.cn

Java: System.getenv("HOME")
来源：http://sb.colortex.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nh.hahajie.cn

Ruby: ENV["HOME"]
来源：http://gn.hahajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ij.newstarts.cn

[M03] 执行外部命令
来源：http://dg.huixiangedu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ry.521024.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ds.shxzskj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hg.szsharing.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://hw.chemitech.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ct.newstarts.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://el.shtwfgs.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ab.huanxung.cn

C#:   Process.Start("ls", "-l");
来源：http://ub.asd995.cn

[M04] 获取当前工作目录
来源：http://bf.bjjhwx.cn

Py:   os.getcwd()
来源：http://xi.jctech888.com.cn

PHP:  getcwd();
来源：http://xr.asd995.cn

JS:   process.cwd()
来源：http://nm.shxzukj.cn

TS:   process.cwd()
来源：http://cj.shxzskj.cn

Java: Path.of("").toAbsolutePath()
来源：http://yj.jianghongdianzi.cn

Go:   os.Getwd()
来源：http://qg.nszjky.cn

Ruby: Dir.pwd
来源：http://ff.9csxet.cn

C#:   Directory.GetCurrentDirectory()
来源：http://cp.bjjhwx.cn

[M05] 设置退出码
来源：http://wi.huixiangedu.cn

Py:   sys.exit(1)
来源：http://hr.newstarts.cn

PHP:  exit(1);
来源：http://kx.szxytkj.cn

JS:   process.exit(1)
来源：http://dv.huixinmuqiang.cn

TS:   process.exit(1)
来源：http://tc.chemitech.net.cn

Java: System.exit(1)
来源：http://ns.9csxet.cn

Go:   os.Exit(1)
来源：http://ul.jctech888.com.cn

Ruby: exit 1
来源：http://zc.szxytkj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://se.9csxet.cn

[M06] 向标准错误输出
来源：http://ld.bookmarksfly.cn

Py:   print("err", file=sys.stderr)
来源：http://nf.colortex.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://nb.shxzskj.cn

JS:   console.error("err")
来源：http://vy.nszjky.cn

TS:   console.error("err")
来源：http://kw.shtwfgs.cn

Java: System.err.println("err")
来源：http://vf.gzmigu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dq.szxytkj.cn

Ruby: warn "err"
来源：http://re.shtwfgs.cn

C#:   Console.Error.WriteLine("err")
来源：http://uk.muxihuayi.cn

[M07] 判断是否为主入口
来源：http://pj.nszjky.cn

Py:   if __name__ == "__main__":
来源：http://de.chemitech.net.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nn.nszjky.cn

JS:   require.main === module
来源：http://wh.huixiangedu.cn

TS:   require.main === module
来源：http://pf.chemitech.net.cn

Java: public static void main(String[] args)
来源：http://ba.huixiangedu.cn

Go:   func main()
来源：http://fr.jctech888.com.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vg.muxihuayi.cn

C#:   static void Main(string[] args)
来源：http://tr.yuntaijiaju.cn


<!-- 参考信息 -->