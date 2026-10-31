代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jf.9csxet.cn

TS:   /error/gim
来源：http://av.hnjuh.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gr.yuexingan06.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://za.bjjhwx.cn

Ruby: s.scan(/error/i)
来源：http://ql.panjiajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dz.huanxung.cn

[I08] 贪婪与非贪婪匹配
来源：http://tp.jianghongdianzi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vc.yuexingan06.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wg.jianghongdianzi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qh.yuexingan06.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qf.jctech888.com.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ih.yuexingan06.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dy.hahajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pl.bookmarksfly.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ri.bookmarksfly.cn

================================================================================
来源：http://yi.szxytkj.cn

J. 日期与时间
来源：http://hh.panjiajie.cn

================================================================================
来源：http://eb.wgjwhj.cn

[J01] 获取当前时间
来源：http://pm.newstarts.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rg.huixinmuqiang.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rm.huixinmuqiang.cn

JS:   new Date();  Date.now()
来源：http://di.bookmarksfly.cn

TS:   new Date();  Date.now()
来源：http://qf.asd995.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ag.szsharing.cn

Go:   time.Now()
来源：http://tw.szxytkj.cn

Ruby: Time.now
来源：http://sz.yuntaijiaju.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mf.shxzskj.cn

[J02] 格式化输出
来源：http://tp.szsharing.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lu.nicolike.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yo.shtwfgs.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yj.521024.cn

TS:   d.toISOString()
来源：http://jz.yuntaijiaju.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wc.szxytkj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gg.yuntaijiaju.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ln.huixinmuqiang.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vn.haigaiapp.cn

[J03] 字符串解析为日期
来源：http://yu.asd995.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ck.nszjky.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lw.nicolike.cn

JS:   new Date("2024-01-02")
来源：http://et.9csxet.cn

TS:   new Date("2024-01-02")
来源：http://od.shxzukj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mf.huanxung.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xe.nszjky.cn

Ruby: Date.parse("2024-01-02")
来源：http://qq.asd995.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zf.panjiajie.cn

[J04] 时间戳与日期互转
来源：http://tz.yuntaijiaju.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://in.shtwfgs.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://se.shtwfgs.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yd.szxytkj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://kn.muxihuayi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jq.huixinmuqiang.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hw.shtwfgs.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sp.9csxet.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dn.shxzskj.cn

[J05] 时间加减（加 7 天）
来源：http://hg.newstarts.cn

Py:   now + timedelta(days=7)
来源：http://by.colortex.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vw.yuntaijiaju.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zo.lnxyls.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xy.shxzskj.cn

Java: LocalDate.now().plusDays(7)
来源：http://rp.chemitech.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vu.szsharing.cn

Ruby: Time.now + 7 * 86400
来源：http://ww.shtwfgs.cn

C#:   DateTime.Now.AddDays(7)
来源：http://tc.haigaiapp.cn

[J06] 计算两时间之差
来源：http://yl.hnjuh.cn

Py:   (end - start).total_seconds()
来源：http://lj.shxzskj.cn

PHP:  $end->diff($start)->days;
来源：http://xf.jianghongdianzi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://am.szxytkj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cf.hahajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://px.chemitech.net.cn

Go:   end.Sub(start).Hours()
来源：http://da.panjiajie.cn

Ruby: end - start                 # 返回秒数
来源：http://bw.szxytkj.cn

C#:   (end - start).TotalSeconds
来源：http://qk.shxzukj.cn

[J07] 比较两个日期
来源：http://ub.521024.cn

Py:   d1 < d2;  d1 == d2
来源：http://xw.szxytkj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cu.newstarts.cn

JS:   d1.getTime() < d2.getTime()
来源：http://dn.szsharing.cn

TS:   d1.getTime() < d2.getTime()
来源：http://da.wgjwhj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wo.muxihuayi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xw.chemitech.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hj.huanxung.cn

C#:   d1 < d2;  d1 == d2
来源：http://iy.panjiajie.cn

[J08] 提取年月日与星期
来源：http://pn.szxytkj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mi.gzmigu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ja.yuexingan06.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gv.muxihuayi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://if.huixiangedu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vq.asd995.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yy.chemitech.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tf.wgjwhj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gq.bjjhwx.cn

[J09] 时区处理
来源：http://fc.nszjky.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jg.huanxung.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jd.muxihuayi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gk.szsharing.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lp.huanxung.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vo.hnjuh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hj.yuexingan06.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xz.haigaiapp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nq.hahajie.cn

[J10] 取今天 / 本月第一天
来源：http://oa.colortex.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ts.yuexingan06.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zt.nszjky.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hx.colortex.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vb.huanxung.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ta.szsharing.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://po.lnxyls.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sk.wgjwhj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ca.newstarts.cn

