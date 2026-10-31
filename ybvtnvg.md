代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ni.yuntaijiaju.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jl.haigaiapp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pj.wgjwhj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://js.9csxet.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://as.chemitech.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xq.wgjwhj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ts.jianghongdianzi.cn

================================================================================
来源：http://sn.jctech888.com.cn

J. 日期与时间
来源：http://oz.bookmarksfly.cn

================================================================================
来源：http://ho.shtwfgs.cn

[J01] 获取当前时间
来源：http://hp.jianghongdianzi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wu.colortex.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://aw.yuntaijiaju.cn

JS:   new Date();  Date.now()
来源：http://pv.panjiajie.cn

TS:   new Date();  Date.now()
来源：http://uj.shxzukj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://iu.521024.cn

Go:   time.Now()
来源：http://sp.chemitech.net.cn

Ruby: Time.now
来源：http://wv.bjjhwx.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://eq.nszjky.cn

[J02] 格式化输出
来源：http://xc.nicolike.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ys.haigaiapp.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lo.huixinmuqiang.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mz.bjjhwx.cn

TS:   d.toISOString()
来源：http://dk.lnxyls.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ay.panjiajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gs.szxytkj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cw.nicolike.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ej.jctech888.com.cn

[J03] 字符串解析为日期
来源：http://sa.huixiangedu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://go.asd995.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wn.gzmigu.cn

JS:   new Date("2024-01-02")
来源：http://tz.haigaiapp.cn

TS:   new Date("2024-01-02")
来源：http://jc.colortex.cn

Java: LocalDate.parse("2024-01-02")
来源：http://av.colortex.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jc.panjiajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://gn.huixinmuqiang.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gv.huanxung.cn

[J04] 时间戳与日期互转
来源：http://qv.wgjwhj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yg.shxzskj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://oj.hnjuh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://je.hnjuh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hp.muxihuayi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gp.nicolike.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zn.panjiajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rp.huixiangedu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://as.lnxyls.cn

[J05] 时间加减（加 7 天）
来源：http://vd.haigaiapp.cn

Py:   now + timedelta(days=7)
来源：http://wl.colortex.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kk.wgjwhj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vq.521024.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://at.szxytkj.cn

Java: LocalDate.now().plusDays(7)
来源：http://rk.newstarts.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lc.asd995.cn

Ruby: Time.now + 7 * 86400
来源：http://ec.yuexingan06.cn

C#:   DateTime.Now.AddDays(7)
来源：http://uo.shtwfgs.cn

[J06] 计算两时间之差
来源：http://ut.hahajie.cn

Py:   (end - start).total_seconds()
来源：http://hd.nicolike.cn

PHP:  $end->diff($start)->days;
来源：http://qq.huixiangedu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ag.9csxet.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ua.shxzskj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rr.szxytkj.cn

Go:   end.Sub(start).Hours()
来源：http://wm.yuexingan06.cn

Ruby: end - start                 # 返回秒数
来源：http://zi.9csxet.cn

C#:   (end - start).TotalSeconds
来源：http://vo.shxzskj.cn

[J07] 比较两个日期
来源：http://sw.521024.cn

Py:   d1 < d2;  d1 == d2
来源：http://nq.lnxyls.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zq.asd995.cn

JS:   d1.getTime() < d2.getTime()
来源：http://dy.hnjuh.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ez.521024.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ca.huanxung.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mq.wgjwhj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bb.shxzskj.cn

C#:   d1 < d2;  d1 == d2
来源：http://fz.jctech888.com.cn

[J08] 提取年月日与星期
来源：http://ok.9csxet.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ni.chemitech.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://eo.chemitech.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jx.wgjwhj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://es.colortex.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://up.jctech888.com.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zq.asd995.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kn.lnxyls.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fn.nszjky.cn

[J09] 时区处理
来源：http://zt.521024.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qv.9csxet.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ie.shxzskj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sf.shxzukj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eb.newstarts.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rq.shxzukj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pj.haigaiapp.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qk.szxytkj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xv.asd995.cn

[J10] 取今天 / 本月第一天
来源：http://zk.huixinmuqiang.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://lm.9csxet.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hx.huanxung.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xc.nicolike.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nl.yuexingan06.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rm.haigaiapp.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lo.huixinmuqiang.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://if.yuexingan06.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rq.muxihuayi.cn

================================================================================
来源：http://tr.huixiangedu.cn

K. JSON 与序列化
来源：http://al.shxzukj.cn

================================================================================
来源：http://ah.huanxung.cn

[K01] 对象转 JSON 字符串
来源：http://wd.muxihuayi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://so.521024.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pz.wgjwhj.cn

JS:   JSON.stringify(obj)
来源：http://ys.nicolike.cn

