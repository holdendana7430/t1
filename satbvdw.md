代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dt.9csxet.cn

[I07] 忽略大小写与多行模式
来源：http://bf.shtwfgs.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wr.bjjhwx.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sh.huixinmuqiang.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rx.hnjuh.cn

TS:   /error/gim
来源：http://ev.jctech888.com.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jx.nicolike.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yd.szxytkj.cn

Ruby: s.scan(/error/i)
来源：http://nr.muxihuayi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kv.shxzukj.cn

[I08] 贪婪与非贪婪匹配
来源：http://ka.hnjuh.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xc.nszjky.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vd.nicolike.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qn.chemitech.net.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://io.shxzskj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://rc.hahajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xr.wgjwhj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://au.wgjwhj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sw.huanxung.cn

================================================================================
来源：http://kc.9csxet.cn

J. 日期与时间
来源：http://wp.shxzukj.cn

================================================================================
来源：http://mp.colortex.cn

[J01] 获取当前时间
来源：http://et.hnjuh.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://mo.9csxet.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ei.521024.cn

JS:   new Date();  Date.now()
来源：http://ke.chemitech.net.cn

TS:   new Date();  Date.now()
来源：http://qx.panjiajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jh.newstarts.cn

Go:   time.Now()
来源：http://zn.521024.cn

Ruby: Time.now
来源：http://cc.shxzukj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://al.shtwfgs.cn

[J02] 格式化输出
来源：http://kk.nicolike.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eo.huixinmuqiang.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dp.huixinmuqiang.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ad.jctech888.com.cn

TS:   d.toISOString()
来源：http://qq.newstarts.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pf.shxzukj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bh.521024.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://av.chemitech.net.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cl.hahajie.cn

[J03] 字符串解析为日期
来源：http://nm.jianghongdianzi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://eb.wgjwhj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cf.wgjwhj.cn

JS:   new Date("2024-01-02")
来源：http://ut.lnxyls.cn

TS:   new Date("2024-01-02")
来源：http://bs.asd995.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ql.nszjky.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://un.shtwfgs.cn

Ruby: Date.parse("2024-01-02")
来源：http://cv.521024.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gv.chemitech.net.cn

[J04] 时间戳与日期互转
来源：http://fs.huanxung.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nx.gzmigu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ig.chemitech.net.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cs.szsharing.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xr.yuntaijiaju.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sm.colortex.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cx.gzmigu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bx.newstarts.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ne.huanxung.cn

[J05] 时间加减（加 7 天）
来源：http://la.jianghongdianzi.cn

Py:   now + timedelta(days=7)
来源：http://gv.hahajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zz.newstarts.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://og.nszjky.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kl.muxihuayi.cn

Java: LocalDate.now().plusDays(7)
来源：http://fm.nszjky.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zc.gzmigu.cn

Ruby: Time.now + 7 * 86400
来源：http://ln.muxihuayi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pl.yuexingan06.cn

[J06] 计算两时间之差
来源：http://kt.hnjuh.cn

Py:   (end - start).total_seconds()
来源：http://sm.chemitech.net.cn

PHP:  $end->diff($start)->days;
来源：http://cs.gzmigu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xw.hahajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yq.shtwfgs.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dv.wgjwhj.cn

Go:   end.Sub(start).Hours()
来源：http://ct.521024.cn

Ruby: end - start                 # 返回秒数
来源：http://ze.szxytkj.cn

C#:   (end - start).TotalSeconds
来源：http://fk.szsharing.cn

[J07] 比较两个日期
来源：http://dm.shxzukj.cn

Py:   d1 < d2;  d1 == d2
来源：http://xz.huixiangedu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jl.hahajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ay.nicolike.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jc.bjjhwx.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://db.nicolike.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bn.szsharing.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wo.yuexingan06.cn

C#:   d1 < d2;  d1 == d2
来源：http://tk.hahajie.cn

[J08] 提取年月日与星期
来源：http://ra.bookmarksfly.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vq.panjiajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://st.gzmigu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tj.chemitech.net.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fx.hnjuh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ys.chemitech.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ux.gzmigu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mg.newstarts.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dl.panjiajie.cn

[J09] 时区处理
来源：http://iy.shtwfgs.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sf.colortex.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://aw.muxihuayi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pw.yuexingan06.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://et.colortex.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ha.huanxung.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xz.hahajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zx.newstarts.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://he.newstarts.cn

[J10] 取今天 / 本月第一天
来源：http://ka.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://px.newstarts.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wy.yuexingan06.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pn.hnjuh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dd.muxihuayi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bo.huixiangedu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jx.jctech888.com.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ht.szxytkj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zz.521024.cn