================================================================================
来源：http://hr.shtwfgs.cn

K. JSON 与序列化
来源：http://wx.huixinmuqiang.cn

================================================================================
来源：http://it.shxzskj.cn

[K01] 对象转 JSON 字符串
来源：http://cd.hnjuh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dr.jctech888.com.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hj.newstarts.cn

JS:   JSON.stringify(obj)
来源：http://us.nicolike.cn

TS:   JSON.stringify(obj)
来源：http://ug.jctech888.com.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://iq.lnxyls.cn

Go:   json.Marshal(obj)
来源：http://jc.bjjhwx.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ky.shxzukj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://nl.newstarts.cn

[K02] JSON 字符串转对象
来源：http://hl.bookmarksfly.cn

Py:   json.loads(s)
来源：http://pm.lnxyls.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nr.yuexingan06.cn

JS:   JSON.parse(s)
来源：http://ep.lnxyls.cn

TS:   JSON.parse(s)
来源：http://or.panjiajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ye.szsharing.cn

Go:   json.Unmarshal(data, &v)
来源：http://om.shxzskj.cn

Ruby: JSON.parse(s)
来源：http://gq.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gb.jianghongdianzi.cn

[K03] JSON 美化输出（带缩进）
来源：http://ij.muxihuayi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tg.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wx.shxzskj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qf.yuntaijiaju.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sd.jianghongdianzi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ad.asd995.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ju.shxzukj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pr.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xy.szxytkj.cn

[K04] 读取 JSON 文件
来源：http://pc.hahajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ge.nszjky.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ev.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jw.muxihuayi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://an.chemitech.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mu.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ky.hnjuh.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fg.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zw.muxihuayi.cn

[K05] 深拷贝对象
来源：http://sq.yuexingan06.cn

Py:   copy.deepcopy(obj)
来源：http://eu.colortex.cn

PHP:  unserialize(serialize($obj));
来源：http://ic.shxzukj.cn

JS:   structuredClone(obj)
来源：http://hn.huixiangedu.cn

TS:   structuredClone(obj)
来源：http://rn.shxzukj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ym.shxzukj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lo.huixiangedu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bi.panjiajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://jj.hnjuh.cn

[K06] 解析 URL 查询串
来源：http://az.shxzukj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ek.wgjwhj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://og.yuexingan06.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jc.jianghongdianzi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zu.bjjhwx.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://aw.chemitech.net.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://jq.bjjhwx.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cn.lnxyls.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://so.chemitech.net.cn

[K07] 进制转换
来源：http://og.bookmarksfly.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://oh.bjjhwx.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mz.nszjky.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ky.jianghongdianzi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kn.lnxyls.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://va.yuntaijiaju.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://al.521024.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://py.yuexingan06.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fb.szsharing.cn

[K08] 二进制序列化（非 JSON）
来源：http://jf.gzmigu.cn

Py:   pickle.dumps(obj)
来源：http://un.yuexingan06.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://py.huanxung.cn

JS:   v8.serialize(obj)        // Node
来源：http://gw.jctech888.com.cn

TS:   v8.serialize(obj)        // Node
来源：http://cz.9csxet.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://oc.yuexingan06.cn

Go:   encoding/gob
来源：http://jl.yuexingan06.cn

Ruby: Marshal.dump(obj)
来源：http://go.shtwfgs.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vh.huixiangedu.cn

================================================================================
来源：http://rg.shxzukj.cn

L. 网络请求
来源：http://rd.hnjuh.cn

================================================================================
来源：http://ca.nszjky.cn

[L01] 发送 GET 请求
来源：http://mv.asd995.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xc.shxzskj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://at.huanxung.cn

JS:   await fetch(url)
来源：http://tr.yuexingan06.cn

TS:   await fetch(url)
来源：http://jh.haigaiapp.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tt.lnxyls.cn

Go:   resp, err := http.Get(url)
来源：http://vo.huixinmuqiang.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ik.shtwfgs.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vf.colortex.cn

[L02] 发送 POST JSON
来源：http://of.chemitech.net.cn

Py:   requests.post(url, json={"a": 1})
来源：http://uz.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ws.hnjuh.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pe.haigaiapp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pj.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://oy.jianghongdianzi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kk.bjjhwx.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://or.9csxet.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lv.yuntaijiaju.cn

[L03] 设置自定义请求头
来源：http://dv.huixiangedu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fa.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pw.9csxet.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://so.hnjuh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ce.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lt.szxytkj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xr.nszjky.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gd.yuntaijiaju.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zk.lnxyls.cn

[L04] 设置超时
来源：http://hq.jctech888.com.cn

