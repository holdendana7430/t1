代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zy.shtwfgs.cn

TS:   /error/gim
来源：http://xh.nszjky.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://di.bookmarksfly.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rr.wgjwhj.cn

Ruby: s.scan(/error/i)
来源：http://ly.gzmigu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ki.wgjwhj.cn

[I08] 贪婪与非贪婪匹配
来源：http://jv.panjiajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pf.szxytkj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jw.wgjwhj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fw.nicolike.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kp.nicolike.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lg.huixiangedu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ji.jctech888.com.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pm.bookmarksfly.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ub.newstarts.cn

================================================================================
来源：http://nl.chemitech.net.cn

J. 日期与时间
来源：http://ws.9csxet.cn

================================================================================
来源：http://kx.szsharing.cn

[J01] 获取当前时间
来源：http://xd.shxzskj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ez.panjiajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bq.huixinmuqiang.cn

JS:   new Date();  Date.now()
来源：http://gc.lnxyls.cn

TS:   new Date();  Date.now()
来源：http://cn.huixiangedu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lo.huixinmuqiang.cn

Go:   time.Now()
来源：http://kb.hahajie.cn

Ruby: Time.now
来源：http://ir.colortex.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jx.jianghongdianzi.cn

[J02] 格式化输出
来源：http://ls.lnxyls.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ed.lnxyls.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nf.szsharing.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wf.hahajie.cn

TS:   d.toISOString()
来源：http://lg.jctech888.com.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://iu.lnxyls.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qk.muxihuayi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dh.gzmigu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yp.bookmarksfly.cn

[J03] 字符串解析为日期
来源：http://vo.bjjhwx.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qa.colortex.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ba.huixinmuqiang.cn

JS:   new Date("2024-01-02")
来源：http://tp.hahajie.cn

TS:   new Date("2024-01-02")
来源：http://mj.nicolike.cn

Java: LocalDate.parse("2024-01-02")
来源：http://uq.jctech888.com.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fe.newstarts.cn

Ruby: Date.parse("2024-01-02")
来源：http://oc.panjiajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cd.huixinmuqiang.cn

[J04] 时间戳与日期互转
来源：http://oe.yuntaijiaju.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uk.haigaiapp.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fo.shxzukj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sc.gzmigu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fb.wgjwhj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://up.huixiangedu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://je.bjjhwx.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://du.shtwfgs.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cf.nicolike.cn

[J05] 时间加减（加 7 天）
来源：http://td.shtwfgs.cn

Py:   now + timedelta(days=7)
来源：http://dv.nszjky.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qe.szsharing.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jt.newstarts.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ej.newstarts.cn

Java: LocalDate.now().plusDays(7)
来源：http://jj.yuntaijiaju.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tr.wgjwhj.cn

Ruby: Time.now + 7 * 86400
来源：http://rh.shxzskj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://cd.bjjhwx.cn

[J06] 计算两时间之差
来源：http://sy.newstarts.cn

Py:   (end - start).total_seconds()
来源：http://gm.yuntaijiaju.cn

PHP:  $end->diff($start)->days;
来源：http://zi.gzmigu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pi.bjjhwx.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dp.jctech888.com.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jy.haigaiapp.cn

Go:   end.Sub(start).Hours()
来源：http://js.nszjky.cn

Ruby: end - start                 # 返回秒数
来源：http://ec.9csxet.cn

C#:   (end - start).TotalSeconds
来源：http://cx.nszjky.cn

[J07] 比较两个日期
来源：http://ap.shtwfgs.cn

Py:   d1 < d2;  d1 == d2
来源：http://mv.shxzukj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vq.bookmarksfly.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wj.colortex.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ft.szsharing.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://eb.szsharing.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sw.yuexingan06.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fi.huixiangedu.cn

C#:   d1 < d2;  d1 == d2
来源：http://rc.lnxyls.cn

[J08] 提取年月日与星期
来源：http://gp.nicolike.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wi.gzmigu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hp.newstarts.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qy.hahajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kb.huanxung.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ry.shxzskj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pc.9csxet.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://se.asd995.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ho.colortex.cn

[J09] 时区处理
来源：http://de.521024.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ff.shxzukj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://us.shxzskj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nn.chemitech.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ro.huanxung.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hl.asd995.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ef.hahajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zw.newstarts.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ql.huixiangedu.cn

[J10] 取今天 / 本月第一天
来源：http://wx.huixinmuqiang.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://mq.newstarts.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rq.nicolike.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cl.nszjky.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vv.szxytkj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fw.chemitech.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qz.panjiajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lu.nicolike.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tf.szsharing.cn

