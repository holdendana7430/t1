代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://al.yuntaijiaju.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yn.521024.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gy.huixiangedu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hx.panjiajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mb.huixiangedu.cn

[I07] 忽略大小写与多行模式
来源：http://vo.jianghongdianzi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bj.shtwfgs.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rc.9csxet.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uj.huanxung.cn

TS:   /error/gim
来源：http://hi.szxytkj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pk.gzmigu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tu.shtwfgs.cn

Ruby: s.scan(/error/i)
来源：http://vv.521024.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wd.nszjky.cn

[I08] 贪婪与非贪婪匹配
来源：http://sz.muxihuayi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qv.yuexingan06.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://se.asd995.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tf.huixiangedu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dm.gzmigu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://oh.huixinmuqiang.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://de.lnxyls.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://my.nicolike.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lo.shtwfgs.cn

================================================================================
来源：http://gd.yuexingan06.cn

J. 日期与时间
来源：http://ge.hnjuh.cn

================================================================================
来源：http://gw.huixinmuqiang.cn

[J01] 获取当前时间
来源：http://zc.hahajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wl.yuntaijiaju.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tn.huanxung.cn

JS:   new Date();  Date.now()
来源：http://ru.hnjuh.cn

TS:   new Date();  Date.now()
来源：http://lj.hahajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://kv.jctech888.com.cn

Go:   time.Now()
来源：http://iu.shxzukj.cn

Ruby: Time.now
来源：http://rx.huanxung.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tf.panjiajie.cn

[J02] 格式化输出
来源：http://nl.huixinmuqiang.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pg.panjiajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vi.nicolike.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://oj.haigaiapp.cn

TS:   d.toISOString()
来源：http://ua.hahajie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pg.huixinmuqiang.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://br.bjjhwx.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bp.yuexingan06.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vj.shxzukj.cn

[J03] 字符串解析为日期
来源：http://xn.shtwfgs.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://md.shxzskj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wr.nicolike.cn

JS:   new Date("2024-01-02")
来源：http://bj.9csxet.cn

TS:   new Date("2024-01-02")
来源：http://mc.huanxung.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dv.panjiajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dc.bookmarksfly.cn

Ruby: Date.parse("2024-01-02")
来源：http://ji.szsharing.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jo.shxzskj.cn

[J04] 时间戳与日期互转
来源：http://ie.jianghongdianzi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ki.colortex.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mh.jctech888.com.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ov.yuntaijiaju.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jp.hnjuh.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ki.hahajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ma.lnxyls.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bk.jianghongdianzi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dx.jctech888.com.cn

[J05] 时间加减（加 7 天）
来源：http://pu.chemitech.net.cn

Py:   now + timedelta(days=7)
来源：http://ad.hahajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yl.nicolike.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yr.shxzskj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ak.newstarts.cn

Java: LocalDate.now().plusDays(7)
来源：http://oc.huixinmuqiang.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ao.bookmarksfly.cn

Ruby: Time.now + 7 * 86400
来源：http://pe.lnxyls.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gr.9csxet.cn

[J06] 计算两时间之差
来源：http://fa.chemitech.net.cn

Py:   (end - start).total_seconds()
来源：http://ed.9csxet.cn

PHP:  $end->diff($start)->days;
来源：http://hn.jctech888.com.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kk.jctech888.com.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://op.szsharing.cn

Java: Duration.between(start, end).toSeconds()
来源：http://pm.yuntaijiaju.cn

Go:   end.Sub(start).Hours()
来源：http://sk.gzmigu.cn

Ruby: end - start                 # 返回秒数
来源：http://im.newstarts.cn

C#:   (end - start).TotalSeconds
来源：http://mk.hnjuh.cn

[J07] 比较两个日期
来源：http://zt.nszjky.cn

Py:   d1 < d2;  d1 == d2
来源：http://gp.bjjhwx.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sh.gzmigu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qy.nicolike.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jn.jctech888.com.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kn.newstarts.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kt.nicolike.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cd.huixiangedu.cn

C#:   d1 < d2;  d1 == d2
来源：http://qr.szxytkj.cn

[J08] 提取年月日与星期
来源：http://re.asd995.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dz.bjjhwx.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ka.yuexingan06.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bl.hahajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vn.gzmigu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fz.bjjhwx.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fa.jianghongdianzi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wz.haigaiapp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vi.hahajie.cn

[J09] 时区处理
来源：http://ac.bookmarksfly.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gz.jctech888.com.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pf.chemitech.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gi.chemitech.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ba.521024.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://je.hahajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bb.hnjuh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ik.shtwfgs.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ap.colortex.cn