================================================================================
来源：http://lr.jianghongdianzi.cn

K. JSON 与序列化
来源：http://bc.muxihuayi.cn

================================================================================
来源：http://ks.muxihuayi.cn

[K01] 对象转 JSON 字符串
来源：http://ty.muxihuayi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://iq.panjiajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ol.huanxung.cn

JS:   JSON.stringify(obj)
来源：http://ps.bookmarksfly.cn

TS:   JSON.stringify(obj)
来源：http://zx.shxzukj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ju.hahajie.cn

Go:   json.Marshal(obj)
来源：http://hs.haigaiapp.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xn.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fl.jianghongdianzi.cn

[K02] JSON 字符串转对象
来源：http://ea.hahajie.cn

Py:   json.loads(s)
来源：http://wx.muxihuayi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jb.shxzukj.cn

JS:   JSON.parse(s)
来源：http://uh.shxzskj.cn

TS:   JSON.parse(s)
来源：http://zv.huixinmuqiang.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sj.gzmigu.cn

Go:   json.Unmarshal(data, &v)
来源：http://zo.chemitech.net.cn

Ruby: JSON.parse(s)
来源：http://oz.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gp.szsharing.cn

[K03] JSON 美化输出（带缩进）
来源：http://lt.chemitech.net.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bg.9csxet.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rd.yuntaijiaju.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qv.szsharing.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zl.newstarts.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nn.huanxung.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nq.9csxet.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xs.521024.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gr.hnjuh.cn

[K04] 读取 JSON 文件
来源：http://gs.chemitech.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lf.chemitech.net.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qd.huixiangedu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fn.huixinmuqiang.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://to.bjjhwx.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rt.nszjky.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mj.bookmarksfly.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xj.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://me.jianghongdianzi.cn

[K05] 深拷贝对象
来源：http://an.jianghongdianzi.cn

Py:   copy.deepcopy(obj)
来源：http://uo.9csxet.cn

PHP:  unserialize(serialize($obj));
来源：http://vp.gzmigu.cn

JS:   structuredClone(obj)
来源：http://la.shxzskj.cn

TS:   structuredClone(obj)
来源：http://fp.bjjhwx.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zy.bookmarksfly.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://go.hnjuh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wj.chemitech.net.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hf.gzmigu.cn

[K06] 解析 URL 查询串
来源：http://uu.9csxet.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hd.haigaiapp.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lb.bookmarksfly.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cb.szsharing.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jw.9csxet.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://we.panjiajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rt.hnjuh.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qk.bookmarksfly.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nc.bjjhwx.cn

[K07] 进制转换
来源：http://jr.yuexingan06.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yr.bjjhwx.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lt.gzmigu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nq.shtwfgs.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tw.hnjuh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ij.shxzukj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sk.hnjuh.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ry.asd995.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gy.lnxyls.cn

[K08] 二进制序列化（非 JSON）
来源：http://mu.jianghongdianzi.cn

Py:   pickle.dumps(obj)
来源：http://pe.9csxet.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ys.jctech888.com.cn

JS:   v8.serialize(obj)        // Node
来源：http://ip.szsharing.cn

TS:   v8.serialize(obj)        // Node
来源：http://ry.yuntaijiaju.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ro.szsharing.cn

Go:   encoding/gob
来源：http://jo.yuntaijiaju.cn

Ruby: Marshal.dump(obj)
来源：http://ch.yuntaijiaju.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ns.shtwfgs.cn

================================================================================
来源：http://fl.haigaiapp.cn

L. 网络请求
来源：http://qz.shxzukj.cn

================================================================================
来源：http://pn.shxzukj.cn

[L01] 发送 GET 请求
来源：http://ya.521024.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dc.nicolike.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://du.gzmigu.cn

JS:   await fetch(url)
来源：http://jq.jianghongdianzi.cn

TS:   await fetch(url)
来源：http://mg.asd995.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mr.huanxung.cn

Go:   resp, err := http.Get(url)
来源：http://ww.newstarts.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ec.huixinmuqiang.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lx.haigaiapp.cn

[L02] 发送 POST JSON
来源：http://mo.huixiangedu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://jf.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hk.yuntaijiaju.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cl.yuntaijiaju.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xj.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sx.huixinmuqiang.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xf.panjiajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://oh.huixiangedu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://at.lnxyls.cn

[L03] 设置自定义请求头
来源：http://nw.bjjhwx.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yu.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qd.521024.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hk.szxytkj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ni.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lx.hnjuh.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://st.newstarts.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ds.9csxet.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gc.jianghongdianzi.cn

