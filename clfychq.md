代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uk.yuntaijiaju.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://co.colortex.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ov.huixinmuqiang.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ko.panjiajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.szsharing.cn

[I07] 忽略大小写与多行模式
来源：http://gb.jctech888.com.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ix.szxytkj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qt.huixinmuqiang.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mq.hahajie.cn

TS:   /error/gim
来源：http://kt.colortex.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pq.huixinmuqiang.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ky.huanxung.cn

Ruby: s.scan(/error/i)
来源：http://ar.hahajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://da.szxytkj.cn

[I08] 贪婪与非贪婪匹配
来源：http://ma.gzmigu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nz.chemitech.net.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qh.gzmigu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gf.521024.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://li.newstarts.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ue.gzmigu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yj.bookmarksfly.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://av.szsharing.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://md.9csxet.cn

================================================================================
来源：http://ox.9csxet.cn

J. 日期与时间
来源：http://pm.nszjky.cn

================================================================================
来源：http://ob.bookmarksfly.cn

[J01] 获取当前时间
来源：http://cc.panjiajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ti.chemitech.net.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qu.shtwfgs.cn

JS:   new Date();  Date.now()
来源：http://mt.huixinmuqiang.cn

TS:   new Date();  Date.now()
来源：http://qx.jianghongdianzi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lv.shxzukj.cn

Go:   time.Now()
来源：http://vl.hnjuh.cn

Ruby: Time.now
来源：http://nj.szsharing.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bv.asd995.cn

[J02] 格式化输出
来源：http://lw.wgjwhj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ym.nicolike.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cz.shxzukj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ni.hnjuh.cn

TS:   d.toISOString()
来源：http://cj.yuexingan06.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ke.shxzukj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zr.hnjuh.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mv.huixiangedu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://au.yuexingan06.cn

[J03] 字符串解析为日期
来源：http://dn.yuexingan06.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://os.szsharing.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://do.haigaiapp.cn

JS:   new Date("2024-01-02")
来源：http://lq.shxzskj.cn

TS:   new Date("2024-01-02")
来源：http://km.szxytkj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ek.newstarts.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lq.nszjky.cn

Ruby: Date.parse("2024-01-02")
来源：http://gd.huanxung.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lo.bjjhwx.cn

[J04] 时间戳与日期互转
来源：http://rl.yuntaijiaju.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uj.huanxung.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qp.hnjuh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://im.jianghongdianzi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tp.newstarts.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rr.shxzskj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qi.nicolike.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qr.asd995.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vp.yuntaijiaju.cn

[J05] 时间加减（加 7 天）
来源：http://ca.colortex.cn

Py:   now + timedelta(days=7)
来源：http://aj.shtwfgs.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yw.gzmigu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://os.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://th.shxzskj.cn

Java: LocalDate.now().plusDays(7)
来源：http://oh.jctech888.com.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://oe.lnxyls.cn

Ruby: Time.now + 7 * 86400
来源：http://tm.hahajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://oz.szsharing.cn

[J06] 计算两时间之差
来源：http://av.chemitech.net.cn

Py:   (end - start).total_seconds()
来源：http://rf.shxzukj.cn

PHP:  $end->diff($start)->days;
来源：http://cg.newstarts.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pe.panjiajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gh.wgjwhj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zh.chemitech.net.cn

Go:   end.Sub(start).Hours()
来源：http://ku.szsharing.cn

Ruby: end - start                 # 返回秒数
来源：http://dk.panjiajie.cn

C#:   (end - start).TotalSeconds
来源：http://kt.hnjuh.cn

[J07] 比较两个日期
来源：http://sf.gzmigu.cn

Py:   d1 < d2;  d1 == d2
来源：http://la.szxytkj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vk.chemitech.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kz.colortex.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qp.szsharing.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://za.huanxung.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uw.shxzukj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qk.haigaiapp.cn

C#:   d1 < d2;  d1 == d2
来源：http://mi.bjjhwx.cn

[J08] 提取年月日与星期
来源：http://ry.hnjuh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xv.bookmarksfly.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qp.yuntaijiaju.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lk.nicolike.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ur.shxzskj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yt.huixiangedu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fh.yuexingan06.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dd.huixiangedu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xt.nicolike.cn

[J09] 时区处理
来源：http://sm.muxihuayi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://th.muxihuayi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://li.hahajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ui.bjjhwx.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://am.521024.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xx.shtwfgs.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yr.huanxung.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zn.jctech888.com.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ap.chemitech.net.cn