[J10] 取今天 / 本月第一天
来源：http://ox.shtwfgs.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vo.panjiajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bw.huixinmuqiang.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ke.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jf.haigaiapp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ec.huixinmuqiang.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fs.lnxyls.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://op.gzmigu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qa.hnjuh.cn

================================================================================
来源：http://yc.chemitech.net.cn

K. JSON 与序列化
来源：http://st.gzmigu.cn

================================================================================
来源：http://ir.nszjky.cn

[K01] 对象转 JSON 字符串
来源：http://nn.hahajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tg.newstarts.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mi.hahajie.cn

JS:   JSON.stringify(obj)
来源：http://ju.shxzskj.cn

TS:   JSON.stringify(obj)
来源：http://qd.9csxet.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nv.wgjwhj.cn

Go:   json.Marshal(obj)
来源：http://sc.hahajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cn.huanxung.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pi.szxytkj.cn

[K02] JSON 字符串转对象
来源：http://ev.bjjhwx.cn

Py:   json.loads(s)
来源：http://sq.hnjuh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ho.colortex.cn

JS:   JSON.parse(s)
来源：http://lo.nszjky.cn

TS:   JSON.parse(s)
来源：http://hi.huanxung.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pv.shxzskj.cn

Go:   json.Unmarshal(data, &v)
来源：http://ei.chemitech.net.cn

Ruby: JSON.parse(s)
来源：http://de.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yx.muxihuayi.cn

[K03] JSON 美化输出（带缩进）
来源：http://gg.lnxyls.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ty.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bv.hahajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://mu.wgjwhj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cz.huixinmuqiang.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hc.haigaiapp.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dz.huixiangedu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://om.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tj.newstarts.cn

[K04] 读取 JSON 文件
来源：http://wn.jianghongdianzi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ul.bookmarksfly.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ul.yuexingan06.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kx.colortex.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ps.hnjuh.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mb.hnjuh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wt.panjiajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qg.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ly.nicolike.cn

[K05] 深拷贝对象
来源：http://cg.yuexingan06.cn

Py:   copy.deepcopy(obj)
来源：http://bb.shxzukj.cn

PHP:  unserialize(serialize($obj));
来源：http://ln.521024.cn

JS:   structuredClone(obj)
来源：http://em.haigaiapp.cn

TS:   structuredClone(obj)
来源：http://wl.lnxyls.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ky.lnxyls.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mf.bookmarksfly.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lx.muxihuayi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vs.asd995.cn

[K06] 解析 URL 查询串
来源：http://bc.szxytkj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ka.nicolike.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://in.521024.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sh.muxihuayi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rc.colortex.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cs.huanxung.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://lp.huanxung.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mv.szxytkj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zz.521024.cn

[K07] 进制转换
来源：http://eh.newstarts.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pt.huanxung.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wh.haigaiapp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tq.nszjky.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gv.haigaiapp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sx.yuntaijiaju.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dk.wgjwhj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pp.szxytkj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bx.lnxyls.cn

[K08] 二进制序列化（非 JSON）
来源：http://py.asd995.cn

Py:   pickle.dumps(obj)
来源：http://xn.szxytkj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wy.colortex.cn

JS:   v8.serialize(obj)        // Node
来源：http://vg.haigaiapp.cn

TS:   v8.serialize(obj)        // Node
来源：http://jk.shtwfgs.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://js.panjiajie.cn

Go:   encoding/gob
来源：http://aw.jianghongdianzi.cn

Ruby: Marshal.dump(obj)
来源：http://ij.szsharing.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://od.wgjwhj.cn

================================================================================
来源：http://eo.hahajie.cn

L. 网络请求
来源：http://yv.bjjhwx.cn

================================================================================
来源：http://mt.shxzukj.cn

[L01] 发送 GET 请求
来源：http://cb.jianghongdianzi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wu.9csxet.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jb.haigaiapp.cn

JS:   await fetch(url)
来源：http://ql.huixiangedu.cn

TS:   await fetch(url)
来源：http://nc.lnxyls.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zb.9csxet.cn

Go:   resp, err := http.Get(url)
来源：http://px.newstarts.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://oi.hahajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vs.muxihuayi.cn

[L02] 发送 POST JSON
来源：http://sb.jctech888.com.cn