Py:   requests.get(url, timeout=5)
来源：http://cu.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fs.9csxet.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yg.9csxet.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vq.szsharing.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fb.asd995.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wz.nszjky.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uf.shtwfgs.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ql.jctech888.com.cn

[L05] 上传文件（multipart）
来源：http://tr.bjjhwx.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ru.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://br.shtwfgs.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rw.521024.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zz.bookmarksfly.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rz.yuexingan06.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rq.panjiajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ac.huanxung.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hg.colortex.cn

[L06] 解析响应为 JSON
来源：http://xd.huanxung.cn

Py:   resp.json()
来源：http://zd.shtwfgs.cn

PHP:  json_decode($body, true);
来源：http://qe.szxytkj.cn

JS:   await resp.json()
来源：http://zj.521024.cn

TS:   await resp.json()
来源：http://wo.bookmarksfly.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ew.huixiangedu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tp.nicolike.cn

Ruby: JSON.parse(resp.body)
来源：http://xt.szxytkj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://au.szxytkj.cn

[L07] 处理 HTTP 状态码
来源：http://xt.huixiangedu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jw.huixiangedu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gm.9csxet.cn

JS:   resp.ok;  resp.status
来源：http://jm.yuexingan06.cn

TS:   resp.ok;  resp.status
来源：http://az.hahajie.cn

Java: resp.statusCode()
来源：http://wr.lnxyls.cn

Go:   resp.StatusCode
来源：http://sb.asd995.cn

Ruby: resp.code.to_i
来源：http://yp.panjiajie.cn

C#:   (int)resp.StatusCode
来源：http://vw.asd995.cn

[L08] 并发请求多个地址
来源：http://hr.jianghongdianzi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ms.yuntaijiaju.cn

PHP:  curl_multi_init() 系列
来源：http://fk.nszjky.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://my.szxytkj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hf.shxzukj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yz.huanxung.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qz.newstarts.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://se.shxzukj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pg.wgjwhj.cn

================================================================================
来源：http://kd.yuexingan06.cn

M. 命令行 / 进程 / 环境
来源：http://xy.huixinmuqiang.cn

================================================================================
来源：http://im.szsharing.cn

[M01] 读取命令行参数
来源：http://le.chemitech.net.cn

Py:   sys.argv[1:]
来源：http://of.nicolike.cn

PHP:  $argv;  $argc;
来源：http://xn.shxzukj.cn

JS:   process.argv.slice(2)
来源：http://wt.huixinmuqiang.cn

TS:   process.argv.slice(2)
来源：http://vy.521024.cn

Java: args 数组（main 方法参数）
来源：http://ic.jctech888.com.cn

Go:   os.Args[1:]
来源：http://du.lnxyls.cn

Ruby: ARGV
来源：http://xz.shxzskj.cn

C#:   args 数组（Main 方法参数）
来源：http://zv.huixiangedu.cn

[M02] 读取环境变量
来源：http://mf.yuntaijiaju.cn

Py:   os.environ.get("HOME")
来源：http://va.nicolike.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rc.nicolike.cn

JS:   process.env.HOME
来源：http://fc.yuexingan06.cn

TS:   process.env.HOME
来源：http://qu.huixinmuqiang.cn

Java: System.getenv("HOME")
来源：http://mg.panjiajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oz.hnjuh.cn

Ruby: ENV["HOME"]
来源：http://gu.wgjwhj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zp.haigaiapp.cn

[M03] 执行外部命令
来源：http://wm.shxzskj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lv.yuexingan06.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vy.shxzukj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ay.yuntaijiaju.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zf.panjiajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zx.yuntaijiaju.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://md.521024.cn

Ruby: system("ls -l");  `ls -l`
来源：http://af.bookmarksfly.cn

C#:   Process.Start("ls", "-l");
来源：http://sv.shxzukj.cn

[M04] 获取当前工作目录
来源：http://bm.hahajie.cn

Py:   os.getcwd()
来源：http://tr.asd995.cn

PHP:  getcwd();
来源：http://nk.chemitech.net.cn

JS:   process.cwd()
来源：http://zz.521024.cn

TS:   process.cwd()
来源：http://yt.bookmarksfly.cn

Java: Path.of("").toAbsolutePath()
来源：http://zx.muxihuayi.cn

Go:   os.Getwd()
来源：http://zn.nszjky.cn

Ruby: Dir.pwd
来源：http://le.muxihuayi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://uo.jianghongdianzi.cn

[M05] 设置退出码
来源：http://yi.521024.cn

Py:   sys.exit(1)
来源：http://bz.nszjky.cn

PHP:  exit(1);
来源：http://sn.bookmarksfly.cn


<!-- 参考信息 -->