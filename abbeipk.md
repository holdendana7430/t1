代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lv.szxytkj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bq.huixiangedu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gq.bjjhwx.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sn.panjiajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cw.9csxet.cn

[I07] 忽略大小写与多行模式
来源：http://ny.nszjky.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ym.szsharing.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://at.521024.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ms.newstarts.cn

TS:   /error/gim
来源：http://uj.chemitech.net.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fg.yuexingan06.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lq.shxzukj.cn

Ruby: s.scan(/error/i)
来源：http://qy.yuexingan06.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oa.asd995.cn

[I08] 贪婪与非贪婪匹配
来源：http://ca.lnxyls.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://li.521024.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hk.muxihuayi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qy.gzmigu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ou.gzmigu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://eo.huanxung.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cd.hahajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ae.newstarts.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wa.szsharing.cn

================================================================================
来源：http://sj.muxihuayi.cn

J. 日期与时间
来源：http://tq.bookmarksfly.cn

================================================================================
来源：http://hv.shtwfgs.cn

[J01] 获取当前时间
来源：http://yy.bookmarksfly.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://tm.asd995.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vu.shxzskj.cn

JS:   new Date();  Date.now()
来源：http://io.szxytkj.cn

TS:   new Date();  Date.now()
来源：http://xh.jianghongdianzi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://gj.9csxet.cn

Go:   time.Now()
来源：http://vd.yuexingan06.cn

Ruby: Time.now
来源：http://hu.lnxyls.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nl.shtwfgs.cn

[J02] 格式化输出
来源：http://bf.9csxet.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wg.yuexingan06.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lp.huixiangedu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tu.yuntaijiaju.cn

TS:   d.toISOString()
来源：http://bs.muxihuayi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xg.asd995.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ih.521024.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nq.hahajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yu.huixiangedu.cn

[J03] 字符串解析为日期
来源：http://vy.shxzukj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://op.lnxyls.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wf.szsharing.cn

JS:   new Date("2024-01-02")
来源：http://cx.hahajie.cn

TS:   new Date("2024-01-02")
来源：http://th.nicolike.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ig.nicolike.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zk.szxytkj.cn

Ruby: Date.parse("2024-01-02")
来源：http://sj.hahajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cn.nszjky.cn

[J04] 时间戳与日期互转
来源：http://sq.chemitech.net.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tk.yuntaijiaju.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ob.gzmigu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://za.wgjwhj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qk.newstarts.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://te.9csxet.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bk.newstarts.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ow.szsharing.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zt.szxytkj.cn

[J05] 时间加减（加 7 天）
来源：http://ez.hnjuh.cn

Py:   now + timedelta(days=7)
来源：http://ge.nszjky.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://np.newstarts.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nt.haigaiapp.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yp.yuntaijiaju.cn

Java: LocalDate.now().plusDays(7)
来源：http://nn.jianghongdianzi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gb.nicolike.cn

Ruby: Time.now + 7 * 86400
来源：http://dp.jianghongdianzi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wf.hahajie.cn

[J06] 计算两时间之差
来源：http://te.haigaiapp.cn

Py:   (end - start).total_seconds()
来源：http://st.huixinmuqiang.cn

PHP:  $end->diff($start)->days;
来源：http://yd.chemitech.net.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wj.yuexingan06.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tj.nszjky.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qt.yuexingan06.cn

Go:   end.Sub(start).Hours()
来源：http://yg.hahajie.cn

Ruby: end - start                 # 返回秒数
来源：http://kn.shxzskj.cn

C#:   (end - start).TotalSeconds
来源：http://qb.shxzskj.cn

[J07] 比较两个日期
来源：http://ne.bookmarksfly.cn

Py:   d1 < d2;  d1 == d2
来源：http://if.shxzukj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ds.9csxet.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mn.jctech888.com.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bz.shtwfgs.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vi.chemitech.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ii.szsharing.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ic.szxytkj.cn

C#:   d1 < d2;  d1 == d2
来源：http://vq.lnxyls.cn

[J08] 提取年月日与星期
来源：http://fz.bjjhwx.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xz.shxzskj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fe.szsharing.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ii.bookmarksfly.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xv.yuexingan06.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://iz.chemitech.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kj.nicolike.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wl.huixiangedu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ec.nicolike.cn

[J09] 时区处理
来源：http://hc.nicolike.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pu.hnjuh.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://na.szsharing.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://na.newstarts.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xw.szsharing.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bl.9csxet.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qg.yuexingan06.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fi.hahajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ha.colortex.cn

