代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://at.bjjhwx.cn

[I07] 忽略大小写与多行模式
来源：http://ux.szxytkj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cc.yuexingan06.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hj.wgjwhj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xq.yuexingan06.cn

TS:   /error/gim
来源：http://yb.shxzukj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pn.newstarts.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ff.jctech888.com.cn

Ruby: s.scan(/error/i)
来源：http://ti.newstarts.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bw.hnjuh.cn

[I08] 贪婪与非贪婪匹配
来源：http://fo.shxzskj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lp.asd995.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yb.jianghongdianzi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fo.newstarts.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jn.hnjuh.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fr.lnxyls.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ef.jianghongdianzi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://po.nszjky.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nv.huanxung.cn

================================================================================
来源：http://xw.panjiajie.cn

J. 日期与时间
来源：http://pp.521024.cn

================================================================================
来源：http://ao.hnjuh.cn

[J01] 获取当前时间
来源：http://oh.asd995.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qf.panjiajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wt.gzmigu.cn

JS:   new Date();  Date.now()
来源：http://za.nszjky.cn

TS:   new Date();  Date.now()
来源：http://vf.asd995.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://oh.hahajie.cn

Go:   time.Now()
来源：http://tw.asd995.cn

Ruby: Time.now
来源：http://vs.newstarts.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hs.huixinmuqiang.cn

[J02] 格式化输出
来源：http://kn.huixiangedu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ep.shxzskj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rg.asd995.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yx.jctech888.com.cn

TS:   d.toISOString()
来源：http://ri.shtwfgs.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://si.szxytkj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://js.chemitech.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://at.newstarts.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vo.jianghongdianzi.cn

[J03] 字符串解析为日期
来源：http://ez.huixinmuqiang.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://aa.huixiangedu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nj.lnxyls.cn

JS:   new Date("2024-01-02")
来源：http://ds.wgjwhj.cn

TS:   new Date("2024-01-02")
来源：http://vb.jctech888.com.cn

Java: LocalDate.parse("2024-01-02")
来源：http://kq.gzmigu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hb.shtwfgs.cn

Ruby: Date.parse("2024-01-02")
来源：http://be.panjiajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kq.wgjwhj.cn

[J04] 时间戳与日期互转
来源：http://en.newstarts.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wr.9csxet.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wr.shxzskj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wy.huixiangedu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zv.lnxyls.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ur.panjiajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://px.panjiajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ya.newstarts.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lp.chemitech.net.cn

[J05] 时间加减（加 7 天）
来源：http://xr.521024.cn

Py:   now + timedelta(days=7)
来源：http://js.muxihuayi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lw.hnjuh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lb.lnxyls.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zv.bjjhwx.cn

Java: LocalDate.now().plusDays(7)
来源：http://vm.hnjuh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://to.huixiangedu.cn

Ruby: Time.now + 7 * 86400
来源：http://bn.shxzskj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ay.hahajie.cn

[J06] 计算两时间之差
来源：http://of.jianghongdianzi.cn

Py:   (end - start).total_seconds()
来源：http://qb.bookmarksfly.cn

PHP:  $end->diff($start)->days;
来源：http://hg.shtwfgs.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mm.newstarts.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yw.newstarts.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ek.hahajie.cn

Go:   end.Sub(start).Hours()
来源：http://kh.lnxyls.cn

Ruby: end - start                 # 返回秒数
来源：http://uh.bookmarksfly.cn

C#:   (end - start).TotalSeconds
来源：http://gb.chemitech.net.cn

[J07] 比较两个日期
来源：http://ac.colortex.cn

Py:   d1 < d2;  d1 == d2
来源：http://zd.wgjwhj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yr.asd995.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ak.shxzukj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bg.521024.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://na.panjiajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rj.wgjwhj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ow.jctech888.com.cn

C#:   d1 < d2;  d1 == d2
来源：http://ts.nszjky.cn

[J08] 提取年月日与星期
来源：http://hk.hnjuh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jf.shxzskj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zb.yuntaijiaju.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mv.chemitech.net.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ag.asd995.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://an.huixinmuqiang.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sp.shxzskj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qy.9csxet.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ul.haigaiapp.cn

[J09] 时区处理
来源：http://ai.huanxung.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lc.colortex.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cw.huixiangedu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zb.yuntaijiaju.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zk.hnjuh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://uy.gzmigu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tt.asd995.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ma.nszjky.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nm.panjiajie.cn

