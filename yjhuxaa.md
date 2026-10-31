代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ty.bjjhwx.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mx.chemitech.net.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ze.panjiajie.cn

================================================================================
来源：http://sk.szsharing.cn

J. 日期与时间
来源：http://jx.yuexingan06.cn

================================================================================
来源：http://uh.shxzukj.cn

[J01] 获取当前时间
来源：http://rx.newstarts.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://po.haigaiapp.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zx.yuexingan06.cn

JS:   new Date();  Date.now()
来源：http://kd.huixiangedu.cn

TS:   new Date();  Date.now()
来源：http://xn.nszjky.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://uo.szsharing.cn

Go:   time.Now()
来源：http://bw.nszjky.cn

Ruby: Time.now
来源：http://ou.shxzskj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://so.muxihuayi.cn

[J02] 格式化输出
来源：http://nr.huixiangedu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pp.panjiajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xw.nicolike.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ym.yuexingan06.cn

TS:   d.toISOString()
来源：http://rn.nicolike.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gz.yuntaijiaju.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://au.chemitech.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qe.newstarts.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ls.muxihuayi.cn

[J03] 字符串解析为日期
来源：http://is.hnjuh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ue.huanxung.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ur.shtwfgs.cn

JS:   new Date("2024-01-02")
来源：http://jr.hnjuh.cn

TS:   new Date("2024-01-02")
来源：http://dt.jianghongdianzi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gv.bjjhwx.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://op.huixiangedu.cn

Ruby: Date.parse("2024-01-02")
来源：http://fj.chemitech.net.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dh.panjiajie.cn

[J04] 时间戳与日期互转
来源：http://ig.yuntaijiaju.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fd.huanxung.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ny.newstarts.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vj.asd995.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hw.huixiangedu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pq.nicolike.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uu.hahajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wa.huanxung.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zx.shtwfgs.cn

[J05] 时间加减（加 7 天）
来源：http://vf.nszjky.cn

Py:   now + timedelta(days=7)
来源：http://cr.gzmigu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nj.521024.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bf.panjiajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ze.colortex.cn

Java: LocalDate.now().plusDays(7)
来源：http://pw.huixiangedu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tz.hahajie.cn

Ruby: Time.now + 7 * 86400
来源：http://ao.muxihuayi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://of.szxytkj.cn

[J06] 计算两时间之差
来源：http://hj.asd995.cn

Py:   (end - start).total_seconds()
来源：http://mn.jctech888.com.cn

PHP:  $end->diff($start)->days;
来源：http://qb.bjjhwx.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mg.jianghongdianzi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wo.huanxung.cn

Java: Duration.between(start, end).toSeconds()
来源：http://uo.bjjhwx.cn

Go:   end.Sub(start).Hours()
来源：http://ez.gzmigu.cn

Ruby: end - start                 # 返回秒数
来源：http://wt.huixinmuqiang.cn

C#:   (end - start).TotalSeconds
来源：http://sb.haigaiapp.cn

[J07] 比较两个日期
来源：http://np.shxzskj.cn

Py:   d1 < d2;  d1 == d2
来源：http://jw.colortex.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ui.huanxung.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tz.szsharing.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fx.yuntaijiaju.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zx.hahajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://we.jctech888.com.cn

Ruby: d1 < d2;  d1 == d2
来源：http://rz.huixiangedu.cn

C#:   d1 < d2;  d1 == d2
来源：http://xq.hnjuh.cn

[J08] 提取年月日与星期
来源：http://xo.shtwfgs.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dk.szsharing.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kw.panjiajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wg.lnxyls.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ef.bookmarksfly.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://om.bjjhwx.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mn.bjjhwx.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sm.yuntaijiaju.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pf.colortex.cn

[J09] 时区处理
来源：http://bu.lnxyls.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nk.asd995.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hh.huixinmuqiang.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wr.haigaiapp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ha.lnxyls.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vi.muxihuayi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://om.hnjuh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zc.nszjky.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wu.lnxyls.cn

[J10] 取今天 / 本月第一天
来源：http://jx.shxzukj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xg.szxytkj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sz.colortex.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kd.nszjky.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ul.hahajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ll.lnxyls.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wb.huixinmuqiang.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tk.bookmarksfly.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ow.gzmigu.cn

================================================================================
来源：http://dw.newstarts.cn

K. JSON 与序列化
来源：http://bc.haigaiapp.cn

================================================================================
来源：http://pd.shxzskj.cn

[K01] 对象转 JSON 字符串
来源：http://bv.bookmarksfly.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uz.bookmarksfly.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zy.panjiajie.cn

JS:   JSON.stringify(obj)
来源：http://nb.hnjuh.cn