[J10] 取今天 / 本月第一天
来源：http://lb.bjjhwx.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zi.shxzskj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uo.wgjwhj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xl.9csxet.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sh.huanxung.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wx.bjjhwx.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vx.chemitech.net.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zk.shtwfgs.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ht.hnjuh.cn

================================================================================
来源：http://qh.lnxyls.cn

K. JSON 与序列化
来源：http://bm.521024.cn

================================================================================
来源：http://mo.yuexingan06.cn

[K01] 对象转 JSON 字符串
来源：http://no.gzmigu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ym.hahajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pb.huixinmuqiang.cn

JS:   JSON.stringify(obj)
来源：http://xk.panjiajie.cn

TS:   JSON.stringify(obj)
来源：http://fw.muxihuayi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://go.asd995.cn

Go:   json.Marshal(obj)
来源：http://fw.521024.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ch.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qk.shxzskj.cn

[K02] JSON 字符串转对象
来源：http://jg.wgjwhj.cn

Py:   json.loads(s)
来源：http://pb.szsharing.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fp.hnjuh.cn

JS:   JSON.parse(s)
来源：http://oi.chemitech.net.cn

TS:   JSON.parse(s)
来源：http://gm.huanxung.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nr.shxzskj.cn

Go:   json.Unmarshal(data, &v)
来源：http://gj.nicolike.cn

Ruby: JSON.parse(s)
来源：http://zz.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hm.shtwfgs.cn

[K03] JSON 美化输出（带缩进）
来源：http://ei.nszjky.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ca.bookmarksfly.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zf.shtwfgs.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kc.newstarts.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ev.yuexingan06.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rm.jianghongdianzi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zr.haigaiapp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hs.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ld.huanxung.cn

[K04] 读取 JSON 文件
来源：http://bm.hnjuh.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nd.huanxung.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ea.szsharing.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ah.gzmigu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cm.yuexingan06.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cw.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jm.yuexingan06.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://tq.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ue.wgjwhj.cn

[K05] 深拷贝对象
来源：http://ro.szsharing.cn

Py:   copy.deepcopy(obj)
来源：http://ba.nicolike.cn

PHP:  unserialize(serialize($obj));
来源：http://pr.gzmigu.cn

JS:   structuredClone(obj)
来源：http://jd.521024.cn

TS:   structuredClone(obj)
来源：http://gu.szsharing.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zx.chemitech.net.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://uh.shxzukj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ex.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ac.521024.cn

[K06] 解析 URL 查询串
来源：http://bl.nszjky.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kv.nicolike.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mf.szxytkj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dv.yuexingan06.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eo.shxzskj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vp.huixiangedu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xp.shxzskj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://eo.hnjuh.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yo.newstarts.cn

[K07] 进制转换
来源：http://et.jianghongdianzi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xe.shtwfgs.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qv.shxzukj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sc.nicolike.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qx.nszjky.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://el.hahajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tc.asd995.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://af.shxzukj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://od.nicolike.cn

[K08] 二进制序列化（非 JSON）
来源：http://iy.lnxyls.cn

Py:   pickle.dumps(obj)
来源：http://io.gzmigu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hv.shxzukj.cn

JS:   v8.serialize(obj)        // Node
来源：http://qx.nicolike.cn

TS:   v8.serialize(obj)        // Node
来源：http://jd.jctech888.com.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hv.9csxet.cn

Go:   encoding/gob
来源：http://jn.bjjhwx.cn

Ruby: Marshal.dump(obj)
来源：http://om.szxytkj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rm.shxzskj.cn

================================================================================
来源：http://uj.9csxet.cn

L. 网络请求
来源：http://sz.hnjuh.cn

================================================================================
来源：http://ir.wgjwhj.cn

[L01] 发送 GET 请求
来源：http://ze.9csxet.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bj.hahajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qp.huanxung.cn

JS:   await fetch(url)
来源：http://yv.muxihuayi.cn

TS:   await fetch(url)
来源：http://vi.yuexingan06.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ju.bjjhwx.cn

Go:   resp, err := http.Get(url)
来源：http://ze.gzmigu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://vi.bookmarksfly.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://al.asd995.cn

[L02] 发送 POST JSON
来源：http://ml.szxytkj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://yx.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pw.muxihuayi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fv.colortex.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gf.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uj.gzmigu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gy.haigaiapp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ny.huanxung.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vw.lnxyls.cn

