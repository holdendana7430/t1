代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yn.wgjwhj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xp.jianghongdianzi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ts.muxihuayi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nm.shtwfgs.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fv.gzmigu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ej.yuexingan06.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bt.huanxung.cn

================================================================================
来源：http://qe.szxytkj.cn

J. 日期与时间
来源：http://ay.huanxung.cn

================================================================================
来源：http://vm.gzmigu.cn

[J01] 获取当前时间
来源：http://mo.hnjuh.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rq.asd995.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wn.huixinmuqiang.cn

JS:   new Date();  Date.now()
来源：http://jt.colortex.cn

TS:   new Date();  Date.now()
来源：http://so.szxytkj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://gg.asd995.cn

Go:   time.Now()
来源：http://pn.yuntaijiaju.cn

Ruby: Time.now
来源：http://os.jctech888.com.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bb.521024.cn

[J02] 格式化输出
来源：http://da.newstarts.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sy.huixiangedu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bu.newstarts.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lj.521024.cn

TS:   d.toISOString()
来源：http://ee.lnxyls.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cz.colortex.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nm.jianghongdianzi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mu.panjiajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ub.shtwfgs.cn

[J03] 字符串解析为日期
来源：http://ct.shtwfgs.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ru.muxihuayi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kk.nicolike.cn

JS:   new Date("2024-01-02")
来源：http://zf.newstarts.cn

TS:   new Date("2024-01-02")
来源：http://pk.haigaiapp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://yr.huixiangedu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hx.shtwfgs.cn

Ruby: Date.parse("2024-01-02")
来源：http://gf.hahajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ag.hahajie.cn

[J04] 时间戳与日期互转
来源：http://ry.yuexingan06.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ut.chemitech.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pj.jianghongdianzi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rh.jianghongdianzi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tu.szxytkj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vc.colortex.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ls.haigaiapp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ww.wgjwhj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cg.muxihuayi.cn

[J05] 时间加减（加 7 天）
来源：http://xl.szxytkj.cn

Py:   now + timedelta(days=7)
来源：http://wo.huixiangedu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://fm.hnjuh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tr.muxihuayi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rp.jianghongdianzi.cn

Java: LocalDate.now().plusDays(7)
来源：http://hg.szxytkj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uy.szsharing.cn

Ruby: Time.now + 7 * 86400
来源：http://xz.521024.cn

C#:   DateTime.Now.AddDays(7)
来源：http://en.521024.cn

[J06] 计算两时间之差
来源：http://ag.521024.cn

Py:   (end - start).total_seconds()
来源：http://et.bjjhwx.cn

PHP:  $end->diff($start)->days;
来源：http://jd.szsharing.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sl.muxihuayi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zy.shxzukj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://sm.huanxung.cn

Go:   end.Sub(start).Hours()
来源：http://zz.9csxet.cn

Ruby: end - start                 # 返回秒数
来源：http://el.szsharing.cn

C#:   (end - start).TotalSeconds
来源：http://xo.shxzukj.cn

[J07] 比较两个日期
来源：http://kb.nszjky.cn

Py:   d1 < d2;  d1 == d2
来源：http://kl.muxihuayi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://op.haigaiapp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zi.yuexingan06.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jm.shxzukj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ro.shxzukj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://il.521024.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ur.lnxyls.cn

C#:   d1 < d2;  d1 == d2
来源：http://xa.muxihuayi.cn

[J08] 提取年月日与星期
来源：http://zh.chemitech.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jw.yuntaijiaju.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yz.muxihuayi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qv.hahajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wd.yuntaijiaju.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ea.wgjwhj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://up.newstarts.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dy.hnjuh.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wk.jctech888.com.cn

[J09] 时区处理
来源：http://rp.jianghongdianzi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gj.hahajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://iu.yuexingan06.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ia.shtwfgs.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rj.szsharing.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bn.bjjhwx.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hr.bjjhwx.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cm.hahajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mc.wgjwhj.cn

[J10] 取今天 / 本月第一天
来源：http://ia.bookmarksfly.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ov.hnjuh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ag.lnxyls.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bs.521024.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qz.yuexingan06.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dk.lnxyls.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://du.hnjuh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://eo.hnjuh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zi.gzmigu.cn

================================================================================
来源：http://nv.chemitech.net.cn

K. JSON 与序列化
来源：http://il.chemitech.net.cn

================================================================================
来源：http://jx.jctech888.com.cn

[K01] 对象转 JSON 字符串
来源：http://by.asd995.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vw.wgjwhj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bl.asd995.cn

JS:   JSON.stringify(obj)
来源：http://rr.panjiajie.cn