[J10] 取今天 / 本月第一天
来源：http://zh.jctech888.com.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cu.521024.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://py.nicolike.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ib.jctech888.com.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wg.huanxung.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xi.bjjhwx.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jg.newstarts.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kf.shtwfgs.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nw.jctech888.com.cn

================================================================================
来源：http://wx.shxzskj.cn

K. JSON 与序列化
来源：http://nd.szsharing.cn

================================================================================
来源：http://dy.shxzskj.cn

[K01] 对象转 JSON 字符串
来源：http://ta.haigaiapp.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dc.muxihuayi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rh.shxzskj.cn

JS:   JSON.stringify(obj)
来源：http://ul.hnjuh.cn

TS:   JSON.stringify(obj)
来源：http://ip.jianghongdianzi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://we.muxihuayi.cn

Go:   json.Marshal(obj)
来源：http://vb.yuexingan06.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ba.hnjuh.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://tc.yuntaijiaju.cn

[K02] JSON 字符串转对象
来源：http://ea.gzmigu.cn

Py:   json.loads(s)
来源：http://ro.9csxet.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gj.521024.cn

JS:   JSON.parse(s)
来源：http://iw.521024.cn

TS:   JSON.parse(s)
来源：http://dj.wgjwhj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wt.wgjwhj.cn

Go:   json.Unmarshal(data, &v)
来源：http://mc.huixinmuqiang.cn

Ruby: JSON.parse(s)
来源：http://uz.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sq.haigaiapp.cn

[K03] JSON 美化输出（带缩进）
来源：http://lc.hnjuh.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://av.nicolike.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://og.colortex.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://oj.jianghongdianzi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://oc.asd995.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://af.jctech888.com.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rr.yuexingan06.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jf.newstarts.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://og.jianghongdianzi.cn

[K04] 读取 JSON 文件
来源：http://uw.huanxung.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pe.yuntaijiaju.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://go.muxihuayi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ad.nszjky.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gn.9csxet.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vh.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ev.colortex.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ic.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://oz.newstarts.cn

[K05] 深拷贝对象
来源：http://xf.yuexingan06.cn

Py:   copy.deepcopy(obj)
来源：http://ju.gzmigu.cn

PHP:  unserialize(serialize($obj));
来源：http://gb.nszjky.cn

JS:   structuredClone(obj)
来源：http://in.huixiangedu.cn

TS:   structuredClone(obj)
来源：http://ne.yuexingan06.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ke.jctech888.com.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vo.yuexingan06.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yn.yuntaijiaju.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hh.jctech888.com.cn

[K06] 解析 URL 查询串
来源：http://sp.yuexingan06.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rj.nicolike.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://so.shxzskj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nm.huixiangedu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pl.newstarts.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ac.hahajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xe.chemitech.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ph.asd995.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ty.gzmigu.cn

[K07] 进制转换
来源：http://hb.huixinmuqiang.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fi.huixiangedu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ct.muxihuayi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yd.521024.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bw.szsharing.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fp.panjiajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jb.hnjuh.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://et.shtwfgs.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kj.yuntaijiaju.cn

[K08] 二进制序列化（非 JSON）
来源：http://tx.gzmigu.cn

Py:   pickle.dumps(obj)
来源：http://uc.yuexingan06.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wm.wgjwhj.cn

JS:   v8.serialize(obj)        // Node
来源：http://fm.colortex.cn

TS:   v8.serialize(obj)        // Node
来源：http://jd.jctech888.com.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xn.jctech888.com.cn

Go:   encoding/gob
来源：http://ew.jianghongdianzi.cn

Ruby: Marshal.dump(obj)
来源：http://zg.newstarts.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ur.chemitech.net.cn

================================================================================
来源：http://zt.shtwfgs.cn

L. 网络请求
来源：http://sx.szsharing.cn

================================================================================
来源：http://kk.jianghongdianzi.cn

[L01] 发送 GET 请求
来源：http://lg.jctech888.com.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xm.shxzukj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cn.asd995.cn

JS:   await fetch(url)
来源：http://xe.jctech888.com.cn

TS:   await fetch(url)
来源：http://nx.yuntaijiaju.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jd.muxihuayi.cn

Go:   resp, err := http.Get(url)
来源：http://yb.bookmarksfly.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ly.szsharing.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gu.wgjwhj.cn

[L02] 发送 POST JSON
来源：http://zx.huixinmuqiang.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bo.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ej.jctech888.com.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pm.muxihuayi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jt.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tk.huanxung.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qr.yuexingan06.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hb.nicolike.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tx.haigaiapp.cn