[L03] 设置自定义请求头
来源：http://tf.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qh.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ax.wgjwhj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ra.9csxet.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sp.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://me.asd995.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bd.chemitech.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://na.chemitech.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yi.szxytkj.cn

[L04] 设置超时
来源：http://pn.gzmigu.cn

Py:   requests.get(url, timeout=5)
来源：http://ew.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hn.huanxung.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wr.hahajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wi.hahajie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rc.521024.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dn.nszjky.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hg.shxzskj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://eb.gzmigu.cn

[L05] 上传文件（multipart）
来源：http://gu.muxihuayi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lv.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tk.521024.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lx.huanxung.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fo.newstarts.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ia.huixiangedu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sf.wgjwhj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hh.huanxung.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zc.colortex.cn

[L06] 解析响应为 JSON
来源：http://ir.newstarts.cn

Py:   resp.json()
来源：http://ei.newstarts.cn

PHP:  json_decode($body, true);
来源：http://ut.hnjuh.cn

JS:   await resp.json()
来源：http://zn.szxytkj.cn

TS:   await resp.json()
来源：http://vk.hnjuh.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fn.huanxung.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dg.521024.cn

Ruby: JSON.parse(resp.body)
来源：http://ws.nszjky.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xl.shxzukj.cn

[L07] 处理 HTTP 状态码
来源：http://gv.yuexingan06.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kd.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vc.colortex.cn

JS:   resp.ok;  resp.status
来源：http://pj.gzmigu.cn

TS:   resp.ok;  resp.status
来源：http://sm.shxzukj.cn

Java: resp.statusCode()
来源：http://fa.hahajie.cn

Go:   resp.StatusCode
来源：http://cm.newstarts.cn

Ruby: resp.code.to_i
来源：http://hk.bjjhwx.cn

C#:   (int)resp.StatusCode
来源：http://vd.huixiangedu.cn

[L08] 并发请求多个地址
来源：http://co.nszjky.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nf.jctech888.com.cn

PHP:  curl_multi_init() 系列
来源：http://dy.haigaiapp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jv.shxzukj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ma.huanxung.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gu.9csxet.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zi.gzmigu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hq.gzmigu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://oi.panjiajie.cn

================================================================================
来源：http://ib.521024.cn

M. 命令行 / 进程 / 环境
来源：http://lu.nszjky.cn

================================================================================
来源：http://rc.bjjhwx.cn

[M01] 读取命令行参数
来源：http://vb.shtwfgs.cn

Py:   sys.argv[1:]
来源：http://zo.panjiajie.cn

PHP:  $argv;  $argc;
来源：http://en.yuntaijiaju.cn

JS:   process.argv.slice(2)
来源：http://ws.jctech888.com.cn

TS:   process.argv.slice(2)
来源：http://nv.newstarts.cn

Java: args 数组（main 方法参数）
来源：http://vp.nszjky.cn

Go:   os.Args[1:]
来源：http://vh.gzmigu.cn

Ruby: ARGV
来源：http://oc.haigaiapp.cn

C#:   args 数组（Main 方法参数）
来源：http://ez.bookmarksfly.cn

[M02] 读取环境变量
来源：http://dj.nszjky.cn

Py:   os.environ.get("HOME")
来源：http://yi.huanxung.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://eq.chemitech.net.cn

JS:   process.env.HOME
来源：http://we.muxihuayi.cn

TS:   process.env.HOME
来源：http://cy.shtwfgs.cn

Java: System.getenv("HOME")
来源：http://yf.wgjwhj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gk.hahajie.cn

Ruby: ENV["HOME"]
来源：http://ag.gzmigu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cl.wgjwhj.cn

[M03] 执行外部命令
来源：http://oq.shxzskj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mf.chemitech.net.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gn.szsharing.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dr.wgjwhj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ty.nicolike.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bs.chemitech.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://pd.huixiangedu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://to.asd995.cn

C#:   Process.Start("ls", "-l");
来源：http://vc.lnxyls.cn

[M04] 获取当前工作目录
来源：http://jt.haigaiapp.cn

Py:   os.getcwd()
来源：http://wc.jctech888.com.cn

PHP:  getcwd();
来源：http://ln.haigaiapp.cn

JS:   process.cwd()
来源：http://in.yuexingan06.cn


<!-- 参考信息 -->