[J10] 取今天 / 本月第一天
来源：http://ri.szxytkj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://pa.szsharing.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://po.jctech888.com.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ol.shxzskj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://il.wgjwhj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lp.521024.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kj.bookmarksfly.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://es.yuexingan06.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ze.hnjuh.cn

================================================================================
来源：http://bk.nszjky.cn

K. JSON 与序列化
来源：http://od.huanxung.cn

================================================================================
来源：http://ti.chemitech.net.cn

[K01] 对象转 JSON 字符串
来源：http://tk.hahajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ka.muxihuayi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rl.szxytkj.cn

JS:   JSON.stringify(obj)
来源：http://vh.muxihuayi.cn

TS:   JSON.stringify(obj)
来源：http://ed.lnxyls.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zf.chemitech.net.cn

Go:   json.Marshal(obj)
来源：http://xb.yuntaijiaju.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hf.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xi.bookmarksfly.cn

[K02] JSON 字符串转对象
来源：http://jf.521024.cn

Py:   json.loads(s)
来源：http://fl.asd995.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://or.nszjky.cn

JS:   JSON.parse(s)
来源：http://xj.jianghongdianzi.cn

TS:   JSON.parse(s)
来源：http://ok.huixiangedu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jp.nszjky.cn

Go:   json.Unmarshal(data, &v)
来源：http://bd.hnjuh.cn

Ruby: JSON.parse(s)
来源：http://mw.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gx.szxytkj.cn

[K03] JSON 美化输出（带缩进）
来源：http://xz.yuntaijiaju.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jz.bookmarksfly.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pt.bjjhwx.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://lm.hahajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://th.nicolike.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vq.szsharing.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sj.newstarts.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hm.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pq.szxytkj.cn

[K04] 读取 JSON 文件
来源：http://mr.shxzskj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rd.nicolike.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pl.hahajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://my.bjjhwx.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yc.wgjwhj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sp.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vd.9csxet.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://nh.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uf.shxzukj.cn

[K05] 深拷贝对象
来源：http://ab.huixiangedu.cn

Py:   copy.deepcopy(obj)
来源：http://xk.yuntaijiaju.cn

PHP:  unserialize(serialize($obj));
来源：http://yn.muxihuayi.cn

JS:   structuredClone(obj)
来源：http://qf.huixinmuqiang.cn

TS:   structuredClone(obj)
来源：http://vn.wgjwhj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ez.huixinmuqiang.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hf.haigaiapp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xm.panjiajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hh.chemitech.net.cn

[K06] 解析 URL 查询串
来源：http://om.asd995.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bv.nszjky.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pj.shtwfgs.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qf.bjjhwx.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wn.jctech888.com.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ue.wgjwhj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zc.nicolike.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ys.hnjuh.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fk.nszjky.cn

[K07] 进制转换
来源：http://my.huanxung.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yc.shtwfgs.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hm.hahajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jr.nicolike.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nj.wgjwhj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ut.shtwfgs.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yn.shxzukj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pk.yuexingan06.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pp.szsharing.cn

[K08] 二进制序列化（非 JSON）
来源：http://cb.shtwfgs.cn

Py:   pickle.dumps(obj)
来源：http://di.bookmarksfly.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wm.wgjwhj.cn

JS:   v8.serialize(obj)        // Node
来源：http://vi.huixinmuqiang.cn

TS:   v8.serialize(obj)        // Node
来源：http://dz.colortex.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ca.chemitech.net.cn

Go:   encoding/gob
来源：http://fs.yuntaijiaju.cn

Ruby: Marshal.dump(obj)
来源：http://xo.521024.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zk.wgjwhj.cn

================================================================================
来源：http://cq.nicolike.cn

L. 网络请求
来源：http://as.muxihuayi.cn

================================================================================
来源：http://xg.muxihuayi.cn

[L01] 发送 GET 请求
来源：http://al.wgjwhj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pn.newstarts.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rt.shxzukj.cn

JS:   await fetch(url)
来源：http://lv.521024.cn

TS:   await fetch(url)
来源：http://co.newstarts.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mx.shtwfgs.cn

Go:   resp, err := http.Get(url)
来源：http://gc.wgjwhj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://lk.shtwfgs.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ex.yuexingan06.cn

[L02] 发送 POST JSON
来源：http://bk.jianghongdianzi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://dy.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ou.panjiajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jx.yuntaijiaju.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wj.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://st.jianghongdianzi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rm.hnjuh.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dy.muxihuayi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jb.shtwfgs.cn