TS:   JSON.stringify(obj)
来源：http://wi.yuntaijiaju.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jk.nicolike.cn

Go:   json.Marshal(obj)
来源：http://lk.hahajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vt.huanxung.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://af.9csxet.cn

[K02] JSON 字符串转对象
来源：http://oo.hnjuh.cn

Py:   json.loads(s)
来源：http://cz.bookmarksfly.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bj.wgjwhj.cn

JS:   JSON.parse(s)
来源：http://dl.szxytkj.cn

TS:   JSON.parse(s)
来源：http://cs.haigaiapp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://te.jianghongdianzi.cn

Go:   json.Unmarshal(data, &v)
来源：http://br.hnjuh.cn

Ruby: JSON.parse(s)
来源：http://sl.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://af.szsharing.cn

[K03] JSON 美化输出（带缩进）
来源：http://tr.nicolike.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dn.jctech888.com.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zt.9csxet.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://au.huixiangedu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tj.jctech888.com.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dx.wgjwhj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oa.shxzukj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://yw.szxytkj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qw.panjiajie.cn

[K04] 读取 JSON 文件
来源：http://ez.jctech888.com.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bz.jianghongdianzi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ni.521024.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jp.szsharing.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zy.shtwfgs.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uq.panjiajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dj.jctech888.com.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dk.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ii.colortex.cn

[K05] 深拷贝对象
来源：http://us.hahajie.cn

Py:   copy.deepcopy(obj)
来源：http://sz.haigaiapp.cn

PHP:  unserialize(serialize($obj));
来源：http://mr.shxzukj.cn

JS:   structuredClone(obj)
来源：http://yi.lnxyls.cn

TS:   structuredClone(obj)
来源：http://wf.muxihuayi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jv.newstarts.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vt.hahajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lw.shtwfgs.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://uo.9csxet.cn

[K06] 解析 URL 查询串
来源：http://cm.haigaiapp.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fo.szxytkj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xl.gzmigu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yk.wgjwhj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ew.wgjwhj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xq.hnjuh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ja.szxytkj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tn.haigaiapp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yz.huanxung.cn

[K07] 进制转换
来源：http://ek.521024.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yb.asd995.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vt.bookmarksfly.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gz.nicolike.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hh.nszjky.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cu.hnjuh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gz.lnxyls.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://um.lnxyls.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yn.muxihuayi.cn

[K08] 二进制序列化（非 JSON）
来源：http://et.chemitech.net.cn

Py:   pickle.dumps(obj)
来源：http://sr.jianghongdianzi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://by.panjiajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://sf.nicolike.cn

TS:   v8.serialize(obj)        // Node
来源：http://gl.jianghongdianzi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zk.shxzskj.cn

Go:   encoding/gob
来源：http://ek.yuexingan06.cn

Ruby: Marshal.dump(obj)
来源：http://rs.nicolike.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ql.shxzskj.cn

================================================================================
来源：http://gu.lnxyls.cn

L. 网络请求
来源：http://xv.szsharing.cn

================================================================================
来源：http://cj.bjjhwx.cn

[L01] 发送 GET 请求
来源：http://pt.nszjky.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uj.yuexingan06.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fp.lnxyls.cn

JS:   await fetch(url)
来源：http://jn.jianghongdianzi.cn

TS:   await fetch(url)
来源：http://lq.bjjhwx.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pl.muxihuayi.cn

Go:   resp, err := http.Get(url)
来源：http://dt.yuntaijiaju.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://tv.huixiangedu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fc.bookmarksfly.cn

[L02] 发送 POST JSON
来源：http://wy.hahajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ly.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fq.gzmigu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://km.gzmigu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ai.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vk.9csxet.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xn.huixiangedu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://md.huanxung.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ac.huixiangedu.cn

[L03] 设置自定义请求头
来源：http://tp.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ts.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rj.jianghongdianzi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vg.bookmarksfly.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dq.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bl.szsharing.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nk.huanxung.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qv.jianghongdianzi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zt.shtwfgs.cn

[L04] 设置超时
来源：http://qa.hahajie.cn

Py:   requests.get(url, timeout=5)
来源：http://il.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ft.haigaiapp.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zw.shtwfgs.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qp.9csxet.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://eg.huixiangedu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sl.jianghongdianzi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xk.szsharing.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://oc.521024.cn

[L05] 上传文件（multipart）
来源：http://gh.shtwfgs.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dn.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bh.jctech888.com.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ti.muxihuayi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://in.muxihuayi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ec.asd995.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fv.gzmigu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://su.lnxyls.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gr.jianghongdianzi.cn

[L06] 解析响应为 JSON
来源：http://yr.521024.cn

Py:   resp.json()
来源：http://zp.shxzukj.cn

PHP:  json_decode($body, true);
来源：http://ui.huanxung.cn