TS:   JSON.stringify(obj)
来源：http://nz.newstarts.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://oz.huixinmuqiang.cn

Go:   json.Marshal(obj)
来源：http://qr.wgjwhj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://lg.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://so.haigaiapp.cn

[K02] JSON 字符串转对象
来源：http://xr.jctech888.com.cn

Py:   json.loads(s)
来源：http://wo.haigaiapp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ml.shxzukj.cn

JS:   JSON.parse(s)
来源：http://fm.haigaiapp.cn

TS:   JSON.parse(s)
来源：http://uj.panjiajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qb.huixinmuqiang.cn

Go:   json.Unmarshal(data, &v)
来源：http://wd.hnjuh.cn

Ruby: JSON.parse(s)
来源：http://ax.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://oz.shtwfgs.cn

[K03] JSON 美化输出（带缩进）
来源：http://pd.colortex.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cy.gzmigu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rd.chemitech.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wb.nicolike.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sh.huanxung.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gb.huixiangedu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://up.yuntaijiaju.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vq.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gy.szxytkj.cn

[K04] 读取 JSON 文件
来源：http://za.panjiajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ck.huanxung.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wk.nszjky.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yi.chemitech.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nu.shxzskj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vm.nszjky.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tc.huixiangedu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://kz.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gr.chemitech.net.cn

[K05] 深拷贝对象
来源：http://xs.nszjky.cn

Py:   copy.deepcopy(obj)
来源：http://ni.haigaiapp.cn

PHP:  unserialize(serialize($obj));
来源：http://lj.szsharing.cn

JS:   structuredClone(obj)
来源：http://mb.jctech888.com.cn

TS:   structuredClone(obj)
来源：http://fa.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ch.nicolike.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bg.lnxyls.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xp.asd995.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tb.huanxung.cn

[K06] 解析 URL 查询串
来源：http://dl.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lq.bjjhwx.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pw.lnxyls.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://km.wgjwhj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://my.jctech888.com.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ic.shxzukj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ag.panjiajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cn.shtwfgs.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ug.panjiajie.cn

[K07] 进制转换
来源：http://fh.bjjhwx.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://db.shxzskj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ni.shxzskj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pl.shxzukj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kj.jctech888.com.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bo.huixiangedu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kd.wgjwhj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wz.gzmigu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pe.gzmigu.cn

[K08] 二进制序列化（非 JSON）
来源：http://pv.chemitech.net.cn

Py:   pickle.dumps(obj)
来源：http://nn.bookmarksfly.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ii.shxzskj.cn

JS:   v8.serialize(obj)        // Node
来源：http://hq.hahajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://kl.huanxung.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wd.9csxet.cn

Go:   encoding/gob
来源：http://hx.nszjky.cn

Ruby: Marshal.dump(obj)
来源：http://le.nicolike.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zg.yuexingan06.cn

================================================================================
来源：http://gc.jianghongdianzi.cn

L. 网络请求
来源：http://pk.szsharing.cn

================================================================================
来源：http://qu.nicolike.cn

[L01] 发送 GET 请求
来源：http://ph.jctech888.com.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xx.521024.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zx.colortex.cn

JS:   await fetch(url)
来源：http://qm.yuexingan06.cn

TS:   await fetch(url)
来源：http://ey.huixiangedu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lk.9csxet.cn

Go:   resp, err := http.Get(url)
来源：http://ny.lnxyls.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bx.yuexingan06.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vl.jctech888.com.cn

[L02] 发送 POST JSON
来源：http://ud.shtwfgs.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cl.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ti.huanxung.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nt.haigaiapp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://az.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xg.huixinmuqiang.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cy.shxzskj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://of.hahajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sj.huanxung.cn

[L03] 设置自定义请求头
来源：http://vv.shxzukj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ui.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nv.muxihuayi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://db.yuntaijiaju.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yn.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ao.panjiajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://iq.hahajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://of.newstarts.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dr.hnjuh.cn

[L04] 设置超时
来源：http://vo.yuexingan06.cn

Py:   requests.get(url, timeout=5)
来源：http://jo.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://oz.shxzskj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ls.shxzukj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fh.wgjwhj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pd.muxihuayi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ca.panjiajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://va.haigaiapp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://so.jianghongdianzi.cn

[L05] 上传文件（multipart）
来源：http://yk.colortex.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ei.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rc.nicolike.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gm.szsharing.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uz.shtwfgs.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ms.shxzskj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://za.bookmarksfly.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://av.huixinmuqiang.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xs.shxzukj.cn

[L06] 解析响应为 JSON
来源：http://cf.lnxyls.cn

Py:   resp.json()
来源：http://wj.9csxet.cn