[L04] 设置超时
来源：http://sa.jianghongdianzi.cn

Py:   requests.get(url, timeout=5)
来源：http://ha.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xd.haigaiapp.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hq.newstarts.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yd.szxytkj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pr.huixiangedu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tx.nszjky.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ld.shtwfgs.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qo.shxzskj.cn

[L05] 上传文件（multipart）
来源：http://mb.hahajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ia.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ag.shtwfgs.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://am.huanxung.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fl.newstarts.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ha.yuntaijiaju.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://om.huanxung.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fz.shxzukj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nm.yuntaijiaju.cn

[L06] 解析响应为 JSON
来源：http://pj.panjiajie.cn

Py:   resp.json()
来源：http://vh.bookmarksfly.cn

PHP:  json_decode($body, true);
来源：http://db.521024.cn

JS:   await resp.json()
来源：http://kg.yuexingan06.cn

TS:   await resp.json()
来源：http://xk.colortex.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ds.wgjwhj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qe.521024.cn

Ruby: JSON.parse(resp.body)
来源：http://sv.panjiajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mx.szsharing.cn

[L07] 处理 HTTP 状态码
来源：http://wf.panjiajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cw.jctech888.com.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kx.9csxet.cn

JS:   resp.ok;  resp.status
来源：http://ac.jianghongdianzi.cn

TS:   resp.ok;  resp.status
来源：http://jy.yuexingan06.cn

Java: resp.statusCode()
来源：http://en.szxytkj.cn

Go:   resp.StatusCode
来源：http://un.muxihuayi.cn

Ruby: resp.code.to_i
来源：http://sk.jctech888.com.cn

C#:   (int)resp.StatusCode
来源：http://xe.yuntaijiaju.cn

[L08] 并发请求多个地址
来源：http://or.newstarts.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rb.9csxet.cn

PHP:  curl_multi_init() 系列
来源：http://kh.newstarts.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bq.wgjwhj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kl.panjiajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://af.haigaiapp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bf.huixinmuqiang.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://aw.nicolike.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ev.shtwfgs.cn

================================================================================
来源：http://hz.panjiajie.cn

M. 命令行 / 进程 / 环境
来源：http://qj.colortex.cn

================================================================================
来源：http://yt.szxytkj.cn

[M01] 读取命令行参数
来源：http://pl.huixinmuqiang.cn

Py:   sys.argv[1:]
来源：http://yc.yuntaijiaju.cn

PHP:  $argv;  $argc;
来源：http://hy.huixiangedu.cn

JS:   process.argv.slice(2)
来源：http://rl.yuntaijiaju.cn

TS:   process.argv.slice(2)
来源：http://bz.bookmarksfly.cn

Java: args 数组（main 方法参数）
来源：http://rr.szsharing.cn

Go:   os.Args[1:]
来源：http://iv.yuntaijiaju.cn

Ruby: ARGV
来源：http://id.jctech888.com.cn

C#:   args 数组（Main 方法参数）
来源：http://xy.nszjky.cn

[M02] 读取环境变量
来源：http://cq.nicolike.cn

Py:   os.environ.get("HOME")
来源：http://nk.szxytkj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jt.jctech888.com.cn

JS:   process.env.HOME
来源：http://yq.nszjky.cn

TS:   process.env.HOME
来源：http://ke.colortex.cn

Java: System.getenv("HOME")
来源：http://el.bjjhwx.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sj.chemitech.net.cn

Ruby: ENV["HOME"]
来源：http://sa.shxzskj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pg.asd995.cn

[M03] 执行外部命令
来源：http://cl.gzmigu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cp.szsharing.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://um.jctech888.com.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ra.newstarts.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vm.newstarts.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hg.nszjky.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ml.szsharing.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ku.jianghongdianzi.cn

C#:   Process.Start("ls", "-l");
来源：http://mh.huixiangedu.cn

[M04] 获取当前工作目录
来源：http://ue.hnjuh.cn

Py:   os.getcwd()
来源：http://mv.lnxyls.cn

PHP:  getcwd();
来源：http://qc.szsharing.cn

JS:   process.cwd()
来源：http://dx.gzmigu.cn

TS:   process.cwd()
来源：http://fk.jctech888.com.cn

Java: Path.of("").toAbsolutePath()
来源：http://sg.bjjhwx.cn

Go:   os.Getwd()
来源：http://kf.yuntaijiaju.cn

Ruby: Dir.pwd
来源：http://ib.nszjky.cn


<!-- 参考信息 -->