Py:   requests.post(url, json={"a": 1})
来源：http://oa.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qt.gzmigu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ze.wgjwhj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ag.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://af.shxzskj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://he.hahajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gr.huixinmuqiang.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xy.huixinmuqiang.cn

[L03] 设置自定义请求头
来源：http://ie.lnxyls.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cg.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uo.colortex.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://er.bookmarksfly.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ym.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ww.huanxung.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uf.yuexingan06.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yq.lnxyls.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://on.yuntaijiaju.cn

[L04] 设置超时
来源：http://wt.jctech888.com.cn

Py:   requests.get(url, timeout=5)
来源：http://gx.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yd.nszjky.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kq.muxihuayi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nj.haigaiapp.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sn.nszjky.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wd.szsharing.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://up.gzmigu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fy.yuexingan06.cn

[L05] 上传文件（multipart）
来源：http://sg.jctech888.com.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://su.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ji.szxytkj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tv.nicolike.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ul.yuntaijiaju.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://na.shxzskj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ft.shxzskj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mu.wgjwhj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sp.jianghongdianzi.cn

[L06] 解析响应为 JSON
来源：http://ka.panjiajie.cn

Py:   resp.json()
来源：http://lr.szxytkj.cn

PHP:  json_decode($body, true);
来源：http://vn.nszjky.cn

JS:   await resp.json()
来源：http://mo.lnxyls.cn

TS:   await resp.json()
来源：http://xa.muxihuayi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nb.szxytkj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ua.huixinmuqiang.cn

Ruby: JSON.parse(resp.body)
来源：http://fd.huanxung.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nj.gzmigu.cn

[L07] 处理 HTTP 状态码
来源：http://vx.szxytkj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zs.szxytkj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qy.yuntaijiaju.cn

JS:   resp.ok;  resp.status
来源：http://pk.asd995.cn

TS:   resp.ok;  resp.status
来源：http://so.521024.cn

Java: resp.statusCode()
来源：http://nv.9csxet.cn

Go:   resp.StatusCode
来源：http://iu.521024.cn

Ruby: resp.code.to_i
来源：http://yz.521024.cn

C#:   (int)resp.StatusCode
来源：http://bm.bookmarksfly.cn

[L08] 并发请求多个地址
来源：http://al.newstarts.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tn.yuexingan06.cn

PHP:  curl_multi_init() 系列
来源：http://my.chemitech.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ce.chemitech.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://te.shtwfgs.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qs.nszjky.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dd.jianghongdianzi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://oh.521024.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ni.9csxet.cn

================================================================================
来源：http://rs.shxzskj.cn

M. 命令行 / 进程 / 环境
来源：http://jr.szsharing.cn

================================================================================
来源：http://eu.hahajie.cn

[M01] 读取命令行参数
来源：http://zb.nicolike.cn

Py:   sys.argv[1:]
来源：http://uc.shxzukj.cn

PHP:  $argv;  $argc;
来源：http://mp.bookmarksfly.cn

JS:   process.argv.slice(2)
来源：http://mi.9csxet.cn

TS:   process.argv.slice(2)
来源：http://td.colortex.cn

Java: args 数组（main 方法参数）
来源：http://vt.gzmigu.cn

Go:   os.Args[1:]
来源：http://gj.nszjky.cn

Ruby: ARGV
来源：http://ni.nicolike.cn

C#:   args 数组（Main 方法参数）
来源：http://qc.gzmigu.cn

[M02] 读取环境变量
来源：http://xi.panjiajie.cn

Py:   os.environ.get("HOME")
来源：http://ek.asd995.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://az.shtwfgs.cn

JS:   process.env.HOME
来源：http://kn.jctech888.com.cn

TS:   process.env.HOME
来源：http://hh.huixiangedu.cn

Java: System.getenv("HOME")
来源：http://uu.lnxyls.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pw.lnxyls.cn

Ruby: ENV["HOME"]
来源：http://ik.panjiajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wz.szxytkj.cn

[M03] 执行外部命令
来源：http://dn.yuntaijiaju.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vb.huanxung.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ph.colortex.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kz.nicolike.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://sd.lnxyls.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cu.shtwfgs.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fc.hahajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hn.shtwfgs.cn

C#:   Process.Start("ls", "-l");
来源：http://sm.shxzukj.cn

[M04] 获取当前工作目录
来源：http://zd.jctech888.com.cn

Py:   os.getcwd()
来源：http://kd.nszjky.cn

PHP:  getcwd();
来源：http://cc.bjjhwx.cn

JS:   process.cwd()
来源：http://sz.yuntaijiaju.cn


<!-- 参考信息 -->