================================================================================
来源：http://fp.szxytkj.cn

K. JSON 与序列化
来源：http://vj.huanxung.cn

================================================================================
来源：http://vo.jctech888.com.cn

[K01] 对象转 JSON 字符串
来源：http://kq.shtwfgs.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gv.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wl.shtwfgs.cn

JS:   JSON.stringify(obj)
来源：http://es.shxzukj.cn

TS:   JSON.stringify(obj)
来源：http://bs.521024.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://br.gzmigu.cn

Go:   json.Marshal(obj)
来源：http://zp.bjjhwx.cn

Ruby: obj.to_json                                     // require "json"
来源：http://lq.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bh.yuntaijiaju.cn

[K02] JSON 字符串转对象
来源：http://er.muxihuayi.cn

Py:   json.loads(s)
来源：http://qr.huixiangedu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ah.yuexingan06.cn

JS:   JSON.parse(s)
来源：http://mu.panjiajie.cn

TS:   JSON.parse(s)
来源：http://ae.haigaiapp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zm.jianghongdianzi.cn

Go:   json.Unmarshal(data, &v)
来源：http://qt.9csxet.cn

Ruby: JSON.parse(s)
来源：http://uy.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ak.hnjuh.cn

[K03] JSON 美化输出（带缩进）
来源：http://tf.yuntaijiaju.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jv.9csxet.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nx.521024.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rl.lnxyls.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ay.wgjwhj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ag.muxihuayi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zu.huanxung.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zb.panjiajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yi.jctech888.com.cn

[K04] 读取 JSON 文件
来源：http://ox.huixinmuqiang.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ku.huixiangedu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nl.haigaiapp.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oo.hahajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zq.chemitech.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zu.shxzskj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ru.huixiangedu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gt.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rk.huanxung.cn

[K05] 深拷贝对象
来源：http://vq.bookmarksfly.cn

Py:   copy.deepcopy(obj)
来源：http://lf.huixiangedu.cn

PHP:  unserialize(serialize($obj));
来源：http://vu.szxytkj.cn

JS:   structuredClone(obj)
来源：http://ec.chemitech.net.cn

TS:   structuredClone(obj)
来源：http://la.wgjwhj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dj.asd995.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fp.huixiangedu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jl.bookmarksfly.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qu.shxzukj.cn

[K06] 解析 URL 查询串
来源：http://fw.shtwfgs.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vp.newstarts.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ci.huanxung.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gz.shtwfgs.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lz.jianghongdianzi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lx.jianghongdianzi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zg.szsharing.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oc.szsharing.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lk.9csxet.cn

[K07] 进制转换
来源：http://ts.haigaiapp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ah.szxytkj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bx.bookmarksfly.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ge.wgjwhj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://us.lnxyls.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ta.szxytkj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qa.newstarts.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nt.szsharing.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nq.huanxung.cn

[K08] 二进制序列化（非 JSON）
来源：http://bn.szxytkj.cn

Py:   pickle.dumps(obj)
来源：http://rg.hahajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://jm.jianghongdianzi.cn

JS:   v8.serialize(obj)        // Node
来源：http://dh.szxytkj.cn

TS:   v8.serialize(obj)        // Node
来源：http://fs.wgjwhj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jz.9csxet.cn

Go:   encoding/gob
来源：http://ku.gzmigu.cn

Ruby: Marshal.dump(obj)
来源：http://yq.huixiangedu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ao.newstarts.cn

================================================================================
来源：http://td.nszjky.cn

L. 网络请求
来源：http://fz.nicolike.cn

================================================================================
来源：http://st.chemitech.net.cn

[L01] 发送 GET 请求
来源：http://zc.bjjhwx.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ei.521024.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pu.nicolike.cn

JS:   await fetch(url)
来源：http://oi.newstarts.cn

TS:   await fetch(url)
来源：http://dm.bjjhwx.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rz.521024.cn

Go:   resp, err := http.Get(url)
来源：http://ag.jianghongdianzi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zq.bookmarksfly.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xe.bjjhwx.cn

[L02] 发送 POST JSON
来源：http://pd.gzmigu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://uj.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cv.asd995.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uf.huixinmuqiang.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ku.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ms.521024.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dq.hnjuh.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nj.szxytkj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sh.panjiajie.cn

[L03] 设置自定义请求头
来源：http://vb.asd995.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tj.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yj.jianghongdianzi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zp.asd995.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://os.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rc.haigaiapp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ys.gzmigu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://en.gzmigu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rf.jianghongdianzi.cn

[L04] 设置超时
来源：http://qf.nicolike.cn