JS:   await resp.json()
来源：http://cb.hahajie.cn

TS:   await resp.json()
来源：http://bg.colortex.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fn.521024.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ch.shxzskj.cn

Ruby: JSON.parse(resp.body)
来源：http://cw.521024.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xm.haigaiapp.cn

[L07] 处理 HTTP 状态码
来源：http://qw.nszjky.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://aj.huixiangedu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ip.shtwfgs.cn

JS:   resp.ok;  resp.status
来源：http://qz.hahajie.cn

TS:   resp.ok;  resp.status
来源：http://ht.shxzukj.cn

Java: resp.statusCode()
来源：http://fo.jctech888.com.cn

Go:   resp.StatusCode
来源：http://lc.shtwfgs.cn

Ruby: resp.code.to_i
来源：http://rp.muxihuayi.cn

C#:   (int)resp.StatusCode
来源：http://ah.nicolike.cn

[L08] 并发请求多个地址
来源：http://ku.lnxyls.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wj.jctech888.com.cn

PHP:  curl_multi_init() 系列
来源：http://mz.shtwfgs.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ef.haigaiapp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ui.haigaiapp.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ly.shxzukj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bu.bookmarksfly.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ez.asd995.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gu.hahajie.cn

================================================================================
来源：http://sd.huixiangedu.cn

M. 命令行 / 进程 / 环境
来源：http://hm.haigaiapp.cn

================================================================================
来源：http://dg.colortex.cn

[M01] 读取命令行参数
来源：http://ce.wgjwhj.cn

Py:   sys.argv[1:]
来源：http://kn.huanxung.cn

PHP:  $argv;  $argc;
来源：http://kn.shxzskj.cn

JS:   process.argv.slice(2)
来源：http://zl.panjiajie.cn

TS:   process.argv.slice(2)
来源：http://rp.szxytkj.cn

Java: args 数组（main 方法参数）
来源：http://ek.gzmigu.cn

Go:   os.Args[1:]
来源：http://hz.huixiangedu.cn

Ruby: ARGV
来源：http://ck.shxzskj.cn

C#:   args 数组（Main 方法参数）
来源：http://qb.nszjky.cn

[M02] 读取环境变量
来源：http://jl.huixinmuqiang.cn

Py:   os.environ.get("HOME")
来源：http://de.wgjwhj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://li.lnxyls.cn

JS:   process.env.HOME
来源：http://ff.yuntaijiaju.cn

TS:   process.env.HOME
来源：http://cg.nszjky.cn

Java: System.getenv("HOME")
来源：http://ee.hnjuh.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pb.huanxung.cn

Ruby: ENV["HOME"]
来源：http://ap.colortex.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fq.521024.cn

[M03] 执行外部命令
来源：http://jo.bookmarksfly.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kn.muxihuayi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qi.huixinmuqiang.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ne.nszjky.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://bw.wgjwhj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mg.hahajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jg.huixiangedu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://lc.yuntaijiaju.cn

C#:   Process.Start("ls", "-l");
来源：http://yl.lnxyls.cn

[M04] 获取当前工作目录
来源：http://fy.colortex.cn

Py:   os.getcwd()
来源：http://km.gzmigu.cn

PHP:  getcwd();
来源：http://vl.newstarts.cn

JS:   process.cwd()
来源：http://oe.wgjwhj.cn

TS:   process.cwd()
来源：http://lv.shtwfgs.cn

Java: Path.of("").toAbsolutePath()
来源：http://ia.huanxung.cn

Go:   os.Getwd()
来源：http://sg.asd995.cn

Ruby: Dir.pwd
来源：http://hw.bookmarksfly.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ky.newstarts.cn

[M05] 设置退出码
来源：http://eg.hahajie.cn

Py:   sys.exit(1)
来源：http://bw.haigaiapp.cn

PHP:  exit(1);
来源：http://ne.jctech888.com.cn

JS:   process.exit(1)
来源：http://pe.jianghongdianzi.cn

TS:   process.exit(1)
来源：http://ax.nicolike.cn

Java: System.exit(1)
来源：http://cj.gzmigu.cn

Go:   os.Exit(1)
来源：http://pw.lnxyls.cn

Ruby: exit 1
来源：http://wk.shxzskj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wm.bookmarksfly.cn

[M06] 向标准错误输出
来源：http://yi.asd995.cn

Py:   print("err", file=sys.stderr)
来源：http://tl.bookmarksfly.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://so.huanxung.cn

JS:   console.error("err")
来源：http://nh.bookmarksfly.cn

TS:   console.error("err")
来源：http://fr.panjiajie.cn

Java: System.err.println("err")
来源：http://sn.szxytkj.cn


<!-- 参考信息 -->