TS:   JSON.stringify(obj)
来源：http://fz.hnjuh.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lr.lnxyls.cn

Go:   json.Marshal(obj)
来源：http://iv.nszjky.cn

Ruby: obj.to_json                                     // require "json"
来源：http://du.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yg.521024.cn

[K02] JSON 字符串转对象
来源：http://xz.bjjhwx.cn

Py:   json.loads(s)
来源：http://jl.jctech888.com.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ie.bookmarksfly.cn

JS:   JSON.parse(s)
来源：http://rm.wgjwhj.cn

TS:   JSON.parse(s)
来源：http://ga.jianghongdianzi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ub.521024.cn

Go:   json.Unmarshal(data, &v)
来源：http://rn.bjjhwx.cn

Ruby: JSON.parse(s)
来源：http://ib.asd995.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jc.nszjky.cn

[K03] JSON 美化输出（带缩进）
来源：http://kx.wgjwhj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nb.9csxet.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://if.shtwfgs.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fw.bjjhwx.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mc.szsharing.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mg.huixinmuqiang.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ww.9csxet.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nh.asd995.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://oq.gzmigu.cn

[K04] 读取 JSON 文件
来源：http://fk.shxzskj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vv.huanxung.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fk.hnjuh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bt.chemitech.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gb.newstarts.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nz.9csxet.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pq.shtwfgs.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://kx.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ly.jianghongdianzi.cn

[K05] 深拷贝对象
来源：http://wb.jctech888.com.cn

Py:   copy.deepcopy(obj)
来源：http://qh.hnjuh.cn

PHP:  unserialize(serialize($obj));
来源：http://sv.szsharing.cn

JS:   structuredClone(obj)
来源：http://eo.shtwfgs.cn

TS:   structuredClone(obj)
来源：http://fe.wgjwhj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bg.nicolike.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://te.nszjky.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cz.szxytkj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://li.jctech888.com.cn

[K06] 解析 URL 查询串
来源：http://za.nicolike.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://we.nszjky.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zt.wgjwhj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://po.huanxung.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ow.newstarts.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vu.yuntaijiaju.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qu.9csxet.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wi.jianghongdianzi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ae.panjiajie.cn

[K07] 进制转换
来源：http://rh.nszjky.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bg.lnxyls.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://id.hnjuh.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://or.wgjwhj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rg.newstarts.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lh.jianghongdianzi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ib.gzmigu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mn.shxzukj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ec.haigaiapp.cn

[K08] 二进制序列化（非 JSON）
来源：http://li.gzmigu.cn

Py:   pickle.dumps(obj)
来源：http://at.shxzukj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fv.bookmarksfly.cn

JS:   v8.serialize(obj)        // Node
来源：http://fa.chemitech.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://yj.muxihuayi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ee.jianghongdianzi.cn

Go:   encoding/gob
来源：http://cf.9csxet.cn

Ruby: Marshal.dump(obj)
来源：http://pp.shxzskj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://eh.muxihuayi.cn

================================================================================
来源：http://ll.panjiajie.cn

L. 网络请求
来源：http://do.jctech888.com.cn

================================================================================
来源：http://ps.colortex.cn

[L01] 发送 GET 请求
来源：http://cr.chemitech.net.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xq.szsharing.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ok.colortex.cn

JS:   await fetch(url)
来源：http://ev.shtwfgs.cn

TS:   await fetch(url)
来源：http://ys.szsharing.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://th.jianghongdianzi.cn

Go:   resp, err := http.Get(url)
来源：http://cw.gzmigu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qq.jctech888.com.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ch.szxytkj.cn

[L02] 发送 POST JSON
来源：http://th.chemitech.net.cn

Py:   requests.post(url, json={"a": 1})
来源：http://lz.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nj.yuntaijiaju.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sd.szxytkj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cc.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ru.newstarts.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://aw.521024.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ps.newstarts.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tf.muxihuayi.cn

[L03] 设置自定义请求头
来源：http://hf.nicolike.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xd.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ns.newstarts.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wb.nicolike.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://px.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bu.jianghongdianzi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tc.521024.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pk.gzmigu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vy.jianghongdianzi.cn

[L04] 设置超时
来源：http://dg.521024.cn

Py:   requests.get(url, timeout=5)
来源：http://mm.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://na.jctech888.com.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cz.szxytkj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sd.colortex.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fm.lnxyls.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xu.jctech888.com.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qo.shtwfgs.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://st.bookmarksfly.cn

[L05] 上传文件（multipart）
来源：http://sz.bjjhwx.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tz.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pv.shxzukj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wg.9csxet.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sg.huixiangedu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gq.shtwfgs.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://np.9csxet.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dc.lnxyls.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hy.9csxet.cn