Py:   requests.get(url, timeout=5)
来源：http://pj.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tm.shxzukj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://du.shxzukj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ih.huixiangedu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://oh.newstarts.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dv.shtwfgs.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bs.chemitech.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gp.chemitech.net.cn

[L05] 上传文件（multipart）
来源：http://qr.muxihuayi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fw.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hx.nszjky.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cj.panjiajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gv.newstarts.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://of.lnxyls.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ct.huanxung.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bi.nicolike.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jm.shxzukj.cn

[L06] 解析响应为 JSON
来源：http://ft.huixinmuqiang.cn

Py:   resp.json()
来源：http://xm.bookmarksfly.cn

PHP:  json_decode($body, true);
来源：http://wz.jctech888.com.cn

JS:   await resp.json()
来源：http://ou.9csxet.cn

TS:   await resp.json()
来源：http://cu.colortex.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uh.yuntaijiaju.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://sd.huixinmuqiang.cn

Ruby: JSON.parse(resp.body)
来源：http://yp.hnjuh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fg.asd995.cn

[L07] 处理 HTTP 状态码
来源：http://pe.colortex.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wa.huixinmuqiang.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bt.jianghongdianzi.cn

JS:   resp.ok;  resp.status
来源：http://id.newstarts.cn

TS:   resp.ok;  resp.status
来源：http://hy.hahajie.cn

Java: resp.statusCode()
来源：http://ap.haigaiapp.cn

Go:   resp.StatusCode
来源：http://yf.bookmarksfly.cn

Ruby: resp.code.to_i
来源：http://ro.newstarts.cn

C#:   (int)resp.StatusCode
来源：http://aq.nszjky.cn

[L08] 并发请求多个地址
来源：http://xm.nicolike.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ng.huanxung.cn

PHP:  curl_multi_init() 系列
来源：http://yc.yuntaijiaju.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rw.yuexingan06.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jz.gzmigu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nn.huanxung.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cu.hahajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://an.gzmigu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pl.panjiajie.cn

================================================================================
来源：http://ls.muxihuayi.cn

M. 命令行 / 进程 / 环境
来源：http://dy.nszjky.cn

================================================================================
来源：http://xa.szsharing.cn

[M01] 读取命令行参数
来源：http://ge.shxzskj.cn

Py:   sys.argv[1:]
来源：http://dy.hnjuh.cn

PHP:  $argv;  $argc;
来源：http://uk.asd995.cn

JS:   process.argv.slice(2)
来源：http://uk.nszjky.cn

TS:   process.argv.slice(2)
来源：http://dq.9csxet.cn

Java: args 数组（main 方法参数）
来源：http://ja.521024.cn

Go:   os.Args[1:]
来源：http://zq.huanxung.cn

Ruby: ARGV
来源：http://zb.jctech888.com.cn

C#:   args 数组（Main 方法参数）
来源：http://mt.yuexingan06.cn

[M02] 读取环境变量
来源：http://pw.asd995.cn

Py:   os.environ.get("HOME")
来源：http://hx.jianghongdianzi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://st.asd995.cn

JS:   process.env.HOME
来源：http://rb.yuntaijiaju.cn

TS:   process.env.HOME
来源：http://mb.newstarts.cn

Java: System.getenv("HOME")
来源：http://ca.521024.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dz.jctech888.com.cn

Ruby: ENV["HOME"]
来源：http://vz.lnxyls.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ig.bjjhwx.cn

[M03] 执行外部命令
来源：http://rh.newstarts.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qh.yuexingan06.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ho.nszjky.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ou.huixiangedu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qu.wgjwhj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zs.muxihuayi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lc.asd995.cn

Ruby: system("ls -l");  `ls -l`
来源：http://lc.newstarts.cn

C#:   Process.Start("ls", "-l");
来源：http://na.wgjwhj.cn

[M04] 获取当前工作目录
来源：http://my.huixiangedu.cn

Py:   os.getcwd()
来源：http://lk.jctech888.com.cn

PHP:  getcwd();
来源：http://pp.jctech888.com.cn

JS:   process.cwd()
来源：http://dd.huixiangedu.cn

TS:   process.cwd()
来源：http://jz.yuntaijiaju.cn

Java: Path.of("").toAbsolutePath()
来源：http://gh.jianghongdianzi.cn

Go:   os.Getwd()
来源：http://th.shxzskj.cn

Ruby: Dir.pwd
来源：http://hk.huixiangedu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://iu.haigaiapp.cn

[M05] 设置退出码
来源：http://yn.newstarts.cn

Py:   sys.exit(1)
来源：http://ju.521024.cn

PHP:  exit(1);
来源：http://kz.panjiajie.cn


<!-- 参考信息 -->