[L03] 设置自定义请求头
来源：http://my.huanxung.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mf.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://re.lnxyls.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ov.shxzukj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yv.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qu.chemitech.net.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jg.muxihuayi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fp.wgjwhj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://oc.huanxung.cn

[L04] 设置超时
来源：http://bq.jctech888.com.cn

Py:   requests.get(url, timeout=5)
来源：http://vf.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ff.wgjwhj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fd.haigaiapp.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cj.jianghongdianzi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dn.shxzukj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ae.asd995.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wf.szxytkj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pm.bjjhwx.cn

[L05] 上传文件（multipart）
来源：http://lm.9csxet.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gr.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sw.szxytkj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pl.jianghongdianzi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ok.newstarts.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hw.nicolike.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fq.colortex.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dn.lnxyls.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tl.wgjwhj.cn

[L06] 解析响应为 JSON
来源：http://zo.jctech888.com.cn

Py:   resp.json()
来源：http://bz.huixiangedu.cn

PHP:  json_decode($body, true);
来源：http://ox.shtwfgs.cn

JS:   await resp.json()
来源：http://cu.asd995.cn

TS:   await resp.json()
来源：http://aj.521024.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gg.shxzskj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wd.bookmarksfly.cn

Ruby: JSON.parse(resp.body)
来源：http://ef.huixiangedu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vm.asd995.cn

[L07] 处理 HTTP 状态码
来源：http://yh.wgjwhj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xv.nszjky.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gc.huixiangedu.cn

JS:   resp.ok;  resp.status
来源：http://je.shtwfgs.cn

TS:   resp.ok;  resp.status
来源：http://cq.shtwfgs.cn

Java: resp.statusCode()
来源：http://am.yuexingan06.cn

Go:   resp.StatusCode
来源：http://zm.haigaiapp.cn

Ruby: resp.code.to_i
来源：http://na.nszjky.cn

C#:   (int)resp.StatusCode
来源：http://pt.yuexingan06.cn

[L08] 并发请求多个地址
来源：http://xb.bookmarksfly.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cb.lnxyls.cn

PHP:  curl_multi_init() 系列
来源：http://jr.nszjky.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vy.yuexingan06.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qe.newstarts.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ea.nszjky.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://na.huixinmuqiang.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xo.521024.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gw.shxzskj.cn

================================================================================
来源：http://cb.huanxung.cn

M. 命令行 / 进程 / 环境
来源：http://nd.hnjuh.cn

================================================================================
来源：http://iy.jctech888.com.cn

[M01] 读取命令行参数
来源：http://rl.gzmigu.cn

Py:   sys.argv[1:]
来源：http://ij.shxzukj.cn

PHP:  $argv;  $argc;
来源：http://oa.asd995.cn

JS:   process.argv.slice(2)
来源：http://ue.shxzskj.cn

TS:   process.argv.slice(2)
来源：http://gc.gzmigu.cn

Java: args 数组（main 方法参数）
来源：http://ui.huixinmuqiang.cn

Go:   os.Args[1:]
来源：http://ed.shxzskj.cn

Ruby: ARGV
来源：http://ps.nicolike.cn

C#:   args 数组（Main 方法参数）
来源：http://ag.shtwfgs.cn

[M02] 读取环境变量
来源：http://qw.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://hj.chemitech.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sx.jctech888.com.cn

JS:   process.env.HOME
来源：http://ly.haigaiapp.cn

TS:   process.env.HOME
来源：http://gs.panjiajie.cn

Java: System.getenv("HOME")
来源：http://ob.jianghongdianzi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cc.shtwfgs.cn

Ruby: ENV["HOME"]
来源：http://jb.9csxet.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ac.szsharing.cn

[M03] 执行外部命令
来源：http://xw.huanxung.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ek.wgjwhj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hq.huixiangedu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gx.yuntaijiaju.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://oc.gzmigu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jp.haigaiapp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vk.shtwfgs.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jb.huixiangedu.cn

C#:   Process.Start("ls", "-l");
来源：http://mt.521024.cn

[M04] 获取当前工作目录
来源：http://ts.asd995.cn

Py:   os.getcwd()
来源：http://iv.521024.cn

PHP:  getcwd();
来源：http://eg.yuexingan06.cn

JS:   process.cwd()
来源：http://ez.nicolike.cn

TS:   process.cwd()
来源：http://rp.521024.cn

Java: Path.of("").toAbsolutePath()
来源：http://vw.hahajie.cn

Go:   os.Getwd()
来源：http://ay.szsharing.cn

Ruby: Dir.pwd
来源：http://oz.bookmarksfly.cn


<!-- 参考信息 -->