[L06] 解析响应为 JSON
来源：http://vv.huanxung.cn

Py:   resp.json()
来源：http://vo.yuntaijiaju.cn

PHP:  json_decode($body, true);
来源：http://hl.bjjhwx.cn

JS:   await resp.json()
来源：http://ja.bookmarksfly.cn

TS:   await resp.json()
来源：http://jr.521024.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hn.huanxung.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ms.bookmarksfly.cn

Ruby: JSON.parse(resp.body)
来源：http://eu.panjiajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ro.huanxung.cn

[L07] 处理 HTTP 状态码
来源：http://ak.bjjhwx.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ud.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hp.szsharing.cn

JS:   resp.ok;  resp.status
来源：http://lp.colortex.cn

TS:   resp.ok;  resp.status
来源：http://mq.szxytkj.cn

Java: resp.statusCode()
来源：http://ua.bjjhwx.cn

Go:   resp.StatusCode
来源：http://ce.gzmigu.cn

Ruby: resp.code.to_i
来源：http://qs.jianghongdianzi.cn

C#:   (int)resp.StatusCode
来源：http://qu.gzmigu.cn

[L08] 并发请求多个地址
来源：http://vn.huixinmuqiang.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://et.haigaiapp.cn

PHP:  curl_multi_init() 系列
来源：http://qv.nicolike.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qo.newstarts.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://an.huixiangedu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ck.jctech888.com.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ku.bjjhwx.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vx.bjjhwx.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mc.newstarts.cn

================================================================================
来源：http://vx.hahajie.cn

M. 命令行 / 进程 / 环境
来源：http://py.asd995.cn

================================================================================
来源：http://cu.hahajie.cn

[M01] 读取命令行参数
来源：http://ws.wgjwhj.cn

Py:   sys.argv[1:]
来源：http://lb.huixinmuqiang.cn

PHP:  $argv;  $argc;
来源：http://mx.wgjwhj.cn

JS:   process.argv.slice(2)
来源：http://zr.szsharing.cn

TS:   process.argv.slice(2)
来源：http://rv.hnjuh.cn

Java: args 数组（main 方法参数）
来源：http://gm.wgjwhj.cn

Go:   os.Args[1:]
来源：http://cc.521024.cn

Ruby: ARGV
来源：http://vn.lnxyls.cn

C#:   args 数组（Main 方法参数）
来源：http://ih.gzmigu.cn

[M02] 读取环境变量
来源：http://lc.bookmarksfly.cn

Py:   os.environ.get("HOME")
来源：http://cd.nszjky.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lw.huixinmuqiang.cn

JS:   process.env.HOME
来源：http://ub.nszjky.cn

TS:   process.env.HOME
来源：http://vu.chemitech.net.cn

Java: System.getenv("HOME")
来源：http://ri.szsharing.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://is.gzmigu.cn

Ruby: ENV["HOME"]
来源：http://sn.chemitech.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xd.bookmarksfly.cn

[M03] 执行外部命令
来源：http://xg.haigaiapp.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ld.yuexingan06.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ox.lnxyls.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://bx.szsharing.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nd.szsharing.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kr.nicolike.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://eb.szsharing.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vc.huanxung.cn

C#:   Process.Start("ls", "-l");
来源：http://ox.yuntaijiaju.cn

[M04] 获取当前工作目录
来源：http://ob.colortex.cn

Py:   os.getcwd()
来源：http://fj.yuexingan06.cn

PHP:  getcwd();
来源：http://qy.bookmarksfly.cn

JS:   process.cwd()
来源：http://kh.lnxyls.cn

TS:   process.cwd()
来源：http://rt.huanxung.cn

Java: Path.of("").toAbsolutePath()
来源：http://an.newstarts.cn

Go:   os.Getwd()
来源：http://vb.szsharing.cn

Ruby: Dir.pwd
来源：http://qa.lnxyls.cn

C#:   Directory.GetCurrentDirectory()
来源：http://va.lnxyls.cn

[M05] 设置退出码
来源：http://pz.hahajie.cn

Py:   sys.exit(1)
来源：http://ln.lnxyls.cn

PHP:  exit(1);
来源：http://sf.jianghongdianzi.cn

JS:   process.exit(1)
来源：http://ax.nszjky.cn

TS:   process.exit(1)
来源：http://wm.lnxyls.cn

Java: System.exit(1)
来源：http://cl.szxytkj.cn

Go:   os.Exit(1)
来源：http://aq.szsharing.cn

Ruby: exit 1
来源：http://ig.newstarts.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ok.yuntaijiaju.cn

[M06] 向标准错误输出
来源：http://lh.jctech888.com.cn

Py:   print("err", file=sys.stderr)
来源：http://fq.yuntaijiaju.cn


<!-- 参考信息 -->