PHP:  json_decode($body, true);
来源：http://yq.nicolike.cn

JS:   await resp.json()
来源：http://vn.nszjky.cn

TS:   await resp.json()
来源：http://rf.shxzskj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nb.hahajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ux.newstarts.cn

Ruby: JSON.parse(resp.body)
来源：http://ov.nszjky.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://st.szsharing.cn

[L07] 处理 HTTP 状态码
来源：http://qp.asd995.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://no.yuntaijiaju.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ok.nszjky.cn

JS:   resp.ok;  resp.status
来源：http://rg.lnxyls.cn

TS:   resp.ok;  resp.status
来源：http://kj.chemitech.net.cn

Java: resp.statusCode()
来源：http://nu.bjjhwx.cn

Go:   resp.StatusCode
来源：http://ff.shxzukj.cn

Ruby: resp.code.to_i
来源：http://yk.yuntaijiaju.cn

C#:   (int)resp.StatusCode
来源：http://sc.yuexingan06.cn

[L08] 并发请求多个地址
来源：http://fe.haigaiapp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hr.lnxyls.cn

PHP:  curl_multi_init() 系列
来源：http://ub.9csxet.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wz.lnxyls.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sr.nszjky.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xs.jctech888.com.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xq.huixiangedu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://or.jianghongdianzi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://me.hnjuh.cn

================================================================================
来源：http://nx.nszjky.cn

M. 命令行 / 进程 / 环境
来源：http://cr.hahajie.cn

================================================================================
来源：http://xa.wgjwhj.cn

[M01] 读取命令行参数
来源：http://vh.521024.cn

Py:   sys.argv[1:]
来源：http://vf.yuntaijiaju.cn

PHP:  $argv;  $argc;
来源：http://rm.lnxyls.cn

JS:   process.argv.slice(2)
来源：http://wl.shxzskj.cn

TS:   process.argv.slice(2)
来源：http://re.hnjuh.cn

Java: args 数组（main 方法参数）
来源：http://dh.colortex.cn

Go:   os.Args[1:]
来源：http://tn.colortex.cn

Ruby: ARGV
来源：http://qy.shxzukj.cn

C#:   args 数组（Main 方法参数）
来源：http://nz.wgjwhj.cn

[M02] 读取环境变量
来源：http://oq.bjjhwx.cn

Py:   os.environ.get("HOME")
来源：http://vs.yuntaijiaju.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://io.yuntaijiaju.cn

JS:   process.env.HOME
来源：http://vz.9csxet.cn

TS:   process.env.HOME
来源：http://at.huanxung.cn

Java: System.getenv("HOME")
来源：http://wx.shtwfgs.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fe.asd995.cn

Ruby: ENV["HOME"]
来源：http://wf.wgjwhj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kw.gzmigu.cn

[M03] 执行外部命令
来源：http://ed.huixiangedu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gj.jctech888.com.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vs.panjiajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://cd.shxzukj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vx.nszjky.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zx.nszjky.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zh.nszjky.cn

Ruby: system("ls -l");  `ls -l`
来源：http://my.huanxung.cn

C#:   Process.Start("ls", "-l");
来源：http://th.szxytkj.cn

[M04] 获取当前工作目录
来源：http://ip.hnjuh.cn

Py:   os.getcwd()
来源：http://jo.jianghongdianzi.cn

PHP:  getcwd();
来源：http://vd.hnjuh.cn

JS:   process.cwd()
来源：http://fi.panjiajie.cn

TS:   process.cwd()
来源：http://pl.jctech888.com.cn

Java: Path.of("").toAbsolutePath()
来源：http://ay.gzmigu.cn

Go:   os.Getwd()
来源：http://qt.szsharing.cn

Ruby: Dir.pwd
来源：http://vm.haigaiapp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yr.shxzskj.cn

[M05] 设置退出码
来源：http://gl.yuexingan06.cn

Py:   sys.exit(1)
来源：http://pm.szxytkj.cn

PHP:  exit(1);
来源：http://fa.hahajie.cn

JS:   process.exit(1)
来源：http://oi.shxzskj.cn

TS:   process.exit(1)
来源：http://pa.yuntaijiaju.cn

Java: System.exit(1)
来源：http://nx.nicolike.cn

Go:   os.Exit(1)
来源：http://zr.yuexingan06.cn

Ruby: exit 1
来源：http://mg.chemitech.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hq.shtwfgs.cn

[M06] 向标准错误输出
来源：http://hn.jianghongdianzi.cn

Py:   print("err", file=sys.stderr)
来源：http://tw.yuexingan06.cn


<!-- 参考信息 -->