[L03] 设置自定义请求头
来源：http://ta.shxzskj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jg.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kp.hahajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://um.newstarts.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uc.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zv.shxzskj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nr.yuntaijiaju.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://un.chemitech.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ca.bjjhwx.cn

[L04] 设置超时
来源：http://qw.jctech888.com.cn

Py:   requests.get(url, timeout=5)
来源：http://cu.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wx.muxihuayi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cv.muxihuayi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://an.wgjwhj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zs.jctech888.com.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tk.panjiajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xk.chemitech.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wj.521024.cn

[L05] 上传文件（multipart）
来源：http://gv.asd995.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zr.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tp.bjjhwx.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ks.nszjky.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cx.nicolike.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yn.nicolike.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jd.huixiangedu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zo.newstarts.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ki.shxzukj.cn

[L06] 解析响应为 JSON
来源：http://qb.panjiajie.cn

Py:   resp.json()
来源：http://ht.521024.cn

PHP:  json_decode($body, true);
来源：http://zn.9csxet.cn

JS:   await resp.json()
来源：http://ei.shxzukj.cn

TS:   await resp.json()
来源：http://re.colortex.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yr.9csxet.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wt.9csxet.cn

Ruby: JSON.parse(resp.body)
来源：http://vo.haigaiapp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://eo.bjjhwx.cn

[L07] 处理 HTTP 状态码
来源：http://xd.nszjky.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fx.gzmigu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dh.521024.cn

JS:   resp.ok;  resp.status
来源：http://pz.9csxet.cn

TS:   resp.ok;  resp.status
来源：http://yi.shtwfgs.cn

Java: resp.statusCode()
来源：http://xf.muxihuayi.cn

Go:   resp.StatusCode
来源：http://hf.521024.cn

Ruby: resp.code.to_i
来源：http://uf.hnjuh.cn

C#:   (int)resp.StatusCode
来源：http://tw.hahajie.cn

[L08] 并发请求多个地址
来源：http://sy.huixinmuqiang.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ue.panjiajie.cn

PHP:  curl_multi_init() 系列
来源：http://qp.nicolike.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tn.huixiangedu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://la.shxzukj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hk.yuexingan06.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://el.gzmigu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tc.newstarts.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dr.bjjhwx.cn

================================================================================
来源：http://me.yuexingan06.cn

M. 命令行 / 进程 / 环境
来源：http://ur.chemitech.net.cn

================================================================================
来源：http://ka.nszjky.cn

[M01] 读取命令行参数
来源：http://jy.newstarts.cn

Py:   sys.argv[1:]
来源：http://cl.9csxet.cn

PHP:  $argv;  $argc;
来源：http://ec.shtwfgs.cn

JS:   process.argv.slice(2)
来源：http://xc.bjjhwx.cn

TS:   process.argv.slice(2)
来源：http://ty.shtwfgs.cn

Java: args 数组（main 方法参数）
来源：http://mx.nicolike.cn

Go:   os.Args[1:]
来源：http://ho.lnxyls.cn

Ruby: ARGV
来源：http://wa.jianghongdianzi.cn

C#:   args 数组（Main 方法参数）
来源：http://rv.hnjuh.cn

[M02] 读取环境变量
来源：http://ln.szxytkj.cn

Py:   os.environ.get("HOME")
来源：http://yt.shtwfgs.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ka.huixinmuqiang.cn

JS:   process.env.HOME
来源：http://qo.521024.cn

TS:   process.env.HOME
来源：http://wy.shxzskj.cn

Java: System.getenv("HOME")
来源：http://dq.chemitech.net.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wg.wgjwhj.cn

Ruby: ENV["HOME"]
来源：http://yc.szxytkj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rz.haigaiapp.cn

[M03] 执行外部命令
来源：http://jh.wgjwhj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yi.wgjwhj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cv.shtwfgs.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://op.huixinmuqiang.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rp.shxzukj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ul.huixinmuqiang.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://bq.jctech888.com.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ao.colortex.cn

C#:   Process.Start("ls", "-l");
来源：http://wq.shxzskj.cn

[M04] 获取当前工作目录
来源：http://xk.huanxung.cn

Py:   os.getcwd()
来源：http://wh.szsharing.cn

PHP:  getcwd();
来源：http://os.bookmarksfly.cn

JS:   process.cwd()
来源：http://rz.wgjwhj.cn


<!-- 参考信息 -->